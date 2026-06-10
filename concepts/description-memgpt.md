> ✨ Translated automatically with [**Do-My-Work**](https://github.com/AlainCo/do-my-work) — profile: technical.

After this excellent introduction to MeMo, you will see that MemGPT is based on a radically different philosophy. Whereas MeMo offloads memory into a separate model to allow the main LLM to focus on reasoning, MemGPT makes the LLM its own memory manager.

This is a great analogy: **MemGPT treats AI as a genuine operating system (OS) for computers**, where the LLM is the conductor that decides what to keep in its "RAM" (random access memory) and what to archive on its "hard drive". A MemGPT agent doesn't just answer your questions; it can think, decide that what you just told it is crucial, and then write it into its memory to always remember it.

# 🤖 1. Architecture: The Three-Memory Hierarchy

MemGPT uses a three-level hierarchy, each with a very specific role, and **all are managed by the agent itself**.

## **Level 1: The "RAM" (Core Memory)**

This is the agent's immediate memory. It is very small but always accessible, and the agent can modify it directly. It contains vital information that must always be present:

- **Persona**: The agent's personality and goals (e.g., "My name is Chaz, I am an optimistic life coach").

- **Human**: Summarized information about the user (e.g., "The user's name is Bob, he is a developer and loves rock climbing").

### **Level 2: Archived Conversations (Recall Memory)**

It's the equivalent of an infinite logbook. **All** past conversations with the user are automatically saved here. The agent can dig into this past to retrieve the context of an old conversation.

### **Level 3: Knowledge (Archival Memory)**

This is the equivalent of a "hard drive" or a long-term library. It can contain external knowledge, entire documents (such as a 500-page product manual), or information that the agent has decided to keep forever. This is where technologies like a vector database (vector/embedding) are found for semantic searches.

## 🤝 2. Management by the "OS Agent": A Concrete Example

What makes MemGPT magical is its **"Self-Editing"** (self-modification) capability. The agent itself acts as the operating system kernel, orchestrating these back-and-forths between the levels of its memory.

**Let's take an example where you talk to "Bob", the MemGPT agent:**

- **Initialization**: In its Core memory, the agent Bob has its `Persona` ("I am helpful and concise") and an empty `Human` (it does not know you yet).

- **Discovery of a vital piece of information**: You tell Bob: *"I am allergic to peanuts, it's very important."* He reads this message.

- **Autonomous decision to write to RAM**: Bob (the LLM) analyzes this sentence and realizes that it is vital for your future interactions. He will **not** settle for storing this in his transient context. He uses a tool (Tool Call) called `core_memory_append` to add "The user is allergic to peanuts" directly into the `Human` block of his **Core Memory** (RAM).

- **End of conversation and archiving**: Your discussion continues. At some point, its context window (its immediate thoughts) starts to get full. Bob triggers his own "cleanup" mechanism:
  He will take the conversation history that is about to go out of his field of view.
  If it's unimportant, he discards it.
  **Key action**: He will compress the history into a **short summary** (recursive summary) and store it as a memory in the **Recall Memory**.

- **Awakening an old memory**: A month later, you ask him: *"Do you remember what we said about allergies?"* Bob no longer has it in his RAM. He will therefore use a **search** tool (`search_archival_memory`) that will dig into his "hard drive" (Archival/Recall). He finds the information, loads it into his context (RAM), and answers you: *"Yes, you are allergic to peanuts!"*

## ⚔️ 3. MemGPT vs. RAG vs. MeMo: The Final Synthesis

| Concept | RAG (Retrieval Augmented Generation) | MemGPT (Memory GPT) | MeMo (Memory as a Model) |
| :--- | :--- | :--- | :--- |
| **Metaphor** | The Passive Librarian | The Operating System | The Separate Brain |
| **Who manages the memory?** | An external system (Vector DB) that searches each turn. | **The agent itself** (the LLM), via autonomous function calls. | A **separate LLM**, specially trained to serve as memory. |
| **How does it store?** | Chunked/indexed documents, without judgment. | The agent decides **itself** what is important. It can write, replace, or delete its own memories. | Supervised learning: the memory model internalizes knowledge via a "reflection" pipeline. |
| **How does it respond?** | Search (embedding) → brute injection into context → generation. | **Hierarchy**: Fast (Core) or Long Search (Recall/Archival) at the agent's decision. | The main LLM decomposes the question → sends prompts to the memory model → the memory model generates the answer. |
| **Problem solved** | Forgets fewer facts (but sometimes off-topic). | **Autonomy** and **personalization** over the very long term (conversations lasting months). | **Robustness** (ignores noise) and **portability** of knowledge. |

## 💎 4. In Summary and Where to Use Them

- **Use RAG** when you need to efficiently search static documents.

- **Use MemGPT (or Letta)** if you are building a **smart conversational agent** that needs to learn from its interactions over time (a life coach, a personal assistant). The agent can evolve, remember your preferences, and infinitely archive its conversations.

- **Use MeMo** if you want to certify complex business knowledge, without modifying your LLM, and ensure that responses adhere to a documentary base without hallucination.

I will conclude with a clarification on the current state of the project: in 2024, the MemGPT repository has evolved. The official **framework** agent and supported by the startup founded by the researchers is now called **"Letta"** (while remaining open-source).

> ✨ Translated automatically with [**Do-My-Work**](https://github.com/AlainCo/do-my-work) — a tool designed to make projects speak globally.
