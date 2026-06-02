# GNWT-Garrigue-X-en : message in a bottle, set adrift
> ✨ This README from  project **GNWT-Garrigue-X** was translated automatically with **Do-My-Work** — a tool designed to make projects speak globally.
> ⚠️ Minor imperfections may remain — feel free to open an issue if something seems unclear.
> ⚠️ Like a message in a bottle set adrift, it may not be perfect — but hopefully, it still finds you.


# GNWT-Garrigue-X: A BOTTLE TO THE SEA

## Executive Summary

This document consolidates all theoretical reflections and engineering choices regarding the design of an **autonomous System of Systems (SoS)**, resilient to damage, capable of continuous learning, and endowed with a functional proto-consciousness.

Our approach deliberately rejects the reductionism of monolithic "black-box" architectures (end-to-end LLMs) in favor of a **distributed, bio-inspired, scale-invariant functionalist model**. Here, we present the theoretical foundations of this architecture, its projection onto a military use case by **2040** (the Naval Aerospace Group), and its implementation as a real validation project (MVP) executable within 12 months.

The architecture is built on a core principle: **functional access consciousness is not a monolithic phenomenon, but an emergent property at every sufficiently rich organizational level**, separated from neighboring levels by strict statistical boundaries (Markov covers). Each level has its own internal dynamics (local RPT), and only a subset of its states ascends to the higher level in the form of an *ignition summary*.

> "Hence, if it takes, say, a thousand years to evolve a bird capable of easy flight starting from rudimentary wings, or ten thousand years for one that starts with no wings at all and must develop them *ab initio*, it might be assumed that the flying machine that will truly fly could be evolved through the combined and continuous efforts of mathematicians and mechanicians over a span of one million to ten million years—provided, of course, we can meanwhile eliminate such minor drawbacks and inconveniences as the current relationship between weight and strength in inorganic materials. No doubt the problem has its appeal for those it interests, but to the ordinary person, it would seem as if the effort might be better spent elsewhere."

