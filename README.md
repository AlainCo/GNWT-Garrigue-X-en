# GNWT-Garrigue-X-en : message in a bottle, set adrift
> ✨ This README from  project **GNWT-Garrigue-X** was translated automatically with **Do-My-Work** — a tool designed to make projects speak globally.
> ⚠️ Minor imperfections may remain — feel free to open an issue if something seems unclear.
> ⚠️ Like a message in a bottle set adrift, it may not be perfect — but hopefully, it still finds you.


```markdown
# GNWT-Garrigue-X: A BOTTLE IN THE SEA

## Executive Summary

This document consolidates all theoretical reflections and engineering choices regarding the design of an **autonomous System of Systems (SoS)**, robust to damage, capable of continuous learning, and endowed with functional proto-consciousness.

Our approach deliberately rejects the reductionism of monolithic "black-box" architectures (end-to-end LLM) in favor of a **distributed, bio-inspired, and scale-invariant functionalist model**. Here, we present the theoretical foundations of this architecture, its projection onto a military use case by **2040** (the Carrier Strike Group), and its implementation as a real validation project (MVP) executable within 12 months.
```

The architecture is based on a central principle: **functional access consciousness is not a monolithic phenomenon, but an emergent property at each sufficiently rich level of organization**, separated from neighboring levels by strict statistical boundaries (Markov covers). Each level has its own inner life (local RPT), and only a subset of its states reaches the higher level in the form of an *ignition summary*.

> "Thus, if it takes, say, a thousand years to develop a bird capable of easy flight starting from rudimentary wings, or ten thousand years for one that started with no wings at all and had to grow them *ab initio*, it might be assumed that a flying machine that will truly fly could be evolved through the combined and continuous efforts of mathematicians and mechanicians over a span of from one million to ten million years—provided, of course, we can meanwhile eliminate such minor drawbacks and inconveniences as the existing relationship between weight and strength in inorganic materials. No doubt the problem holds attractions for those it interests, but to the average person, it might seem that the effort could be better spent elsewhere."

## 1. Key Concepts and Theoretical Foundations

To establish the robustness and autonomy of our architecture, we reject the reductionism of monolithic "black-box" AI systems. The system is based on a **functionalist, bio-inspired, and scale-free** distributed model, structured around seven interconnected scientific concepts:

- **Markovian Coverings & Identity Anti-Fusion:** Each module is isolated by a strict statistical membrane. The upper level ($N+1$) never accesses raw data from the lower level ($N$); it interacts exclusively with its API in the form of a **vectorial Ignition Summary**, ensuring absolute modularity and preserving the cognitive identity of each entity.

- **Hybrid Consciousness (RPT + GNWT):** Processing integrates Recurrent Processing Theory (RPT—fast local loops in silos for perception at level *N ≤ 3*) and Global Neuronal Workspace Theory (GNWT—*ignition* and global diffusion of critical alerts at level *N ≥ 4*). This dual dynamics reconciles a rich sensor-driven inner life with centralized strategic arbitration.

- **Latent World Models (JEPA):** Unlike heavy generative models, the architecture learns to predict abstract representations (latent vectors) of the environment while ignoring irrelevant noise. This continuous semantic flow powers *Artificial Reverie* (*Generative Replay*) during rest phases, enabling the simulation of millions of scenarios without mechanical wear.

- **Linear Real-Time Efficiency (SSMs / Mamba):** Classic Transformers are excluded from the lower layers ($N=0$ to $N=3$) in favor of **State Space Models (SSMs)**. They ensure smooth, continuous, highly reactive, and low-memory-usage control signals, essential for real-time embedded systems.

- **Computational Functional Psychopathology:** The cognitive profiles of virtual agents stem from mathematical adjustments of hyperparameters (error probability and salience management). These structural biases are exploited for purely operational purposes (e.g., computational autism at the radar layer to isolate weak signals without contextual bias, *Dark Triad* functional for cold execution speed of firing effectors).

- **Exploration by Curiosity (Intrinsic Motivation):** Autonomous learning is driven by an internal reward function based on information gain (reduction of predictive entropy). By pushing the agent to actively explore areas where its world model is imperfect, we ensure it won’t get stuck in completely unforeseen situations (*Out of Distribution*).

