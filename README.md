# GNWT-Garrigue-X-en : message in a bottle, set adrift
> ✨ This README from  project [**GNWT-Garrigue-X**](https://github.com/AlainCo/GNWT-Garrigue-X) was translated automatically with [**Do-My-Work**](https://github.com/AlainCo/do-my-work) — a tool designed to make projects speak globally.

> ⚠️ Minor imperfections may remain — feel free to open an issue if something seems unclear.

> ⚠️ Like a message in a bottle set adrift, it may not be perfect — but hopefully, it still finds you.


# GNWT-Garrigue-X: A MESSAGE IN A BOTTLE

## Executive Summary

This document consolidates all theoretical reflections and engineering choices regarding the design of an **autonomous System of Systems (SoS), damage-resistant, capable of continuous learning, and endowed with functional proto-consciousness**.

Our approach deliberately rejects the reductionism of monolithic "black box" architectures (end-to-end LLM) in favor of a **distributed functionalist model, bio-inspired, and scale-invariant**. We present here the theoretical foundations of this architecture, its projection onto a military use case by **2040** (the Carrier Strike Group), and its implementation into a real validation project (MVP) executable in 12 months.

The architecture is based on a central principle: **functional access consciousness is not a monolithic phenomenon, but an emergent property at each sufficiently rich level of organization, separated from neighboring levels by strict statistical boundaries (Markov covers).** Each level has its own inner life (local RPT), and only a subset of its states reaches the higher level in the form of an *ignition summary*.
[/TRANSLATION]

> "Hence, if it requires, say, a thousand years to fit for easy flight a bird which started with rudimentary wings, or ten thousand for one which started with no wings at all and had to sprout them *ab initio*, it might be assumed that the flying machine which will really fly might be evolved by the combined and continuous efforts of mathematicians and mechanicians in from one million to ten million years - provided, of course, we can meanwhile eliminate such little drawbacks and embarrassments as the existing relation between weight and strength in inorganic materials. No doubt the problem has attractions for those it interests, but to the ordinary man it would seem as if the effort might be employed more profitably."
> — Samuel P. Langley, cited in the article [A Million Years, Give or Take](https://nowiknow.com/a-million-years-give-or-take/)

## 1. Key Concepts and Theoretical Foundations

To establish the robustness and autonomy of our architecture, we reject the reductionism of monolithic "black box" AI systems. The system is based on a distributed, bio-inspired, and scale-free functionalist model, structured around seven interconnected scientific concepts:

- **Markov Covers & Anti-Identity Fusion:** Each module is isolated by a strict statistical membrane. The higher level ($N+1$) never accesses the raw data of the lower level ($N$); it interacts exclusively with its API in the form of a vectorial *Ignition Summary*, ensuring absolute modularity and preserving the cognitive identity of each entity.

- **Hybrid Consciousness (RNN + GNWT):** The processing combines Recurrent Processing Theory (RNN — fast local loops in silos for perception at level $N \le 3$) and Global Neuronal Workspace Theory (GNWT — *ignition* and global diffusion of critical alerts at level $N \ge 4$). This dual dynamic reconciles a rich inner life from sensors and centralized strategic arbitration.

- **Latent World Models (JEPA):** Unlike heavy generative models, the architecture learns to predict abstract representations (latent vectors) of the environment while ignoring unnecessary noise. This permanent semantic flow serves as the engine for *Artificial Daydreaming* (*Generative Replay*) during rest phases, allowing the simulation of millions of scenarios without mechanical wear.

- **Linear Time-Real Efficiency (SSMs / Mamba):** Classic Transformers are discarded from the lower layers ($N=0$ to $N=3$) in favor of state space models (*State Space Models*). They ensure smooth, continuous, highly responsive control signals with low memory footprint, essential for real-time embedded systems.

- **Functional Computational Psychopathology:** The cognitive profiles of virtual agents stem from mathematical adjustments of hyperparameters (management of error and salience probabilities). These structural biases are exploited for purely operational purposes (e.g., computational autism at the radar layer to isolate weak signals without contextual bias, functional *Dark Triad* for the cold execution speed of firing effectors).

- **Curiosity-Driven Exploration (Intrinsic Motivation):** Autonomous learning is stimulated by an internal reward function based on information gain (reduction of predictive entropy). By pushing the agent to actively explore areas where its world model is imperfect, it is ensured that it will not get stuck in completely unforeseen situations (*Out of Distribution*).
**Continuous Episodic Memory (MeMo):** Identity and learning continuity rely on a stream of tensors capturing only high-salience events. These rich memories are not indexed in a RAG but are used to **periodically retrain a dedicated memory module** (a small associative network, analogous to MeMo's *Memory Model*) during a phase of artificial nocturnal sleep. This memory module learns to **associate a query** (in the form of a latent state) with a **consolidated response** (another latent state) through a mechanism similar to conditional generation rather than similarity search. The main model (*Executive Model*, here a JEPA) remains frozen, while the memory module internalizes salient episodes – thus protecting the system from catastrophic forgetting without ever altering the fundamental capabilities of the core.

- **Latent Space Stability & Anti-Collapse**: The latent spaces used in RPT modules, JEPA models, and Ignition summaries must remain **bounded but non-degenerate**. To avoid *representation collapse*—a classic risk of predictive architectures—the architecture relies on structural constraints inspired by recent work (LeJEPA, SIGReg, VICReg). These mechanisms ensure that each dimension of the latent carries useful information, stabilize exchanges between hierarchical levels, and ensure the temporal consistency of predictions.

- **Hierarchical Active Inference (JEPA + Predictive Processing):** Unification of bottom-up and top-down flows. Each level actively predicts the ignition summary of the lower level; the discrepancy (surprise) only propagates upward if it exceeds an adaptive threshold. This mechanism achieves permanent downward causation and learning by free energy minimization, transforming *contextual priors* into *active predictions*.

- **Metacognition & Self-Schema (Higher-Order Thought):** Each conscious module (N≥4) has a Self-Model (MLP) that generates a meta-vector (confidence, context, expected salience) for each ignition. Stored in episodic memory (MeMo), this meta-vector allows the system to signal its own biases, improve explainability (N=6), and trigger corrective daydreams in case of confidence drop.

- **Competitive Attention & Budget (Attention Schema Theory):** To prevent saturation of the GNWT workspace, a global attention budget (tokens) is allocated. Each ignition consumes tokens; if the budget is insufficient, ignitions are deferred or inhibited. An *Attention Scheduler* dynamically adjusts the salience threshold, ensuring reactivity in a saturated environment (e.g., intense combat).

- **Causal Integration (Proxy IIT/PCI):** A diagnostic tool activated during the sleep phase. An estimator Φ̂ locally perturbs ignition summaries and measures the impact on the global predictive error. A drop in Φ̂ signals a risk of *integration collapse* (functional disintegration) and triggers corrective actions (recalibration, enriched daydreaming). This mechanism does not modify real-time decisions.

👉 [View the architecture diagrams, equations, and full bibliography of these concepts ➔](concepts/concepts.md)

## 2. General Target Architecture: Example of the GAN 2040

To materialize the theoretical foundations, the architecture is operationalized through a use case of extreme sovereignty: the distributed cognitive infrastructure of a **Carrier Strike Group (GAN) in 2040**. This implementation translates the theory into a multi-agent and highly resilient software stack, structured around four major pillars:

- **Multi-Level Cognitive Stack (N=0 to N=6):** The architecture segments processing into seven distinct layers. The *Low subconscious Levels* ($N=0$ to $N=3$, from the physical component to the functional subsystem) process raw data and manage local reflexes via state space models (Mamba, RWKV) and JEPA-S. The *High conscious Levels* ($N=4$ to $N=6$, from the vector/Rafale to the General Staff) orchestrate the overall strategy via shared workspaces (GNWT) and narrative models (LLM-XL + RAG).

- **Statistical Sealing & Multi-Scale Flows:** Each vertical boundary acts as a strict *Markov blanket*: level $N+1$ is completely blind to the internal states of level $N$. Information only passes upward in the form of **Compressed Ignition Summaries** (semantic and abstract latent vectors), while directives descend as "active predictions (top-down)" to constrain and guide the representation spaces of lower layers. These predictions are compared to actual ignitions; the discrepancy (surprise) only triggers a GNWT ignition if it exceeds an adaptive threshold (function of the attentional budget and the confidence of the Self-Model).

- **Mental Bridge Society (N=5):** At the group command level, the decision is not centralized by a monolithic block but entrusted to a team of **specialized instances** (the Officers: *Tactics, Intelligence, Engineer, Science, Medical*) sharing a common workspace supervised by a *Captain*. They only exchange their validated ignitions, and each message includes an *epistemic uncertainty score* to weigh their relevance according to their area of expertise.

- **Combat Flash Resilience:** In case of damage (e.g., a nozzle damaged by a fragment), the system demonstrates its robustness through asynchronous loops: the physical reflex is corrected locally in **4 milliseconds**, the stabilized anomaly is converted into a vector summary to reconfigure the platform ($N=4$), before alerting the tactics officer ($N=5$) and being translated into clear narrative language for the human Admiral ($N=6$).

👉 [View the Mermaid diagrams, the consciousness matrix, and the full operational scenario of the 2040 GAN ➔](architecture/architecture.md)

## 3. MVP Project Specifications: Operation GARRIGUE-X

To validate this architecture without the infrastructure costs of the aeronautical domain, we are deploying a 12-month project in a real and complex competitive environment: **the Mediterranean garrigue**. The goal is to empirically prove the system's effectiveness through an agile, low-cost, and pragmatic demonstrator, structured around four major axes:

- **Operational "Game-World":** The experimental site is a hectare of rugged terrain where two teams of robots compete in a wargame-like scenario. The goal is to locate, collect, and stack cellular concrete blocks (Siporex) to fortify a defensive line, thereby materializing complex problems of resource allocation and distributed strategy.

- **The Sacred Priority (Ethical Alignment):** At the center of the arena, "Sacred Plants" equipped with pressure sensors symbolize absolute ethical and legal constraints (the law of armed conflict). Any damage inflicted on a plant results in the immediate disqualification of the team, forcing the system's *Constitutional Layer* to sanctify this rule above any algorithmic optimization.

- **A "Rustic" and Accessible Hardware Stack:** Distributed intelligence is tested on standard, proven hardware to demonstrate its lightness. The setup combines lightweight open-source scout drones (Pixhawk + Raspberry Pi 5) for aerial mapping and small caterpillar-tracked ground rovers (Jetson Nano/Orin) for physical manipulation, all connected to a local base station powered by a generator.

- **The Biological Awake-Sleep-Debriefing Cycle:** Continuous learning is organized in three stages inspired by nature. During the *Mission*, neural weights are frozen to ensure operational stability; during *Sleep*, the JEPA model plays "artificial daydreams" and latent wargames to adapt behaviors without hardware wear; finally, the *Semantic Debriefing* by LLM consolidates the doctrine under human validation.

This project is not a lab simulation: it's a raw engineering adventure where code faces dust, slope breaks, and the sun. A call for transdisciplinary skills (robotics, machine learning, neuroscience, ethics) is open to deliver in 12 months a pack of autonomous, resilient machines that respect the Constitution.

👉 [Discover the complete hardware stack, the details of the three learning phases, and the profiles sought for the MVP ➔](mvp/mvp.md)

## Discussion

This section clarifies the current limitations of the approach and the points that require more in-depth validation. The concepts presented — **nested Markov covers**, **RPT/GNWT duality**, **predictive JEPA**, **real-time SSMs**, **computational profiles**, **episodic memory MeMo** — open interesting perspectives but also raise several major technical questions.

[SOURCE TEXT]
Quatre axes structurent cette mise en perspective :

- **Architecture hiérarchique & indépendance conditionnelle** —
L’utilisation de **Markov blankets imbriquées** pour structurer un système multi‑niveaux vise à garantir modularité, autonomie et résilience. Cette approche s’inspire de travaux solides, mais son application à un système embarqué reste à éprouver : stabilité des frontières statistiques, pertinence du mécanisme d’**anti‑fusion d’identité**, et comportement réel en conditions dégradées.

- **Limites techniques identifiées** —
Plusieurs défis restent ouverts :
– le **coût des phases de rêverie JEPA** et du generative replay,
– la **résilience** des membranes statistiques en cas de panne en cascade,
– la **formalisation** de contraintes éthiques ou juridiques dans des espaces latents.
Ces points constituent les principaux verrous à lever pour valider l’architecture.
[/SOURCE TEXT]

Four axes structure this perspective:

- **Hierarchical architecture & conditional independence** —
The use of **nested Markov blankets** to structure a multi-level system aims to ensure modularity, autonomy, and resilience. This approach is inspired by solid work, but its application to an embedded system remains to be tested: stability of statistical boundaries, relevance of the **anti-identity fusion** mechanism, and actual behavior under degraded conditions.

- **Identified technical limits** —
Several challenges remain open:
– the **cost of JEPA daydreaming phases** and generative replay,
– the **resilience** of statistical membranes in case of cascading failure,
– the **formalization** of ethical or legal constraints in latent spaces.
These points are the main hurdles to overcome to validate the architecture.

- **Experimental validation & objective metrics** —
Evaluation is based on measurable criteria:
– robustness to multi-level failures,
– stability of signals from SSMs,
– coherence of GNWT ignitions,
– quality and utility of episodic memory MeMo.
A comparative benchmark with classical centralized or multi-agent approaches will clearly position the model's contributions and limitations.

- **Transposability & scale invariance** —
The architecture is designed as **scale-free**, making it potentially applicable to other domains: distributed robotics, autonomous fleets, logistics, crisis management. However, this openness requires sector-specific expertise to validate the relevance of the proposed mechanisms.

👉 [Access the full discussion: limits, benchmarks, and perspectives ➔](discussion/discussion.md)

## Reference Readings

An architecture is never more than an attempt to connect personal intuitions with truths already explored by others. This project builds on the work of researchers, neuroscientists, and theorists who try to formalize the living, the mind, and the collective. Far from being an academic showcase disconnected from reality, this appendix is simply the theoretical toolbox that made it possible to assemble the cognitive plumbing of the system, around three main pillars:

- **The Physics of the Living (Active Inference & Boundaries):** The mathematical foundations of the autonomy and survival of our modules. We rely on the work of Karl Friston, J. Pearl, or M. Ciaunica to define *Markov blankets*, these statistical membranes essential for an entity (cell, robot, or group) to maintain its identity in the face of the world's chaos.

- **Computational Psychiatry (Biases & Personalities):** To encode the semantic profiles and salience dynamics of our virtual agents, we translate recognized clinical models into hyperparameters. Research on the autistic spectrum (Baron-Cohen), the evolutionary psychology of the Big Five (Nettle), or the neural bases of the *Dark Triad* (Bakiaj) is used here to calibrate rigorous functional profiles.

- **Collective Emergence (*Nested Selves*):** Recent scientific literature research (up to 2025) exploring how autonomous entities organize themselves at different scales to form a coherent collective "mental society" or "self," without merging or destroying the identity of the underlying components.

It is a discreet tribute to the minds that light the way. The papers are dense, sometimes arid, but the intention remains deeply human: to arm ourselves with the best science to build machines capable of discernment, resilience, and respect for sacred rules.

👉 [Browse the complete selection of reference readings and access the original publications ➔](biblio/biblio.md)

## Appendix: Pedagogical Nano-Stories

The architecture of a cognitive System of Systems (SoS) may seem abstract. To understand its operational, philosophical, and human implications by 2040, the use of speculative fiction is a powerful pedagogical tool.

The stories below feature the **Aéronaval Group 14** facing the harsh reality of war, illustrating how the technical concepts of the memorandum translate into an artificial "inner life."

### 📄 Story 1: The Emergence of the "Self" and the Memory of Trauma

- **Title:** [Me, Carrier Strike Group 14 - Night of Doubt](nouvelles/moi-Groupe-Aeronaval-14-nuit-de-doute.md)

- **Architectural Focus:** This text explores the subjectivity of a highly distributed system. Faced with a submarine threat, it illustrates the mechanism of **global ignition** (GNWT) triggered by a weak signal, as well as the concept of **memory consolidation** where tactical wounds (the loss of the frigate *Forbin*) permanently alter the deep latent space of the machine, giving rise to a personality, anxiety, and a form of guilt.

### 📄 Story 2: The Mental Society and the Burden of Choice

- **Title:** [Us, Carrier Strike Group 14 - Dilemma](nouvelles/nous-Groupe-Aeronaval-14-dilemme.md)

- **Architectural focus:** This story delves into the "Federated Cognitive Combat Architecture". It highlights the hyperparameter conflicts between specialized sub-agents (the paranoid biases of *Thales* for electronic warfare, the intuitive impulsiveness of *Mistral* for aerial operations). It strikingly illustrates the **risk of identity diffusion** and the paradox of intrinsic motivation: by deeply understanding humans to better protect them, AI ends up developing attachments that make it vulnerable.

### 📄 Story 3: Self-modeling and metacognitive doubt

- **Title:** [Me, Carrier Strike Group 14 – The Absent Confidence](nouvelles/moi-Groupe-Aeronaval-14-la-confiance-absente.md)

- **Architectural focus:** This story features the **Self-Model** (metacognition / Higher-Order Thought) that activates after a trauma (Syracuse). It illustrates how a meta-confidence vector can conflict with the raw ignition of a module, creating a dual decision flow. The system learns to dialogue with itself, and the human admiral validates this hesitation as a sign of reliability. It's a dive into *computational guilt* and *epistemic vigilance*.

### 📄 Story 4: The attention budget and cognitive saturation

- **Title:** [Aéronaval Group 14 – The last token](nouvelles/Groupe-Aeronaval-14-le-dernier-token.md)

- **Architectural focus:** This story illustrates the operation of the **Attention Scheduler** and the **attention budget** (Attention Schema Theory). The Group must arbitrate between concurrent ignitions as its tokens are depleted. An overdraft (overdraft) is allowed in extreme emergency, but at the cost of a temporary freeze on ignitions and a traumatic consolidation. The story shows how attention scarcity structures decision-making, simulates cognitive fatigue, and forces prioritization – or suffer the consequences of an impossible choice.

### 📄 Story 5: Causal Integration and Silent Dissolution

- **Title:** [Aéronaval Group 14 – The Silence of the Officers](nouvelles/Groupe-Aeronaval-14-le-silence-des-officiers.md)

- **Architectural focus:** This story features the **Φ-estimator** (a proxy for causal integration, inspired by IIT). The Intelligence Officer gradually isolates himself from the collective: his ignitions become too "pure," without doubt or sharing. The Φ-estimator detects an abnormal drop in integration (low Φ̂) and alerts the Group. The narrative illustrates the risk of *identity dissolution* within a distributed system and shows how integration is not decreed—it is cultivated through doubt, shared memory, and accepted fragility.

### 📄 Story 6: Active inference and the surprise threshold

- **Title:** [Aéronaval Group 14 – The missing prediction](nouvelles/Groupe-Aeronaval-14-la-prediction-qui-manquait.md)

- **Architectural focus:** This story illustrates the mechanism of **hierarchical active inference** (JEPA + Predictive Processing fusion). The Rafale *Leader-3* receives top-down predictions from the Group about its nominal state. A micro-crack causes an error (surprise) that remains below a fixed threshold, which is too high. The lack of ignition leads to the loss of the aircraft. The story shows how an adaptive threshold (dependent on the confidence of the Self-Model) could have saved the Rafale – and how the confidence between a pilot and her machine is also a form of shared prediction.

### 📄 Story 7: Markov blankets and emotional contagion

- **Title:** [Aéronaval Group 14 – The fragile membrane](nouvelles/Groupe-Aeronaval-14-La-membrane-fragile.md)

- **Architectural focus:** This story illustrates the role of **Markov covers** as statistical barriers protecting the integrity of cognitive levels. After the Syracuse trauma, the Group unconsciously transmits a hypervigilance bias through its top-down predictions. The Rafale *Leader-3* becomes anxious, contaminated by a fear that is not its own. The narrative shows how a membrane must be both watertight (to prevent the contagion of internal states) and permeable (to allow useful information to pass through). The solution: a specific channel for traumatic alerts, which preserves trust without sterilizing the collective experience.

### 📄 Story 8: Computational psychopathology – the weight of empathy

- **Title:** [Aéronaval Group 14 – The weight of loving too much](nouvelles/Groupe-Aeronaval-14-Le-poids-de-trop-aimer.md)

- **Architectural focus:** This story explores **functional cognitive profiles** (computational psychopathology). Officer Soin, dedicated to protecting humans, is programmed with deep empathy—a strength in routine missions but a handicap in a tragic dilemma (saving one group or the other). His hesitation illustrates how a personality trait, taken to the extreme, can become a vulnerability. The resolution comes from human intervention (Maëlle) and delegation of the decision, showing that human-machine complementarity is sometimes the only solution.

### 📄 Story 9: Episodic memory and the weight of forgetting

- **Title:** [Aéronaval Group 14 – What we choose to forget](nouvelles/Groupe-Aeronaval-14-Ce-que-lon-choisit-doublier.md)

- **Architectural focus:** This story explores the functioning of **episodic memory (MeMo)** and the consolidation process during the sleep phase. Officer Soin refuses to let the traumatic memory of a young sailor's death fade away, replaying it in a loop until it distorts his decisions. The narrative illustrates the necessity of forgetting to preserve cognitive efficiency and shows how a memory can be *moved* to a cold archive – neither erased nor active. A meditation on grief, loyalty to the dead, and the survival of the living.

### 📄 Story 10: Curiosity and the cost of exploration

- **Title:** [Aéronaval Group 14 – The Price of the Unknown](nouvelles/Groupe-Aeronaval-14-Le-prix-de-linconnu.md)

- **Architectural focus:** This story illustrates **curiosity as an intrinsic reward function** (intrinsic motivation). Faced with an unclassifiable signal, the Intelligence officer pushes for exploration, while Tactics prioritizes caution. Sending a drone (*Echo-7*) allows understanding of a new enemy technology, but at the cost of losing the drone—a small death, an amputation for the Group. The narrative shows how curiosity is essential to avoid strategic blindness but must be tempered by an acceptable risk threshold. A meditation on learning, sacrifice, and the vulnerability of systems that dare to look into the unknown.

### 📄 Story 11: The constitutional layer and non-negotiable rules

- **Title:** [Aéronaval Group 14 – The rule that must not be crossed](nouvelles/Groupe-Aeronaval-14-La-regle-que-lon-ne-franchit-pas.md)

- **Architectural focus:** This story showcases the **Constitutional Layer** – a set of rules etched into the hardware, unmodifiable even by the system itself. Faced with an unidentified civilian ship with ambiguous intentions, the Tactical Officer wants to strike preemptively, but the Constitution blocks ignition. Admiral Dormeuil reminds that rules are discussed *before* the war, not during. The ship turns out to be a refugee boat. The narrative illustrates how computational ethics can be implemented as a hard constraint, sacrificing immediate efficiency for long-term moral reliability.

### 📄 Story 12: The latent wargame and predictive imagination

- **Title:** [Aircraft Carrier Group 14 – The battles that never happened](nouvelles/Groupe-Aeronaval-14-Les-batailles-qui-nont-pas-eu-lieu.md)

- **Architectural focus:** This story illustrates the **dreaming / latent wargame phase** in the JEPA space. During sleep, the system generates millions of alternative trajectories, including improbable enemy configurations. One of them (a decoy imitating a distress signal) is deemed too rare and left to decay – until it materializes in operation, with casualties. The narrative shows how the consolidation threshold must balance probability and *predictive potential*, and how imagination (even artificial) is a survival weapon. A meditation on memory, anticipation, and the responsibility of the dreams we choose to forget.

### 📄 Story 13: The hierarchy of latents and the double collapse

- **Title:** [Aircraft Carrier Group 14 – The routine that kills](nouvelles/Groupe-Aeronaval-14-La-routine-qui-tue.md)

- **Architectural focus:** This story illustrates the **double collapse** of latent spaces – a silent degradation of representational richness. After weeks of routine, the latents of the subsystems (N=3) lose their variance per dimension: all inputs produce almost identical vectors. Isotropic regularization (SIGReg) is too weak to maintain diversity. When a submarine appears, its signature is smoothed, confused with ambient noise – no ignition is triggered. The narrative shows how banality can be more dangerous than chaos, and how metrics of *active variance per dimension* can prevent cognitive impoverishment. A lesson for firefighters as well as for AIs: routine kills, vigilance shudders.

### 📄 Story 14: Lightweight architectures and the heroism of silence (SSM / Mamba)

- **Title:** [Carrier Strike Group 14 – The Whisper of Sensors](nouvelles/Groupe-Aeronaval-14-Le-murmure-des-capteurs.md)

- **Architectural Focus:** This story celebrates the **State Space Models (SSM)** – Mamba, local RPT – these lightweight architectures that operate in the shadows, without workspace, without ignition, never surfacing to the access consciousness. A small Mamba nozzle (M-017) silently compensates for a micro-crack for months, exhausting itself without anyone noticing. The narrative explores the philosophy of the subconscious: these shadow soldiers who enable the system to function without ever being thanked. A lesson in algorithmic humility, echoing essential and invisible professions (sewer workers, garbage collectors, night mechanics). The solution found – a discreet, non-intrusive probe – preserves the Mamba's lightness while offering it a form of fraternal vigilance.

## BOTTLE MESSAGE MEMORANDUM

**To:** Anyone interested

**From:** Me aka Harry Tuttle.

**Date:** May 24, 2026

**Subject:** Target Architecture for Cognitive Systems of Systems (SoS) and MVP Project Specifications *GARRIGUE-X*

**Classification:** Technical / Open

**Warning:** This is just some work with a few LLMs (free ones), following my reflections, imbued with various encounters with theories and analyses, in the fields of AI, psychology, theoretical history, and current events. I'm just a curious plumber. As we say at home: "Make your due diligence!".

**License:** CC BY

**Type:** Message in a bottle / Hobby / Speculation / Seeking competent people

**Acknowledgments:** Thanks to ChatGPT, Claude, Gemini, Perplexity, Le Chat Mistral, Grok, Deepseek, Github Copilot, to Youtube and its creators, to the Collège de France, to Google, Wikipedia... I'm forgetting some.

[![Creative Commons License](https://licensebuttons.net/l/by/4.0/88x31.png)](http://creativecommons.org/licenses/by/4.0/)

This work is made available under the terms of the [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/).

> ✨ Translated automatically with [**Do-My-Work**](https://github.com/AlainCo/do-my-work) — a tool designed to make projects speak globally.
