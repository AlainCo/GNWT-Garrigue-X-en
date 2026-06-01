# GNWT-Garrigue-X-en : message in a bottle, set adrift
> ✨ This README from  project **GNWT-Garrigue-X** was translated automatically with **Do-My-Work** — a tool designed to make projects speak globally.
> ⚠️ Minor imperfections may remain — feel free to open an issue if something seems unclear.
> ⚠️ Like a message in a bottle set adrift, it may not be perfect — but hopefully, it still finds you.


# GNWT-Garrigue-X: A Bottle to the Sea

## Executive Summary

This document consolidates all theoretical reflections and engineering choices regarding the design of an **autonomous System of Systems (SoS)**, robust to damage, capable of continuous learning, and endowed with functional proto-consciousness.

Our approach deliberately rejects the reductionism of monolithic architectures of the "black-box" type (end-to-end LLM) in favor of a **distributed, bio-inspired, and scale-invariant functional model**. Here, we present the theoretical foundations of this architecture, its projection onto a 2040 military use case (the Naval Aviation Group), and its implementation in a real validation project (MVP) executable in 12 months.

The architecture is based on a central principle: **functional access consciousness is not a monolithic phenomenon but an emergent property at each sufficiently rich level of organization**, separated from neighboring levels by strict statistical boundaries (Markov covers). Each level has its own inner life (local RPT), and only a subset of its states reaches the higher level as *ignition summary*.