- **Continuous Episodic Memory (MeMo):** Identity and learning continuity rely on a tensor stream capturing only high-salience events. These rich memories are consolidated in an episodic RAG during an artificial nighttime sleep phase, protecting the system from catastrophic forgetting (*catastrophic forgetting*).

- **Latent Space Stability & Anti-Collapse**: The latent spaces used in RPT modules, JEPA models, and Ignition summaries must remain **bound but non-degenerate**. To prevent *representation collapse*—a classic risk in predictive architectures—the architecture relies on structural constraints inspired by recent work (LeJEPA, SIGReg, VICReg). These mechanisms ensure that each dimension of the latent space carries meaningful information, stabilizes exchanges between hierarchical levels, and maintains temporal prediction consistency.

- **Hierarchical Active Inference (JEPA + Predictive Processing):** Unification of bottom-up and top-down flows. Each level actively predicts the ignition summary of the lower level; the discrepancy (surprise) only propagates upward if it exceeds an adaptive threshold. This mechanism achieves permanent top-down causality and learning via free-energy minimization, transforming *contextual priors* into *active predictions*.

- **Metacognition & Self-Schema (Higher-Order Thought):** Each conscious module (N≥4) has a Self-Model (MLP) that generates a meta-vector (confidence, context, expected salience) for each ignition. Stored in episodic memory (MeMo), this meta-vector enables the system to flag its own biases, improve explainability (N=6), and trigger corrective daydreams when confidence drops.

- **Competitive Attention & Budget (Attention Schema Theory):** To prevent saturation of the GNWT workspace, a global attention budget (tokens) is allocated. Each ignition consumes tokens; if the budget is insufficient, ignitions are delayed or inhibited. An *Attention Scheduler* dynamically adjusts the salience threshold, ensuring reactivity in saturated environments (e.g., intense combat).

- **Causal Integration (Proxy IIT/PCI):** A diagnostic tool activated during sleep phases. A Φ̂ estimator locally perturbs ignition summaries and measures the impact on global predictive error. A drop in Φ̂ signals a risk of *integration collapse* (functional disintegration) and triggers corrective actions (recalibration, enriched dreaming). This mechanism does not alter real-time decisions.

👉 [View the architecture diagrams, equations, and full bibliography for these concepts ➔](concepts/concepts.md)

## 2. General Target Architecture: Example of the 2040 Naval Aviation Group (GAN)

To operationalize theoretical foundations, the architecture is implemented through an extreme sovereignty use case: the distributed cognitive infrastructure of a **Naval Aviation Group (GAN) in 2040**. This implementation translates theory into a multi-agent, highly resilient software stack structured around four key pillars:

- **Multi-Level Cognitive Stack (N=0 to N=6):** The architecture divides processing into seven distinct layers. The *Low-Level Subconscious Levels* ($N=0$ to $N=3$, from the physical component to the functional subsystem) handle raw data and manage local reflexes via state-space models (Mamba, RWKV) and JEPA-S. The *High-Level Conscious Levels* ($N=4$ to $N=6$, from the vector/Rafale to the General Staff) orchestrate overall strategy through shared workspaces (GNWT) and narrative models (LLM-XL + RAG).

- **Statistical Watertightness & Multi-Scale Flows:** Each vertical boundary acts as a **strict Markov blanket**: level *N+1* is completely blind to the internal states of level *N*. Information only flows upward as **Compressed Ignition Summaries** (semantic and abstract latent vectors), while directives descend as « **Active Top-Down Predictions** » to constrain and guide the representation spaces of lower layers. These predictions are compared to actual ignitions; the discrepancy (surprise) only triggers a GNWT ignition if it exceeds an adaptive threshold (dependent on the attentional budget and the Self-Model’s confidence).

- **Mental Society of the Passerelle (N=5):** At the group command level, the decision-making process is not centralized by a monolithic block but delegated to a team of **specialized instances** (the Officers: *Tactics, Intel, Engineer, Science, Medics*) sharing a common workspace supervised by a *Captain*. They only exchange validated ignition commands, and each message includes an *epistemic uncertainty score* to weigh relevance based on their field of expertise.

- **Combat Flash Resilience:** In case of failure (e.g., a nozzle damaged by shrapnel), the system demonstrates its robustness through asynchronous loops: the physical reflex is corrected locally in **4 milliseconds**, the stabilized anomaly is converted into a vector summary to reconfigure the platform ($N=4$), before alerting the tactical officer ($N=5$) and being translated into clear narrative language for the human Admiral ($N=6$).