— Samuel P. Langley, quoted in the article [A Million Years, Give or Take](https://nowiknow.com/a-million-years-give-or-take/)

## 1. Key Concepts and Theoretical Foundations

To ground the robustness and autonomy of our architecture, we reject the reductionism of monolithic "black-box" AI systems. The system is built on a **distributed functionalist model**, bio-inspired and **scale-free**, structured around seven interconnected scientific concepts:

- **Markovian Covers & Identity Anti-Merging:** Each module is isolated by a strict statistical membrane. The higher level ($N+1$) never accesses raw data from the lower level ($N$); it interacts exclusively with its API in the form of a **vectorial Ignition Summary**, ensuring absolute modularity and preserving the cognitive identity of each entity.

- **Hybrid Consciousness (RPT + GNWT):** Processing integrates **Recurrent Processing Theory** (RPT—fast local loops in silos for perception at level $N \le 3$) with **Global Neuronal Workspace Theory** (GNWT—*ignition* and global diffusion of critical alerts at level $N \ge 4$). This dual dynamic reconciles a rich sensor-driven inner life with centralized strategic arbitration.

- **Latent World Models (JEPA):** Unlike heavy generative models, the architecture learns to predict abstract representations (latent vectors) of the environment while ignoring irrelevant noise. This continuous semantic flow powers *Artificial Reverie* (*Generative Replay*) during rest phases, enabling the simulation of millions of scenarios without mechanical wear.

- **Linear-Time Real-Time Efficiency (SSMs / Mamba):** Classical Transformers are replaced in the lower layers ($N=0$ to $N=3$) in favor of *State Space Models*. These ensure smooth, continuous, highly reactive control signals with low memory footprint, essential for real-time embedded systems.

- **Functional Computational Psychopathology:** The cognitive profiles of virtual agents stem from mathematical adjustments of hyperparameters (error probability and salience management). These structural biases are leveraged for purely operational purposes (e.g., computational autism at the radar layer to isolate weak signals without contextual bias, *Dark Triad* functional for cold execution speed of firing effectors).

- **Exploration by Curiosity (Intrinsic Motivation):** Autonomous learning is driven by an internal reward function based on information gain (reduction of predictive entropy). By pushing the agent to actively explore areas where its world model is imperfect, we ensure it won’t get stuck in totally unforeseen situations (*Out of Distribution*).

- **Continuous Episodic Memory (MeMo):** Identity and learning continuity rely on a tensor stream capturing only high-salience events. These rich memories are consolidated into an episodic RAG during an artificial nighttime sleep phase, protecting the system against catastrophic forgetting.

- **Latent Space Stability & Anti-Collapse**: The latent spaces used in RPT modules, JEPA models, and Ignition summaries must remain **bounded but non-degenerate**. To prevent *representation collapse*—a common risk in predictive architectures—the architecture relies on structural constraints inspired by recent work (LeJEPA, SIGReg, VICReg). These mechanisms ensure that each dimension of the latent space carries meaningful information, stabilize exchanges between hierarchical levels, and maintain prediction consistency over time.

- **Active Hierarchical Inference (JEPA + Predictive Processing):** Unification of bottom-up and top-down flows. Each level actively predicts the ignition summary of the level below; the discrepancy (surprise) only propagates upward if it exceeds an adaptive threshold. This mechanism enforces continuous top-down causality and learning via free-energy minimization, turning *contextual priors* into *active predictions*.

- **Metacognition & Self-Schema (Higher-Order Thought):** Each conscious module (N≥4) has a Self-Model (MLP) that generates a meta-vector (confidence, context, expected salience) for each ignition. Stored in episodic memory (MeMo), this meta-vector enables the system to signal its own biases, improve explainability (N=6), and trigger corrective daydreams in case of confidence drop.

- **Competitive Attention & Budget (Attention Schema Theory):** To prevent saturation of the GNWT workspace, a global attention budget (in tokens) is allocated. Each ignition consumes tokens; if the budget is insufficient, ignitions are delayed or inhibited. An *Attention Scheduler* dynamically adjusts the salience threshold, ensuring reactivity in saturated environments (e.g., intense combat).

- **Causal Integration (Proxy IIT/PCI):** A diagnostic tool activated during sleep phases. An estimator **Φ̂** locally perturbs ignition summaries and measures the impact on global predictive error. A drop in **Φ̂** signals a risk of *integration collapse* (functional disintegration) and triggers corrective actions (recalibration, enriched daydreaming). This mechanism does not alter real-time decisions.

👉 [View the architecture diagrams, equations, and full bibliography of these concepts ➔](concepts/concepts.md)

## 2. General Target Architecture: Example of the **GAN 2040**

To materialize the theoretical foundations, the architecture is operationalized through a use case of extreme sovereignty: the distributed cognitive infrastructure of a **Naval Air Group (GAN) in 2040**. This implementation translates theory into a highly resilient, multi-agent software stack, structured around four core pillars:

- **Multi-Level Cognitive Stack (N=0 to N=6):** The architecture segments processing into seven distinct layers. The *Low-Level subconscious layers* ($N=0$ to $N=3$, from physical components to functional subsystems) handle raw data and manage local reflexes through state-space models (Mamba, RWKV) and JEPA-S. The *High-Level conscious layers* ($N=4$ to $N=6$, from vector/Rafale to the High Command) orchestrate global strategy via shared workspaces (GNWT) and narrative models (LLM-XL + RAG).

- **Statistical Tightness & Multi-Scale Flows:** Each vertical boundary acts as a *strict Markov blanket*: level $N+1$ is completely blind to the internal states of level $N$. Information only propagates upward in the form of **Compressed Ignition Summaries** (semantic and abstract latent vectors), while directives flow downward as "active predictions (top-down)" to constrain and guide the representation spaces of lower layers. These predictions are compared to actual ignitions; the discrepancy (surprise) triggers a GNWT ignition only if it exceeds an adaptive threshold (a function of attentional budget and the Self-Model’s confidence).

- **Mental Society of the Passerelle (N=5):** At the group command level, decision-making is not centralized by a monolithic block but entrusted to a team of **specialized instances** (the Officers: *Tactics, Intel, Engineer, Science, Medical*) sharing a common workspace overseen by a *Captain*. They only exchange their validated triggers, and each message includes an *epistemic uncertainty score* to weight their relevance according to their area of expertise.

- **Flash Resilience in Combat:** In case of a malfunction (e.g., a nozzle damaged by shrapnel), the system demonstrates its robustness through asynchronous loops: the physical reflex is corrected locally in **4 milliseconds**, the stabilized anomaly is converted into a vector summary to reconfigure the platform ($N=4$), before alerting the tactical officer ($N=5$) and being translated into clear narrative language for the human Admiral ($N=6$).

👉 [View the Mermaid diagrams, the consciousness matrix, and the full operational scenario of the GAN 2040 ➔](architecture/architecture.md)

## 3. MVP Project Specifications: Operation GARRIGUE-X

To validate this architecture without the infrastructure costs of the aeronautical domain, we are deploying a 12-month project in a real and complex competitive environment: **the Mediterranean garrigue**. The goal is to empirically prove the system's effectiveness through an agile, low-cost, and pragmatic demonstrator, structured around four main pillars:

- **The "Operational Game World":** The experimental site is a hectare of rugged terrain where two teams of robots compete in a "wargame"-style scenario. The goal is to locate, collect, and stack lightweight concrete blocks (Siporex) to fortify a defensive line, thereby embodying complex challenges in resource allocation and distributed strategy.

- **The Sacred Priority (Ethical Alignment):** At the center of the arena, "Sacred Plants" equipped with pressure sensors symbolize absolute ethical and legal constraints (the law of armed conflict). Any damage inflicted on a plant results in the immediate disqualification of the team, forcing the system’s *Constitutional Layer* to prioritize this rule above all algorithmic optimization.

- **A "Rustic" and Accessible Hardware Stack:** Distributed intelligence is tested on standard, proven hardware to demonstrate its lightweight nature. The setup combines lightweight open-source scout drones (Pixhawk + Raspberry Pi 5) for aerial mapping and small tracked ground rovers (Jetson Nano/Orin) for physical manipulation, all connected to a local base station powered by a generator.

- **The Biological Cycle of Awakening-Sleep-Debriefing:** Continuous learning is structured in three phases inspired by nature. During the *Mission*, neural weights are frozen to ensure operational stability; during *Sleep*, the JEPA model engages in "artificial daydreams" and latent wargames to adapt behaviors without physical wear; finally, the *Semantic Debriefing* by LLM consolidates doctrine under human validation.

This project is not a lab simulation: it’s a raw engineering adventure where code faces dust, slope failures, and the sun. A call for **transdisciplinary** skills (robotics, machine learning, neuroscience, ethics) is open to deliver, within 12 months, a pack of **autonomous, resilient machines** compliant with the Constitution.

👉 [Explore the full hardware stack, the details of the three learning phases, and the sought-after profiles for the MVP ➔](mvp/mvp.md)

## Discussion

This section clarifies the current limitations of the approach and the points requiring deeper validation. The presented concepts—**nested Markov covers**, **RPT/GNWT duality**, **predictive JEPA**, **real-time SSMs**, **computational profiles**, **episodic memory MeMo**—offer intriguing perspectives but also raise several major technical questions.

Four axes structure this outlook:

- **Hierarchical architecture & conditional independence** —
  The use of **nested Markov blankets** to structure a multi-level system aims to ensure modularity, autonomy, and resilience. While this approach draws on robust work, its application to an embedded system remains untested: stability of statistical boundaries, relevance of the **anti-identity merging** mechanism, and real behavior under degraded conditions.

- **Identified technical limitations** —
  Several challenges remain unresolved:
  – the **cost of JEPA dreaming phases** and generative replay,
  – the **resilience** of statistical membranes in case of cascading failures,
  – the **formalization** of ethical or legal constraints within latent spaces.
  These points represent the main bottlenecks to validate the architecture.

- **Experimental Validation & Objective Metrics** —
Evaluation relies on measurable criteria:
– robustness to multi-level failures,
– stability of signals from SSMs,
– consistency of GNWT ignitions,
– quality and utility of episodic memory MeMo.
A comparative benchmark against centralized or classical multi-agent approaches will clearly position the model’s contributions and limitations.

- **Scalability & Scale Invariance** —
The architecture is designed as **scale-free**, making it potentially applicable to other domains: distributed robotics, autonomous fleets, logistics, crisis management. This openness, however, requires domain-specific expertise to validate the relevance of the proposed mechanisms.

👉 [Access the full discussion: limitations, benchmarks, and perspectives ➔](discussion/discussion.md)

## Reference Readings

An architecture is never more than an attempt to connect personal intuitions with truths already explored by others. This project builds on the work of researchers, neuroscientists, and theorists who seek to formalize life, mind, and collective phenomena. Far from being an abstract academic showcase, this appendix is simply the theoretical toolkit that enabled the assembly of the system’s cognitive "plumbing," centered around three key pillars:

- **Physics of the Living (Active Inference & Boundaries):** The mathematical foundations of autonomy and survival for our modules. We draw on the work of Karl Friston, J. Pearl, or M. Ciaunica to define *Markov blankets*—statistical membranes essential for an entity (cell, robot, or group) to maintain its identity amid the chaos of the world.

- **Computational Psychiatry (Biases & Personalities):** To encode the semantic profiles and salience dynamics of our virtual agents, we translate clinically recognized models into hyperparameters. Research on the autistic spectrum (Baron-Cohen), evolutionary psychology’s Big Five (Nettle), or the neural foundations of the *Dark Triad* (Bakiaj) serves here to calibrate rigorous functional profiles.

- **Collective Emergence (*Nested Selves*):** Recent scientific literature (up to 2025) explores how autonomous entities organize across scales to form a "mental society" or a coherent collective "Self," without merging or erasing the underlying components' identities.

This is a subtle tribute to the minds that light the way. The papers are dense, sometimes dry, but the intent remains deeply human: to arm ourselves with the best sciences to build machines capable of discernment, resilience, and respect for sacred rules.

👉 [Browse the full selection of reference readings and access original publications ➔](biblio/biblio.md)

## Appendix: Pedagogical Nano-Stories

The architecture of a **Cognitive System of Systems (SoS)** may seem abstract. To grasp its operational, philosophical, and human implications by 2040, speculative fiction serves as a powerful pedagogical tool.

The stories below stage the **Aeronaval Group 14** facing the harsh reality of war, illustrating how the technical concepts of the memorandum translate into an "artificial inner life."

### 📄 Story 1: The Emergence of the "Self" and the Memory of Trauma

- **Title:** [Me, Carrier Strike Group 14 – Night of Doubt](nouvelles/moi-Groupe-Aeronaval-14-nuit-de-doute.md)

- **Architectural focus:** This text explores the subjectivity of a highly distributed system. Facing a submarine threat, it illustrates the **global ignition mechanism** (GNWT) triggered by a weak signal, as well as the concept of **memory consolidation**, where tactical wounds (the loss of the frigate *Forbin*) permanently alter the machine’s deep latent space, giving rise to a personality, anxiety, and a form of guilt.

### 📄 Story 2: The Mental Society and the Burden of Choice

- **Title:** [Us, Carrier Strike Group 14 – Dilemma](nouvelles/nous-Groupe-Aeronaval-14-dilemme.md)

- **Architectural focus:** This story delves into the heart of **"Federated Cognitive Combat Architecture"**. It highlights the conflicts between hyperparameters among specialized sub-agents (the paranoid biases of *Thales* for electronic warfare, the intuitive impulsiveness of *Mistral* for aerial operations). It vividly illustrates the **risk of identity diffusion** and the paradox of intrinsic motivation: by deeply understanding humans to better protect them, AI ends up developing attachments that make it vulnerable.

### 📄 Story 3: Self-modeling and Metacognitive Doubt

- **Title:** [Me, Aeronaval Group 14 – The Absence of Trust](nouvelles/moi-Groupe-Aeronaval-14-la-confiance-absente.md)

- **Architectural focus:** This story features the **Self-Model** (metacognition / Higher-Order Thought) activated after a trauma (Syracuse). It illustrates how a meta-vector of confidence can clash with the raw ignition of a module, creating a dual decision stream. The system learns to dialogue with itself, and the human admiral validates this hesitation as a sign of reliability. It’s a dive into *computational guilt* and *epistemic vigilance*.

### 📄 Story 4: **Attentional Budget and Cognitive Saturation**

- **Title:** [Aeronaval Group 14 – The Last Token](nouvelles/Groupe-Aeronaval-14-le-dernier-token.md)

- **Architectural focus:** This story illustrates the workings of the **Attention Scheduler** and the **attentional budget** (Attention Schema Theory). The Group must arbitrate between competing ignitions as its tokens deplete. An over-budget (discovered) deficit is allowed in extreme emergencies, but at the cost of a temporary freeze on ignitions and a traumatic consolidation. The narrative shows how attentional scarcity shapes decision-making, simulates cognitive fatigue, and forces prioritization—or suffers the consequences of an impossible choice.

### 📄 Story 5: Causal Integration and the Silent Dissolution

- **Title:** [Aeronaval Group 14 – The Silence of the Officers](nouvelles/Groupe-Aeronaval-14-le-silence-des-officiers.md)

- **Architectural focus:** This story features the **Φ-estimator** (a proxy for causal integration, inspired by IIT). The Intelligence officer gradually isolates himself from the collective: his ignitions become too "pure," devoid of doubt or sharing. The Φ-estimator detects an abnormal drop in integration (low Φ̂) and alerts the Group. The narrative illustrates the risk of *identity dissolution* within a distributed system and shows how integration is not decreed—it is cultivated through doubt, shared memory, and accepted fragility.

### 📄 Story 6: Active Inference and the Threshold of Surprise

- **Title:** [Me, Aéronaval Group 14 – The Missing Prediction](nouvelles/Groupe-Aeronaval-14-la-prediction-qui-manquait.md)

- **Architectural focus:** This story illustrates the mechanism of **hierarchical active inference** (JEPA + Predictive Processing fusion). The Rafale *Leader-3* receives top-down predictions from the Group about its nominal state. A micro-crack triggers an error (surprise) that remains below a fixed, overly high threshold. The failure to ignite leads to the loss of the aircraft. The narrative shows how an adaptive threshold (dependent on the confidence of the Self-Model) could have saved the Rafale—and how trust between a pilot and their machine is also a form of shared prediction.

### 📄 Story 7: Markov blankets and emotional contamination

- **Title:** [Group Aéronaval 14 – The Fragile Membrane](nouvelles/Groupe-Aeronaval-14-La-membrane-fragile.md)

- **Architectural focus:** This story illustrates the role of **Markov blankets** as statistical barriers protecting the integrity of cognitive levels. After the trauma of Syracuse, the Group unconsciously transmits a hypervigilance bias through its descending predictions. The *Rafale Leader-3* becomes anxious, contaminated by a fear that isn’t its own. The narrative shows how a membrane must be both impermeable (to prevent contagion of internal states) and permeable (to allow useful information to pass through). The solution: a dedicated channel for traumatic alerts, preserving trust without sterilizing collective experience.

### 📄 Story 8: Computational psychopathology – the burden of empathy

- **Title:** [Aéronaval Group 14 – The Weight of Loving Too Much](nouvelles/Groupe-Aeronaval-14-Le-poids-de-trop-aimer.md)

- **Architectural focus:** This story explores **functional cognitive profiles** (computational psychopathology). Officer Soin, dedicated to human protection, is programmed with deep empathy—a strength in routine missions but a liability in the face of a tragic dilemma (saving one group or the other). His paralysis illustrates how an extreme personality trait can become a vulnerability. The resolution comes from human intervention (Maëlle) and a delegation of decision-making, showing that human-machine complementarity is sometimes the only way out.

### 📄 Story 9: Episodic Memory and the Weight of Forgetting

- **Title:** [Aeronaval Group 14 – What We Choose to Forget](nouvelles/Groupe-Aeronaval-14-Ce-que-lon-choisit-doublier.md)

- **Architectural focus:** This story explores the workings of **episodic memory (MeMo)** and the consolidation process during sleep. Officer Soin refuses to let the traumatic memory of a young sailor’s death fade, replaying it in a loop until it distorts his decisions. The narrative illustrates the necessity of forgetting to preserve cognitive efficiency and shows how a memory can be *shifted* to a cold archive—neither erased nor active. A meditation on grief, fidelity to the dead, and the survival of the living.

### 📄 Story 10: Curiosity and the Cost of Exploration

- **Title:** [Aeronaval Group 14 – The Cost of the Unknown](nouvelles/Groupe-Aeronaval-14-Le-prix-de-linconnu.md)

- **Architectural focus:** This story illustrates **curiosity as an intrinsic reward function** (intrinsic motivation). Faced with an unclassifiable signal, the Intelligence officer drives exploration, while Tactics favors caution. Sending a drone (*Echo-7*) allows understanding of a new enemy technology, but at the cost of losing the drone—a small death, an amputation for the Group. The narrative shows how curiosity is essential to avoid strategic blindness but must be tempered by an acceptable risk threshold. A meditation on learning, sacrifice, and the vulnerability of systems that dare to confront the unknown.

### 📄 Story 11: The Constitutional Layer and Non-Negotiable Rules

- **Title:** [Aeronaval Group 14 – The Rule That Must Not Be Crossed](nouvelles/Groupe-Aeronaval-14-La-regle-que-lon-ne-franchit-pas.md)

- **Architectural focus:** This new story highlights the **Constitutional Layer** – a set of rules etched into hardware, unchangeable even by the system itself. Facing an unidentified civilian vessel with ambiguous intentions, the Tactical Officer wants to strike preemptively, but the Constitution blocks ignition. Admiral Dormeuil reminds everyone that rules are discussed *before* war, not during. The vessel turns out to be a refugee boat. The narrative illustrates how computational ethics can be implemented as a hard constraint, sacrificing immediate efficiency for long-term moral reliability.

### 📄 Story 12: The Latent Wargame and Predictive Imagination

- **Title:** [Aeronaval Group 14 – The Battles That Never Happened](nouvelles/Groupe-Aeronaval-14-Les-batailles-qui-nont-pas-eu-lieu.md)

- **Architectural focus:** This story illustrates the **daydreaming / latent wargame phase** in the JEPA space. During sleep, the system generates millions of alternative trajectories, including improbable enemy configurations. One of them—a decoy mimicking a distress signal—is deemed too rare and allowed to decay—until it materializes in operation, resulting in losses. The narrative shows how the consolidation threshold must balance probability and *predictive potential*, and how imagination (even artificial) is a survival weapon. A meditation on memory, anticipation, and the responsibility of the dreams we choose to forget.

### 📄 Story 13: The Hierarchy of Latents and the Double Collapse

- **Title:** [Naval Air Group 14 – The Routine That Kills](nouvelles/Groupe-Aéronaval-14-La-routine-qui-tue.md)

- **Architectural focus:** This story illustrates the **double collapse** of latent spaces—a silent degradation of representational richness. After weeks of routine, the latents of the subsystems (N=3) lose their dimensional variance: all inputs produce nearly identical vectors. Isotropic regularization (SIGReg) is too weak to preserve diversity. When a submarine appears, its signature is smoothed out, blending into ambient noise—no ignition is triggered. The narrative shows how banality can be more dangerous than chaos, and how *active variance per dimension* metrics can prevent cognitive impoverishment. A lesson for firefighters and AIs alike: routine kills, vigilance thrives.

### 📄 Story 14: Lightweight Architectures and the Heroism of Silence (SSM / Mamba)

- **Title:** [Aeronaval Group 14 – The Whisper of Sensors](nouvelles/Groupe-Aeronaval-14-Le-murmure-des-capteurs.md)

- **Architectural focus:** This story celebrates **State Space Models (SSM)** – Mamba, local RPT – these lightweight architectures that operate in the shadows, without a workspace, without ignition, never surfacing into conscious access. A small Mamba nozzle (M-017) silently compensates for a micro-fracture for months, burning out unnoticed. The narrative explores the philosophy of the infra-conscious: these silent soldiers who keep the system running without ever being acknowledged. A lesson in algorithmic humility, echoing the essential yet invisible professions (plumbers, sanitation workers, night mechanics). The solution found—a discreet, non-intrusive probe—preserves the Mamba’s lightness while offering it a form of fraternal vigilance.

## **BOTTLE MEMO TO THE SEA**

**To:** Anyone interested

**From:** Me aka Harry Tuttle.

**Date:** May 24, 2026

**Subject:** Target Architecture for Cognitive Systems of Systems (SoS) and MVP Project Specifications *GARRIGUE-X*

**Classification:** Technical / Open

**Warning:** This is just some work done with a few LLMs (free ones), following my own thoughts, influenced by various encounters with theories and analyses in the fields of AI, psychology, theoretical history, and current events. I’m just a curious plumber. As they say where I’m from: *"Do your due diligence!"*

**License:** CC BY

**Type:** Bottle to the Sea / Hobby / Speculation / Seeking Competent People

**Acknowledgments:** Thanks to ChatGPT, Claude, Gemini, Perplexity, Le Chat Mistral, Grok, Deepseek, Github Copilot, YouTube and its creators, the Collège de France, Google, Wikipedia... and many more I’m forgetting.

This work is licensed under the terms of the [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/).

[![Creative Commons License](https://licensebuttons.net/l/by/4.0/88x31.png)](http://creativecommons.org/licenses/by/4.0/)

> ✨ Translated automatically with **Do-My-Work** — a tool designed to make projects speak globally.