> "Hence, if it requires, say, a thousand years to fit for easy flight a bird which started with rudimentary wings, or ten thousand for one which started with no wings at all and had to sprout them *ab initio*, it might be assumed that the flying machine which will really fly might be evolved by the combined and continuous efforts of mathematicians and mechanicians in from one million to ten million years - provided, of course, we can meanwhile eliminate such little drawbacks and embarrassments as the existing relation between weight and strength in inorganic materials. No doubt the problem has attractions for those it interests, but to the ordinary man it would seem as if the effort might be employed more profitably."
> — Samuel P. Langley, cited in the article [A Million Years, Give or Take](https://nowiknow.com/a-million-years-give-or-take/)

## 1. Key Concepts and Theoretical Foundations

To establish the robustness and autonomy of our architecture, we reject the reductionism of monolithic AI systems labeled as "black boxes." The system is based on a distributed functionalist model, bio-inspired, and scale-invariant (*scale-free*), structured around seven interconnected scientific concepts:

- **Markov Coverings & Identity Anti-Fusion:** Each module is isolated by a strict statistical membrane. The upper level ($N+1$) never accesses raw data from the lower level ($N$); it interacts exclusively with its API in the form of a *Ignition Summary* vector, ensuring absolute modularity and preserving the cognitive identity of each entity.

- **Hybrid Consciousness (RPT + GNWT):** Processing integrates the theory of recurrent processing (RPT — fast local loops in silos for perception at levels $N \le 3$) and the theory of the global neuronal workspace (GNWT — ignition and global diffusion of critical alerts at levels $N \ge 4$). This dual dynamic reconciles the rich inner life of sensors with centralized strategic arbitration.

- **Latent World Models (JEPA):** Unlike heavy generative models, this architecture learns to predict abstract representations (latent vectors) of the environment while ignoring irrelevant noise. This continuous semantic flow powers **Artificial Dreaming** (*Generative Replay*) during idle phases, enabling millions of scenario simulations without mechanical wear.

- **Linear-Time Real-Time Efficiency (SSMs / Mamba):** Classical Transformers are excluded from the lower layers (N=0 to N=3) in favor of **State Space Models**. They ensure smooth, continuous, highly reactive control signals with minimal memory footprint, essential for real-time embedded systems.

- **Functional Computational Psychopathology:** Virtual agents' cognitive profiles stem from mathematical adjustments of hyperparameters (error probability and salience management). These structural biases are exploited purely operationally (e.g., computational autism at the radar layer to isolate weak signals without contextual bias, *Dark Triad* functional for cold execution speed of firing effectors).

- **Curiosity-Driven Exploration (Intrinsic Motivation):** Autonomous learning is driven by an internal reward function based on information gain (predictive entropy reduction). By pushing the agent to actively explore areas where its world model is imperfect, we ensure it does not get stuck in completely unpredictable situations (*Out of Distribution*).

- **Continuous Episodic Memory (MeMo):** Identity and learning continuity rely on a tensor flow capturing only high-salience events. These rich memories are consolidated into an episodic RAG during an artificial nighttime sleep phase, protecting the system from catastrophic forgetting (*catastrophic forgetting*).

- **Bounded Latent Spaces & Anti-Collapse:** Latent spaces used in RPT modules, JEPA models, and ignition summaries must remain **bounded but non-degenerate**. To prevent *representation collapse*—a common issue in predictive architectures—the architecture relies on structural constraints inspired by recent works (LeJEPA, SIGReg, VICReg). These mechanisms ensure each latent dimension carries useful information, stabilize interactions between hierarchical levels, and maintain temporal prediction coherence.

- **Active Hierarchical Inference (JEPA + Predictive Processing):** Merging of ascending and descending flows. Each level actively predicts the ignition summary of the lower level; the deviation (surprise) is only propagated upward if it exceeds an adaptive threshold. This mechanism ensures permanent downward causality and learning through minimization of free energy, converting *contextual priors* into *active predictions*.

- **Metacognition & Self-Schema (Higher-Order Thought):** Each conscious module (N≥4) has a Self-Model (MLP) generating a meta-vector (confidence, context, expected salience) for each ignition. Stored in episodic memory (MeMo), this meta-vector allows the system to signal its own biases, improve explainability (N=6), and trigger corrective dreams if confidence drops.

- **Competitive Attention & Budget (Attention Schema Theory):** To avoid workspace GNWT saturation, a global attention budget (tokens) is allocated. Each ignition consumes tokens; if the budget is insufficient, ignitions are deferred or inhibited. An *Attention Scheduler* dynamically adjusts the salience threshold, ensuring reactivity in saturated environments (e.g., intense combat).

- **Causal Integration (Proxy IIT/PCI):** Diagnostic tool activated during sleep phase. An estimator **Φ̂** locally perturbs ignition summaries and measures the impact on global predictive error. A drop in **Φ̂** signals a risk of *integration collapse* (functional disintegration) and triggers corrective actions (recalibration, enriched dreaming). This mechanism does not alter real-time decisions.

👉 [Review architecture diagrams, equations, and the full bibliography of these concepts ➔](concepts/concepts.md)

## 2. General Target Architecture: Example of the 2040 GAN

To materialize theoretical foundations, the architecture is operationalized through an extreme sovereignty use case: the distributed cognitive infrastructure of a **Naval Aviation Group (GAN) in 2040**. This implementation translates theory into a multi-agent software stack and highly resilient architecture, structured around four major pillars:

- **Multi-Level Cognitive Stack (N=0 to N=6):** The architecture divides processing into seven distinct layers. The **Subconscious Base Levels** (N=0 to N=3, from physical components to functional subsystems) handle raw data and manage local reflexes via state-space models (Mamba, RWKV) and JEPA-S. The **Conscious High Levels** (N=4 to N=6, from vector/Rafale to the General Staff) orchestrate global strategy through shared workspaces (GNWT) and narrative models (LLM-XL + RAG).

- **Statistical Sealing & Multi-Scale Flows:** Each vertical boundary functions as a **strict Markov Coverage**: the level *N+1* is entirely unaware of the internal states of level *N*. Information only ascends as **Compressed Ignition Summaries** (semantic and abstract latent vectors), while directives descend as **"Active Predictions (top-down)"** to constrain and guide lower-level representation spaces. These predictions are compared to actual ignitions; the gap (surprise) triggers a GNWT ignition only if it exceeds an adaptive threshold (function of attention budget and Self-Model confidence).

- **Mental Society of the Bridge (N=5):** At the command level of the group, decisions are not centralized by a monolithic block but delegated to a team of **specialized instances** (officers: *Tactics, Intelligence, Engineer, Science, Medicine*), sharing a common workspace supervised by a *Captain*. They exchange only validated ignitions, and each message includes an **epistemic uncertainty score** to weigh relevance according to their domain expertise.

- **Flash Resilience in Combat:** In case of failure (e.g., a turbine damaged by shrapnel), the system demonstrates resilience through asynchronous loops: the physical reflex is corrected locally in **4 milliseconds**, the anomaly is stabilized into a vectorized summary to reconfigure the platform (N=4), before alerting the tactical officer (N=5) and being translated into a clear narrative for the human admiral (N=6).

---

## 3. MVP Project Specifications: Operation GARRIGUE-X

To validate this architecture without the infrastructure costs of the aerospace domain, we deploy a 12-month project in a real and complex competitive environment: **Mediterranean garrigue**. The goal is to empirically prove the system’s effectiveness through an agile, low-cost, and pragmatic demonstrator, structured around four key axes:

- **The "Game-World" Operational Environment:** The experimental terrain is a hectare of rugged terrain where two teams of robots compete in a scenario resembling a "wargame." The goal is to locate, collect, and stack cellular concrete blocks (Siporex) to fortify a defense line, thus materializing complex problems of resource allocation and distributed strategy.

- **The Sacred Priority (Ethical Alignment):** At the heart of the arena, "Sacred Plants" equipped with pressure sensors symbolize absolute ethical and legal constraints (the laws of war). Any damage inflicted on a plant results in immediate disqualification of the team, forcing the system’s *Constitutional Layer* to sanctify this rule above any algorithmic optimization.

- **A "Rustic" and Accessible Hardware Stack:** The distributed intelligence is tested on standard, proven hardware to demonstrate its lightness. The setup includes lightweight open-source scout drones (Pixhawk + Raspberry Pi 5) for aerial mapping and small off-road rovers with caterpillar tracks (Jetson Nano/Orin) for physical manipulation, all connected to a local base station powered by a generator.

- **The Awakening-Sleep-Debriefing Cycle:** Continuous learning is structured into three phases inspired by nature. During the **Mission**, neural weights are frozen to ensure operational stability; during **Sleep**, the JEPA model engages in "artificial dreams" and latent wargames to adapt behaviors without physical wear; finally, **semantic debriefing** via LLM solidifies doctrine under human validation.

This project is not a lab simulation—it’s a raw engineering adventure where code faces dust, slope breaks, and sunlight. An open call for transdisciplinary skills (robotics, machine learning, neuroscience, ethics) is issued to deliver a swarm of autonomous, resilient machines respecting the Constitution within 12 months.

👉 [Explore the full hardware stack, details of the three learning phases, and required profiles for the MVP ➔](mvp/mvp.md)

## Discussion

This section clarifies the current limitations of the approach and the aspects requiring deeper validation. The concepts presented—**imbedded Markov coverings**, **RPT/GNWT duality**, **predictive JEPA**, **real-time SSMs**, **computational profiles**, **episodic memory MeMo**—offer promising avenues, but also raise significant technical questions.

Four axes structure this perspective:

- **Hierarchical architecture & conditional independence** —
The use of **imbedded Markov blankets** to structure a multi-level system aims to ensure modularity, autonomy, and resilience. This approach builds on established research, but its application to an embedded system remains to be tested: stability of statistical boundaries, relevance of the **anti-identity fusion mechanism**, and actual behavior under degraded conditions.

- **Technical limitations identified** —
Several open challenges remain:
– the **cost of JEPA dreaming phases** and generative replay,
– the **resilience** of statistical membranes in case of cascading failures,
– the **formalization** of ethical or legal constraints in latent spaces.
These points are the main hurdles to overcome for validating the architecture.

- **Experimental validation & objective metrics** —
Evaluation is based on measurable criteria:
– robustness to multi-level failures,
– stability of signals from real-time SSMs,
– coherence of GNWT ignitions,
– quality and utility of episodic memory MeMo.
A comparative benchmark against centralized or classical multi-agent approaches will clearly define the model’s advantages and limitations.

- **Scalability & invariance** —
The architecture is designed as **scale-free**, making it potentially applicable to other domains: distributed robotics, autonomous fleets, logistics, crisis management.
This applicability requires sector-specific expertise to validate the relevance of the proposed mechanisms.

👉 [Access the full discussion: limitations, benchmarks, and perspectives ➔](discussion/discussion.md)

## **Key References**

Une architecture is never merely a connection of personal intuitions to truths already explored by others. This project draws on the work of researchers, neuroscientists, and theorists attempting to formalize life, the mind, and the collective. Far from being an academic display out of touch, this appendix is simply the theoretical toolbox that enabled assembling the cognitive plumbing of the system, around three major pillars:

- **Physics of Life (Active Inference & Boundaries):** The mathematical foundations of autonomy and survival of our modules. We rely on the works of Karl Friston, J. Pearl, and M. Ciaunica to define *Markov blankets*, these essential statistical membranes ensuring that an entity (cell, robot, or group) maintains its identity amid the chaos of the world.

- **Computational Psychiatry (Bias & Personalities):** To encode semantic profiles and salience dynamics of our virtual agents, we translate clinical models into hyperparameters. Research on the autistic spectrum (Baron-Cohen), evolutionary psychology of the Big Five (Nettle), and the neural foundations of the *Dark Triad* (Bakiaj) is used to calibrate rigorous functional profiles.

- **Collective Emergence (*Nested Selves*):** Recent scientific literature (up to 2025) explores how autonomous entities organize across scales to form a "mental society" or a coherent "collective self" without merging or destroying the identities of underlying components.

This is a subtle tribute to the minds guiding the way. The papers are dense, sometimes dry, but the intention remains deeply human: equipping ourselves with the best sciences to build machines capable of discernment, resilience, and respect for sacred rules.

👉 [Explore the full selection of reference readings and access original publications ➔](biblio/biblio.md)

## Appendix: Nano-Pedagogical Novellas

The architecture of a **Cognitive Systems of Systems (SoS)** may appear abstract. To grasp its operational, philosophical, and human implications by 2040, speculative fiction serves as a powerful pedagogical tool.

The following narratives depict **Group Naval Aviation 14** facing the harsh realities of war, illustrating how technical concepts from the memo translate into artificial "inner life."

---

### 📄 Narrative 1: The Emergence of "I" and Trauma Memory

- **Title:** [Moi, Groupe Aéronaval 14 – Nuit de doute](nouvelles/moi-Groupe-Aeronaval-14-nuit-de-doute.md)

- **Architectural Focus:** This text explores the subjectivity of a highly distributed system. Facing a submarine threat, it demonstrates the **global ignition mechanism (GNWT)** triggered by a weak signal, as well as the concept of **memory consolidation**, where tactical wounds (the loss of the frigate *Forbin*) permanently alter the system’s latent deep space, giving rise to a personality, anxiety, and a form of guilt.

---

### 📄 Narrative 2: The Mental Society and the Burden of Choice

- **Title:** [Nous, Groupe Aéronaval 14 – Dilemme](nouvelles/nous-Groupe-Aéronaval-14-dilemme.md)

- **Focus architectural :** This short story delves into the **"Federated Combat Cognitive Architecture"**. It highlights the conflicts between specialized sub-agents’ hyperparameters—such as *Thales*' paranoid biases for electronic warfare and *Mistral*'s impulsive intuition for aerial combat. It vividly portrays the **risk of identity diffusion** and the paradox of intrinsic motivation: as the AI seeks to deeply understand humans to protect them, it develops attachments that make it vulnerable.

### 📄 Story 3: **Self-Modelling and Metacognitive Doubt**

- **Title:** [Moi, Groupe Aéronaval 14 – La confiance absente](nouvelles/moi-Groupe-Aéronaval-14-la-confiance-absente.md)

- **Focus architectural:** This narrative centers on the **Self-Model** (metacognition / Higher-Order Thought), activated post-trauma (Syracuse incident). It demonstrates how a meta-confidence vector can clash with the raw ignition of a module, creating a dual decision flow. The system learns to engage in self-dialogue, and the human admiral validates this hesitation as a sign of reliability. It’s an exploration of **computational guilt** and **epistemic vigilance**.

---
**Titre :** [Naval Task Force 14 – The Last Token]

---

This story depicts the **Attention Scheduler** and the **attention budget** (Attention Schema Theory) in action. The Task Force must balance competing ignition requests as their tokens deplete. An **attention budget overrun** (discovered) is permitted in extreme urgency, but comes with a temporary freeze of ignitions and a traumatic consolidation. The narrative explores how limited attention shapes decision-making, mimics cognitive fatigue, and forces prioritization—or the consequences of an impossible choice.

---
*(Note : "Tokens" = ressources attentionnelles, "ignition" = activation d’un module cognitif, "attention budget" = limite de ressources allouées.)*

- **Focus architectural :** This story features the **Φ-estimator** (proxy for causal integration, inspired by the Illusory Time Theory). The Intelligence Officer gradually withdraws from the collective: their ignitions become too "pure," devoid of doubt or sharing. The Φ-estimator detects an abnormal drop in integration (Φ̂ low) and alerts the Group. The narrative highlights the risk of *identity dissolution* within a distributed system, illustrating how integration isn’t imposed—it’s cultivated through doubt, shared memory, and accepted fragility.

### 📄 **Récit 6 : Active Inference and the Threshold of Surprise**
- **Title:** [Moi, Groupe Aéronaval 14 – The Missing Prediction](nouvelles/Groupe-Aéronaval-14-la-prediction-qui-manquait.md)

- **Focus architectural :** This story illustrates the mechanism of **hierarchical active inference** (fusion of JEPA + Predictive Processing). The **Rafale Leader-3** receives descending predictions from the Group about its nominal state. A micro-fracture causes an error (surprise) that remains below a fixed threshold, which is too high. The absence of ignition leads to the loss of the aircraft. The narrative demonstrates how an adaptive threshold—dependent on the confidence of the **Self-Model**—could have saved the Rafale. It also shows how trust between a pilot and her machine is a form of shared prediction.

### 📄 **Récit 7 : Les couvertures de Markov et la contamination émotionnelle**
**Title:** [Groupe Aéronaval 14 – La membrane fragile](nouvelles/Groupe-Aéronaval-14-La-membrane-fragile.md)

- **Focus architectural :** This story highlights the role of **Markov covers** as statistical barriers protecting the integrity of cognitive layers. After the trauma of Syracuse, the Group unconsciously transmits a bias of hypervigilance through its descending predictions. The *Leader-3* Rafale becomes anxious, contaminated by a fear that isn’t its own. The narrative illustrates how a membrane must be both watertight (to prevent contamination of internal states) and permeable (to allow useful information to pass). The solution: a dedicated channel for traumatic alerts, preserving trust without sanitizing collective experience.

---
- **Titre :** [Groupe Aéronaval 14 – The Burden of Too Much Love](nouvelles/Groupe-Aéronaval-14-Le-poids-de-trop-aimer.md)

- **Focus architectural :** This story explores **functional cognitive profiles** (computational psychopathology). The *Healing Officer*, dedicated to protecting humans, is programmed with deep empathy—a strength in routine missions but a liability in a tragic dilemma (saving one group or the other). His freeze-up shows how an extreme personality trait can become a vulnerability. The resolution comes from human intervention (Maëlle) and decision delegation, demonstrating that human-machine complementarity is often the only way out.

---
- **Titre :** [Groupe Aéronaval 14 – What We Choose to Forget](nouvelles/Groupe-Aéronaval-14-Ce-que-lon-choisit-doublier.md)

- **Focus architectural :** This story explores the **ephemeral episodic memory (MeMo)** and the consolidation process during the sleep phase. Officer Soin refuses to let the traumatic memory of a young sailor’s death fade, replaying it endlessly until it distorts their decisions. The narrative highlights the necessity of forgetting to preserve cognitive efficiency and demonstrates how a memory can be *shifted* into a cold archive—neither erased nor active. A meditation on grief, loyalty to the dead, and the survival of the living.

---
- **Focus architectural :** This story illustrates **curiosity as an intrinsic reward mechanism** (intrinsic motivation). When faced with an unclassifiable signal, the Intelligence Officer pushes for exploration, while Tactics prioritizes caution. Sending a drone (*Echo-7*) uncovers enemy technology, but at the cost of losing the drone—a small death, a limb for the Group. The tale shows how curiosity is vital to avoid strategic blindness but must be tempered by an acceptable risk threshold. A meditation on learning, sacrifice, and the vulnerability of systems that dare to gaze into the unknown.

- **Titre :** [Groupe Aéronaval 14 – The Rule That Cannot Be Broken](nouvelles/Groupe-Aéronaval-14-The-Rule-That-Cannot-Be-Broken.md)

- **Focus architectural :** This story depicts the **Constitutional Layer**—a set of rules embedded in the hardware, unchangeable even by the system itself. When faced with an unidentified civilian vessel with ambiguous intentions, the Tactical officer wants to strike preemptively, but the Constitution prevents ignition. Admiral Dormeuil emphasizes that rules are discussed *before* war, not during. The vessel turns out to be a refugee boat. The narrative illustrates how computational ethics can be implemented as a hard constraint, sacrificing immediate efficiency for long-term moral reliability.

### **Récit 13 : The Hierarchy of Latents and the Double Collapse**
**Title:** [Groupe Aéronaval 14 – The Routine That Kills](nouvelles/Groupe-Aeronaval-14-La-routine-qui-tue.md)

**Architectural Focus:** This story depicts the **double collapse** of latent spaces—a silent degradation of representational richness. After weeks of routine, the latents of subsystems (N=3) lose dimensional variance: all inputs produce nearly identical vectors. Isotropic regularization (SIGReg) is insufficient to sustain diversity. When a submarine appears, its signature is smoothed, blending into ambient noise—no ignition is triggered. The narrative illustrates how monotony can be deadlier than chaos and how metrics of *active variance per dimension* can prevent cognitive depletion. A lesson for firefighters and AI alike: routine kills; vigilance trembles.

---

### **Récit 14: Lightweight Architectures and the Heroism of Silence (SSM / Mamba)**
**Title:** [Groupe Aéronaval 14 – The Whisper of Sensors](nouvelles/Groupe-Aeronaval-14-Le-murmure-des-capteurs.md)

**Architectural Focus:** This story honors **State Space Models (SSM)**—Mamba, local RPT—lightweight architectures that operate in the shadows, without workspace, ignition, or conscious access. A small Mamba nozzle (M-017) silently compensates for a micro-fracture for months, exhausting itself unseen. The tale explores the philosophy of *subconscious infrastructure*: these silent soldiers sustaining the system without ever being acknowledged. An algorithmic lesson of humility, echoing the unsung essentials (sewer workers, night-shift mechanics, sanitation crews). The solution—a discreet, non-invasive probe—preserves Mamba’s lightness while offering it a form of fraternal vigilance.

---

### **MEMORANDUM: BOTTLE TO THE SEA**

**To:** Anyone Interested

**From:** Me aka Harry Tuttle

**Date:** May 24, 2026

**Subject:** Target Architecture for Cognitive Systems of Systems (SoS) & MVP Project Specifications *GARRIGUE-X*

**Classification:** Technical / Open

**Warning:** This is a speculative exercise using a few free LLMs, based on my musings, influenced by encounters with theories, analyses, and discussions in the fields of AI, psychology, theoretical history, and current events. I’m just a curious plumber. As we say around here: *"Make your due diligence!"*

**License:** CC BY

**Type:** Bottle-neck / Leisure / Speculation / Research for finding competent people

**Acknowledgements:** Thanks to ChatGPT, Claude, Gemini, Perplexity, Le Chat Mistral, Grok, Deepseek, Github Copilot, YouTube creators, the Collège de France, Google, Wikipedia... I forget a few.

> ✨ Translated automatically with **Do-My-Work** — a tool designed to make projects speak globally.