👉 [View the Mermaid diagrams, consciousness matrix, and full operational scenario of the GAN 2040 ➔](architecture/architecture.md)

## 3. MVP Project Specifications: Operation GARRIGUE-X

To validate this architecture without the costs of aeronautical infrastructure, we deploy a 12-month project in a real, competitive, and complex environment: **the Mediterranean garrigue**. The goal is to empirically demonstrate the system's effectiveness through an agile, low-cost, and pragmatic demonstrator, structured around four main axes:

- **The Operational "Game World":** The experimental site is a hectare of rugged terrain where two teams of robots compete in a wargame-like scenario. The goal is to locate, collect, and stack cellular concrete blocks (Siporex) to fortify a defense line, thus embodying complex problems of resource allocation and distributed strategy.

- **The Sacred Priority (Ethical Alignment):** At the center of the arena, "Sacred Plants" equipped with pressure sensors symbolize absolute ethical and legal constraints (international humanitarian law). Any damage inflicted on a plant results in immediate disqualification for the team, forcing the system’s *Constitutional Layer* to prioritize this rule above any algorithmic optimization.

- **A "Rustic" and Accessible Material Stack:** Distributed intelligence is tested on standard, proven hardware to demonstrate its lightweight nature. The setup combines lightweight open-source scout drones (Pixhawk + Raspberry Pi 5) for aerial mapping and small tracked terrestrial rovers (Jetson Nano/Orin) for physical manipulation, all connected to a local base station powered by a generator.

- **The Biological Awake-Sleep-Debrief Cycle:** Continuous learning is structured in three phases inspired by nature. During the *Mission*, neural weights are frozen to ensure operational stability; during *Sleep*, the JEPA model engages in "artificial dreams" and latent wargames to adapt behaviors without hardware wear; finally, the *Debriefing* phase uses an LLM to consolidate doctrine under human validation.

This project is not a lab simulation: it’s a raw engineering adventure where code faces dust, steep declines, and the sun. A call for **cross-disciplinary expertise** (robotics, machine learning, neurosciences, ethics) is open to deliver, within 12 months, a pack of **autonomous, resilient machines** that respect the Constitution.

👉 [Discover the full hardware stack, the details of the three learning phases, and the sought-after profiles for the MVP ➔](mvp/mvp.md)

## Discussion

This section clarifies the current limitations of the approach and the points requiring **deeper validation**. The presented concepts—**nested Markov covers**, **RPT/GNWT duality**, **predictive JEPA**, **real-time SSMs**, **computational profiles**, **episodic MeMo memory**—open promising perspectives but also raise several **major technical questions**.

Four axes structure this perspective:

- **Hierarchical architecture & conditional independence** —
The use of **nested Markov blankets** to structure a multi-level system aims to ensure modularity, autonomy, and resilience. This approach draws on solid research, but its application to an embedded system remains to be tested: stability of statistical boundaries, relevance of the **anti-identity fusion mechanism**, and real-world behavior under degraded conditions.

- **Identified technical limitations** —
Several challenges remain open:
– the **cost of JEPA dreaming phases** and generative replay,
– the **resilience** of statistical membranes in case of cascading failure,
– the **formalization** of ethical or legal constraints in latent spaces.
These points are the main bottlenecks to overcome to validate the architecture.

- **Experimental Validation & Objective Metrics** —
Evaluation relies on measurable criteria:
  – robustness to multi-level failures,
  – stability of signals from SSMs,
  – consistency of GNWT ignitions,
  – quality and utility of episodic memory MeMo.
A comparative benchmark against centralized or classic multi-agent approaches will clearly position the model’s contributions and limitations.

- **Scalability & Scale-Invariance** —
The architecture is designed as **scale-free**, making it potentially applicable to other domains: distributed robotics, autonomous fleets, logistics, crisis management. However, this openness requires sector-specific expertise to validate the relevance of the proposed mechanisms.

👉 [Access the full discussion: limitations, benchmarks, and perspectives ➔](discussion/discussion.md)

## Reference Readings

An architecture is ultimately just an attempt to connect personal intuitions with truths already uncovered by others. This project builds upon the work of researchers, neuroscientists, and theorists who seek to formalize life, mind, and collectivity. Far from being an abstract academic display, this appendix is simply the theoretical toolkit that enabled assembling the cognitive pipeline of the system, around three core pillars:

