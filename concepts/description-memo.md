> ✨ Translated automatically with [**Do-My-Work**](https://github.com/AlainCo/do-my-work) — profile: technical.

This confusion between **MeMo** and other concepts (like **RAG** or **MemGPT**) is very common, as the ecosystem of memories for LLMs is in full effervescence. The article you are looking for (`arXiv:2605.15156`) is exactly called **"MeMo: Memory as a Model"**, and it proposes a particularly elegant architecture.

Here is a detailed explanation, from the basics to the technical mechanisms, to help you see clearly.

# 🤖 1. Clarification of fundamental terms

Before diving into the architecture, let's clarify the three concepts you mentioned: **token, embedding, and vector**. Understanding them is essential to grasp how MeMo works.

- **Token**: This is the basic unit that the LLM reads or generates. A token can be a whole word (`"car"`), part of a word (`"aut"` + `"omobile"`) or a character (`"!"`). For the same text, the number of tokens can vary depending on the tokenization method (e.g., `"J'adore les chats."` could become 4 or 5 tokens depending on the model). The token is the fundamental unit of reasoning for the LLM.

- **Embedding**: An embedding is the mathematical representation of a token (or a sentence, a document) in the form of a **list of floating-point numbers**. To obtain it, the token or text is passed through an embedding model (e.g., `text-embedding-3-small` from OpenAI). The embedding captures the **semantic meaning**: two words close in meaning will have embeddings close in the mathematical space. Embeddings are calculated **once** and stored (usually in a vector database).

- **Vector**: This is a generic mathematical structure — an ordered list of numbers. An embedding **is** a vector, but a vector is not necessarily an embedding. For example, the vector `[3.5, -1.2, 0.7]` is just numbers; for it to be an embedding, it must be the **result of passing text through an embedding model**. In the context of MeMo, the vector can be the embedding of a question or a document, but also an **internal representation** of the Memory model.

**Analogy**: Imagine a CSV file with thousands of columns. The first column contains the original phrase (`"The sky is blue"`). The following columns contain numerical values (`0.2`, `-0.5`, `0.8`, ...). The set of numerical values in a row constitutes **the embedding** of this phrase. The fact that these values are organized in a list makes it **a vector**.

## 🧠 2. MeMo Architecture: Two Models, One Memory

MeMo is based on a radical separation of responsibilities:

### **The Executive Model**

- This is the main LLM, capable of complex reasoning (e.g., GPT-4o, Gemini, Qwen).

- It is **completely frozen**: its weights are never modified, which eliminates any risk of "catastrophic forgetting" (loss of prior knowledge during retraining).

### **The Memory Model**

- A **smaller LLM** (Qwen2.5-14B in experiments) whose **sole function is to store and retrieve knowledge**.

- It is **specifically trained** on new knowledge (documents, databases) and its architecture is based on **layered associative memories** — a structure that mimics how the human brain associates ideas with each other.

**Key advantage**: Its small size makes it much less costly to retrain than the main LLM.

## 🎓 3. Training phase: Transforming documents into "reflections"

This is the most innovative part of MeMo. Instead of simply "chunking" (splitting) documents and indexing them (as RAG does), MeMo uses a **five-step reflection QA synthesis pipeline** to generate what the authors call **"reflections"**.

### **The 5 steps in detail**:

- **Fact extraction**: The `GENERATOR` model (Qwen2.5-32B) extracts from documents:
  Explicitly mentioned facts
  Information that can be logically inferred (inferences)
  Processing is done in parallel on each segment.

- **Consolidation**: QA pairs sharing a common context (same entity, same period, same relationship) are merged into multi-fact pairs.

- **Verification and rewriting**: Each QA pair is verified to ensure it is self-contained. Implicit references (e.g., "He said..." without mentioning "He") are rewritten to include the full context.

- **Entity surfacing**: Generation of QA pairs that force the model to handle relationships in both directions. This resolves the "reversal curse" (if the model has learned "A is B", it often fails on "B is A") by explicitly generating both formulations.

- **Cross-document synthesis**: Most critical step. The `GENERATOR` identifies and synthesizes two types of connections:
**Convergent cues**: Multiple documents discuss the same entity.
**Parallel properties**: Different entities share common attributes.
This step is so important that, in ablation, removing it causes precision to drop from **24.00% to 6.37%** on NarrativeQA.

The final product is a set of **QA pairs** that encapsulate the information from the source corpus from all angles. It is **this dataset** that will be used to train the **Memory Model**.

## ⚡ 4. Inference phase: A structured protocol in 3 phases

When a user asks a question, the interaction between the two models follows a well-defined protocol:

- **Decomposition** (Phase 1 — Grounding): The Executive Model receives the user's question `Q`. It does not respond directly. It analyzes `Q` and **decomposes it into several atomic sub-questions** `(q1, q2, q3,...)` which are independent units of knowledge.
*Example*: For the question `"What are the economic and ecological impacts of the new energy policy?"`, the sub-questions could be `"What are the economic impacts?"` and `"What are the ecological impacts?"`.

- **Interrogation** (Phase 2 — Querying): For each sub-question `q_i`, the Executive Model **formulates a prompt in natural language** and sends it to the Memory Model. This is where MeMo fundamentally differs from RAG:
  **RAG**: Converts `q_i` into an embedding, performs a similarity search in a vector database, and retrieves raw documents.
  **MeMo**: Sends **the text of `q_i`** to the Memory Model as one would send a query to an expert. The Memory Model, thanks to its training, is capable of **generating** the response (not searching for it) — this is **inference**, not retrieval.
  The result is a response `r_i` generated by the Memory Model.

- **Synthesis** (Phase 3 — Synthesis): The Executive Model receives all `(q_i, r_i)` pairs. It aggregates, confronts, and **synthesizes** them to produce the final response `R`, which is presented to the user.

This is the mechanism that the article summarizes with the triplet **"Memorization-retrieval-response"**.

## 🆚 5. Key Differences Between MeMo and RAG

The table below summarizes the fundamental architectural differences:

| Feature | RAG (Retrieval-Augmented Generation) | MeMo (Memory as a Model) |
| :--- | :--- | :--- |
| **Memory Nature** | Approximate text search (vector similarity) | A **trained model** that has *understood* and *internalized* the information |
| **Query Mechanism** | Embedding → Vector DB → Similarity Search | Natural language prompt → Memory model inference |
| **Cross-document Capacity** | Low (each chunk is independent) | Excellent (training step 5 explicitly synthesizes connections) |
| **Noise in Sources** | Very sensitive (the final LLM can be disrupted by noise) | Robust (the memory model learns to ignore noise during training) |
| **Update Cost** | Adding/replacing documents in the vector database | Retraining the memory model (less costly than a full LLM) |
| **Transparency** | Source documents are retrieved, but their interpretation remains opaque | Reasoning is humanly comprehensible QA pairs |

## 💎 6. In summary: The elegance of simplicity

The beauty of MeMo is that it solves three major problems of existing approaches:

- **Cost**: No retraining of the main LLM, only of the small memory model.

- **Obsolescence**: Possible updates without losing previous capabilities.

- **Portability**: Once trained, the memory model can be used with **any executive LLM** (open source or proprietary).

Technically, MeMo replaces approximate text search (RAG) with **targeted inference** and replaces costly retraining with **fine-tuning of a smaller model**. The end user sees only one response, but behind the scenes, it's a true collaboration between two distinct artificial intelligences.

> ✨ Translated automatically with [**Do-My-Work**](https://github.com/AlainCo/do-my-work) — a tool designed to make projects speak globally.