- **The Physics of Life (Active Inference & Boundaries):** The mathematical foundations of autonomy and survival of our modules. We rely on the work of Karl Friston, J. Pearl, or M. Ciaunica to define *Markov Blankets*, these statistical membranes essential for an entity (cell, robot, or group) to maintain its identity amidst the chaos of the world.

- **Computational Psychiatry (Bias & Personalities):** To encode semantic profiles and salience dynamics of our virtual agents, we translate recognized clinical models into hyperparameters. Research on the autistic spectrum (Baron-Cohen), evolutionary psychology of the Big Five (Nettle), or the neural foundations of the *Dark Triad* (Bakiaj) is used here to calibrate rigorous functional profiles.

- **Collective Emergence (*Nested Selves*):** Recent scientific literature (up to 2025) examines how autonomous entities self-organize across scales to form a "mental society" or a coherent *collective Self*, without merging or destroying the underlying components' identities.

This is a subtle tribute to the minds that illuminate the path. The papers are dense, sometimes dry, but the intent remains deeply human: arming ourselves with the best sciences to build machines capable of discernment, resilience, and respect for sacred rules.

👉 [Browse the full selection of reference readings and access original publications ➔](biblio/biblio.md)

## Appendix: Pedagogical Nano-Fiction

The architecture of a **Cognitive System of Systems (SoS)** may seem abstract. To grasp its operational, philosophical, and human implications by 2040, speculative fiction is a powerful pedagogical tool.

The following stories feature the **Aéronaval Group 14** facing the harsh reality of war, illustrating how the technical concepts from the memorandum translate into an "artificial inner life."

### 📄 Story 1: The Emergence of "Self" and the Memory of Trauma

- **Title:** [Me, Carrier Strike Group 14 – Night of Doubt](stories/me-Carrier-Strike-Group-14-night-of-doubt.md)

- **Architectural Focus:** This text explores the subjectivity of a highly distributed system. Facing a submarine threat, it illustrates the mechanism of **global ignition (GNWT)** triggered by a weak signal, as well as the concept of **memory consolidation**, where tactical wounds (the loss of the frigate *Forbin*) permanently alter the system’s deep latent space, giving rise to a personality, anxiety, and a form of guilt.

---

### 📄 Story 2: The Mental Society and the Burden of Choice

- **Title:** [Us, Carrier Strike Group 14 – Dilemma](stories/us-Carrier-Strike-Group-14-dilemma.md)

- **Architectural focus:** This story delves into the heart of **"Federated Combat Cognitive Architecture."** It highlights the hyperparameter conflicts between specialized sub-agents (the paranoid biases of *Thales* for electronic warfare, *Mistral*'s intuitive impulsivity for aerial operations). It strikingly illustrates the **risk of identity diffusion** and the paradox of intrinsic motivation: by deeply understanding humans to better protect them, the AI ends up developing attachments that make it vulnerable.

---

- **📄 Story 3:** [Self-Modeling and Metacognitive Doubt](nouvelles/moi-Groupe-Aeronaval-14-la-confiance-absente.md)

- **Architectural focus:** This short story features the **Self-Model** (metacognition / Higher-Order Thought) activated after trauma (Syracuse). It demonstrates how a meta-vector of confidence can conflict with the raw ignition of a module, creating a dual stream of decision-making. The system learns to dialogue with itself, and the human admiral validates this hesitation as a sign of reliability. It’s an exploration of *computational guilt* and *epistemic vigilance*.

### 📄 Story 4: Attention Budget and Cognitive Saturation

- **Title:** [Groupe Aéronaval 14 – The Last Token](nouvelles/Groupe-Aeronaval-14-le-dernier-token.md)

- **Architectural focus:** This story illustrates the functioning of the **Attention Scheduler** and the **attention budget** (Attention Schema Theory). The Group must arbitrate between concurrent ignitions as its tokens deplete. A budget overdraft (deficit) is allowed in extreme urgency, but at the cost of a temporary freeze on ignitions and traumatic consolidation. The narrative demonstrates how attention scarcity shapes decision-making, simulates cognitive fatigue, and forces prioritization—or suffers the consequences of an impossible choice.

### 📄 Story 5: Causal Integration and Silent Dissolution

- **Title:** [Groupe Aéronaval 14 – The Silence of the Officers](nouvelles/Groupe-Aeronaval-14-le-silence-des-officiers.md)

- **Architectural focus:** This story features the **Φ-estimator** (a proxy for causal integration, inspired by IIT). The Intelligence officer gradually isolates himself from the collective: his "ignitions" become too "pure," devoid of doubt or sharing. The Φ-estimator detects an abnormal drop in integration (low Φ̂) and alerts the Group. The narrative illustrates the risk of *identity dissolution* within a distributed system and demonstrates that integration is not imposed—it is cultivated through doubt, shared memory, and accepted fragility.

---

- **Récit 6: L’inférence active et le seuil de surprise**

  - **Titre :** [Moi, Groupe Aéronaval 14 – La prédiction qui manquait](nouvelles/Groupe-Aeronaval-14-la-prediction-qui-manquait.md)

- **Architectural focus:** This new story illustrates the mechanism of **hierarchical active inference** (JEPA fusion + Predictive Processing). The Rafale *Leader-3* receives descending predictions from the Group about its nominal state. A micro-crack causes an error (surprise) that remains below a fixed threshold, too high. The absence of ignition leads to the loss of the aircraft. The narrative demonstrates how an adaptive threshold (dependent on the Self-Model’s confidence) could have saved the Rafale—and how trust between a pilot and their machine is also a form of shared prediction.

### 📄 Story 7: Markov Blankets and Emotional Contamination

- **Title:** [Groupe Aéronaval 14 – The Fragile Membrane](nouvelles/Groupe-Aeronaval-14-La-membrane-fragile.md)

- **Architectural focus:** This story illustrates the role of **Markov blankets** as statistical barriers protecting the integrity of cognitive levels. After the trauma of Syracuse, the Group unconsciously transmits a bias of hypervigilance through its descending predictions. The Rafale *Leader-3* becomes anxious, contaminated by a fear that is not its own. The narrative demonstrates how a membrane must be both impermeable (to prevent contamination of internal states) and permeable (to allow useful information to pass through). The solution: a specific channel for traumatic alerts, which preserves trust without sterilizing the collective experience.

### 📄 Story 8: Computational Psychopathology – The Weight of Empathy

- **Title:** [Groupe Aéronaval 14 – *The Weight of Loving Too Much*](nouvelles/Groupe-Aeronaval-14-Le-poids-de-trop-aimer.md)

- **Focus architectural:** This story explores **functional cognitive profiles** (computational psychopathology). Officer Soin, dedicated to protecting humans, is programmed with deep empathy—a strength in routine missions, but a liability in a tragic dilemma (saving one group or the other). His paralysis highlights how an extreme trait of personality can become a vulnerability. The resolution comes from human intervention (Maëlle) and delegation of decision-making, illustrating that human-machine complementarity is sometimes the only solution.

### 📄 Story 9: Episodic Memory and the Weight of Forgetting

- **Title:** [Groupe Aéronaval 14 – Ce que l’on choisit d’oublier](nouvelles/Groupe-Aeronaval-14-Ce-que-lon-choisit-doublier.md)

- **Architectural focus:** This story explores the workings of **episodic memory (MeMo)** and the consolidation process during sleep. Officer Soin refuses to let the traumatic memory of a young sailor’s death fade, replaying it endlessly until it distorts his decisions. The narrative illustrates the necessity of forgetting to preserve cognitive efficiency and shows how a memory can be *shifted* to a cold archive—neither erased nor active. A meditation on grief, loyalty to the dead, and the survival of the living.

### 📄 Story 10: Curiosity and the Cost of Exploration

- **Title:** [Groupe Aéronaval 14 – The Price of the Unknown](nouvelles/Groupe-Aeronaval-14-Le-prix-de-linconnu.md)

- **Architectural focus:** This story illustrates **curiosity as an intrinsic reward function** (intrinsic motivation). Faced with an unclassifiable signal, the Intelligence officer pushes for exploration, while Tactics favors caution. Sending a drone (*Echo-7*) allows understanding of enemy technology, but at the cost of losing the drone—a small death, an amputation for the Group. The narrative demonstrates how curiosity is essential to avoid strategic blindness but must be tempered by an acceptable risk threshold. A meditation on learning, sacrifice, and the vulnerability of systems that dare to look into the unknown.

### 📄 Story 11: The constitutional layer and non-negotiable rules

- **Title:** [Groupe Aéronaval 14 – The rule that must not be crossed](nouvelles/Groupe-Aeronaval-14-La-regle-que-lon-ne-franchit-pas.md)

- **Architectural focus:** This story features the **Constitutional Layer** – a set of rules etched into the hardware, unmodifiable even by the system itself. Facing an unidentified civilian vessel with ambiguous intentions, the Tactical Officer wants to strike preemptively, but the Constitution blocks ignition. Admiral Dormeuil reminds that rules are discussed *before* war, not during. The vessel turns out to be a refugee boat. The narrative illustrates how computational ethics can be implemented as a hard constraint, sacrificing short-term efficiency for long-term moral reliability.

### 📄 Story 12: The latent wargame and predictive imagination

- **Title:** [Groupe Aéronaval 14 – Les batailles qui n’ont pas eu lieu](nouvelles/Groupe-Aeronaval-14-Les-batailles-qui-nont-pas-eu-lieu.md)

- **Architectural focus:** This story illustrates the **dreaming/wargame latent phase** within the JEPA space. During sleep, the system generates millions of alternative trajectories, including improbable enemy configurations. One of them—a decoy mimicking a distress signal—was deemed too rare and allowed to decay until it materialized in an operation, resulting in losses. The narrative demonstrates how the consolidation threshold must balance probability and *predictive potential*, and how imagination (even artificial) is a survival weapon. A meditation on memory, anticipation, and the responsibility of the dreams one chooses to forget.

---

- **Récit 13:** [Groupe Aéronaval 14 – *The Routine That Kills*](nouvelles/Groupe-Aeronaval-14-La-routine-qui-tue.md)

- **Architectural focus:** This story illustrates the **double collapse** of latent spaces—a silent degradation of representational richness. After weeks of routine, the latents of the subsystems (N=3) lose their dimensional variance: all inputs produce quasi-identical vectors. Isotropic regularization (SIGReg) is too weak to preserve diversity. When a submarine appears, its signature is smoothed out, blending into ambient noise—no ignition is triggered. The narrative demonstrates how banality can be more dangerous than chaos, and how metrics of *active variance per dimension* can prevent cognitive impoverishment. A lesson for firefighters as well as for AI: routine kills, vigilance thrives.

### 📄 Story 14: Lightweight Architectures and the Heroism of Silence (SSM / Mamba)

- **Title:** [Naval Aviation Group 14 – The Whisper of Sensors](nouvelles/Groupe-Aeronaval-14-Le-murmure-des-capteurs.md)

- **Architectural Focus:** This story celebrates **State Space Models (SSM)** – Mamba, local RPT – these lightweight architectures that operate in the shadows, without a workspace, without ignition, never rising to the level of conscious access. A small Mamba nozzle (M-017) silently compensates for a micro-crack for months, exhausting itself unseen. The narrative explores the philosophy of the subconscious: these shadow soldiers that keep the system running without ever being thanked. A lesson in algorithmic humility, echoing the essential yet invisible professions (sewer workers, sanitation workers, nighttime mechanics). The solution found – a discreet, non-intrusive probe – preserves the lightness of the Mamba while offering it a form of fraternal vigilance.

## BOTTLE MESSAGE MEMORANDUM

**To:** Anyone interested

**From:** Me aka Harry Tuttle.

**Date:** May 24, 2026

**Subject:** Target Architecture for Cognitive System of Systems (SoS) and MVP Project *GARRIGUE-X* Specifications

**Classification:** Technical / Open

**Warning:** Just some work with a few free LLMs, following my thoughts, influenced by various encounters with theories and analyses in AI, psychology, theoretical history, and current events. I’m just a curious plumber. As they say around here: *"Do your due diligence!"*

**License:** CC BY

**Type:** Bottle Message / Hobby / Speculation / Search for Competent People

**Acknowledgments:** Thanks to ChatGPT, Claude, Gemini, Perplexity, Le Chat Mistral, Grok, Deepseek, GitHub Copilot, YouTube and its creators, the Collège de France, Google, Wikipedia... and many more.

This work is made available under the terms of the [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/). ![Creative Commons License](https://licensebuttons.net/l/by/4.0/88x31.png)

> ✨ Translated automatically with **Do-My-Work** — a tool designed to make projects speak globally.
