> ✨ Translated automatically with [**Do-My-Work**](https://github.com/AlainCo/do-my-work) — profile: technical.

# Key Concepts and Theoretical Foundations

To prove the viability of this architecture to our peers, every software engineering decision is based on major milestones in the scientific literature on neuroscience, AI, and theoretical physics.

## A. Conditional Independence: Nested Markov Blankets

**Theoretical Foundation**:
[Judea Pearl, *Probabilistic Reasoning in Intelligent Systems*, 1988](https://www.sciencedirect.com/book/monograph/9780080514895/probabilistic-reasoning-in-intelligent-systems) for Bayesian networks;
[Kirchhoff, Parr, Palacios, Friston, Kiverstein, *The Markov blankets of life: autonomy, active inference and the free energy principle* (2018)](https://royalsocietypublishing.org/doi/10.1098/rsif.2017.0792) for theoretical biology;
[Ciaunica, Levin, Rosas, Friston et al., *Nested Selves: Self-Organization and Shared Markov Blankets in Prenatal Development in Humans* (2023)](https://onlinelibrary.wiley.com/doi/10.1111/tops.12717) for generalization to collective systems.

**The Concept:** The Markov blanket refers to the statistical membrane separating the internal states ($I$) of a system from the external states ($E$) of its environment. It consists of sensory states (inputs) and active states (outputs). The fundamental equation of independence is written as:

$$P(I \mid B, E) = P(I \mid B)$$

**What recent literature adds:** A collective of active inference agents can, if it maintains a Markov blanket at the group level, constitute a higher-level agent with its own generative model. This property is *scale-free*: it applies from the cell to the organism, and from the effector to the carrier strike group. The structures nest like Russian dolls.

**Technical Justification:** This is the principle of **identity anti-fusion**. The higher level ($N+1$) never processes the raw data of $N$ — only its statistical API (the *ignition summary*). This ensures strict modularity of the component up to the entire fleet, and preserves the identity of each level as a distinct cognitive entity. A conscious Rafale is perceived by the group as an opaque external object — exactly as you perceive your liver as "doing well" without accessing the hepatocytes.

```mermaid
flowchart TD
    subgraph N6 ["N=6 : Headquarters"]
        N6c["LLM-XL + RAG"]
    end

    subgraph N5 ["N=5 : Carrier Strike Group"]
        N5c["Officers + GNWT Workspace"]
    end

    subgraph N4 ["N=4 : Platform (Rafale)"]
        N4c["JEPA-M + Workspace"]
    end

    subgraph N3 ["N=3 : Sub-systems"]
        N3c["JEPA-S + Local RPT"]
    end

    N6c ---|"Ignition Summary\n(latent vector)"| N5c
    N5c ---|"Ignition Summary"| N4c
    N4c ---|"Ignition Summary"| N3c

    N3c ---|"Contextual Priors"| N4c
    N4c ---|"Contextual Priors"| N5c
    N5c ---|"Strategic Objectives"| N6c

    classDef blanket fill:#e0f2f1,stroke:#00695c
    class N3c,N4c,N5c,N6c blanket
```

### B. The Two-Tier Consciousness: GNWT + RPT as Facets of the Same Mechanism

**Theoretical Foundation:** [Bernard Baars, *A Cognitive Theory of Consciousness*, 1988](https://philpapers.org/rec/BAAACT) and [Stanislas Dehaene (*A Neuronal Model of a Global Workspace in Effortful Cognitive Tasks*, 2006)](https://nyaspubs.onlinelibrary.wiley.com/doi/abs/10.1111/j.1749-6632.2001.tb05714.x) for the *Global Neuronal Workspace Theory* (GNWT); [Victor Lamme, *Towards a true neural stance on consciousness*, 2006](https://www.cell.com/trends/cognitive-sciences/abstract/S1364-6613(06)00237-3); work from the [COGITATE consortium](https://www.arc-cogitate.com/project) and especially [Storm et al., *An integrative, multiscale view on neural theories of consciousness*, Neuron, 2024](https://www.sciencedirect.com/science/article/pii/S0896627324000886).

**The Concept:** Long considered as competitors, GNWT and RPT actually describe **two complementary temporal and functional phases** of the same conscious processing process, as highlighted by Storm et al. in their multiscale synthesis:

```mermaid
flowchart LR
    A[Rapid Feedforward\nStage 1-2] --> B[Local Recurrence\nStage 3 - RPT]
    B --> C[Ignition + Global Broadcast\nStage 4 - GNWT]

    B -.->|"Rich Inner Life\n(Phenomenal Consciousness)"| D["'Seeing without knowing that one sees'"]
    C --> E["Conscious Access + Report\n(Access Consciousness)"]
    E -.-> F["'Knowing that one sees and being able to talk about it'"]

    classDef rpt fill:#fff3e0
    classDef gnwt fill:#e8f5e9
    class B rpt
    class C gnwt
```

**RPT** accounts for the **rich inner life** of each module through local feedback loops (recurrent processing). It explains phenomenal consciousness (PC) — the raw subjective experience, even if unreportable. **GNWT** describes what happens when a consolidated signal crosses a salience threshold and propagates widely in the global workspace, enabling **access consciousness** (AC): integration, reporting, arbitration, and voluntary control.

**Critical architectural consequence:** In our hierarchy, the RPT→GNWT threshold naturally lies at the **N=3 → N=4** boundary. Below: continuous processing in local RPT (inner life of subsystems, without global broadcast). From N=4 onwards: central workspace, ignitions, and the ability to "report" a compressed summary to the higher level.

This separation is not arbitrary—it reflects both computational constraints (cost of broadcast) and biological mechanisms identified by recent literature. As noted by Storm et al., theories do not oppose each other but operate at complementary scales: local (RPT) and global (GNWT).

**Technical Justification:** An airplane engine (N=2-3) resolves its micro-failures in local RPT loops (Mamba). If the damage exceeds its capacity, it generates a **vectorial Ignition Summary** upwards. The Rafale (N=4) captures this signal in its GNWT workspace, reconfigure its flight law, and only reports an abstract summary to the group—thus preserving Markov covers while enabling functional access consciousness at each relevant level.

## C. World Models and Hierarchical Active Inference (JEPA + Predictive Processing)

### Theoretical Foundation

- **Joint Embedding Predictive Architecture (JEPA)** : [LeCun, *A Path Towards Autonomous Machine Intelligence* (2022)](https://www.semanticscholar.org/paper/A-Path-Towards-Autonomous-Machine-Intelligence-LeCun-Courant/775f42ed458b8c5b0f2094ea4ff5b64c557b1a34) – predict abstract (latent) representations of the world rather than raw observations. It ignores unnecessary noise and favors learning causal structures.

- **Predictive Processing (PP)** : [Clark, *Whatever next? Predictive brains, situated agents, and the future of cognitive science* (2013)](https://doi.org/10.1098/rstb.2013.0176) – the brain is a prediction machine that constantly minimizes prediction error. Consciousness emerges when this error cannot be resolved locally.

- **Active inference**: [Friston, *The free-energy principle: a unified brain theory* (2010)](https://doi.org/10.1038/nrn2787) – an agent minimizes its free energy by acting on the world to make its predictions true.

- **Predictive hierarchies**: higher levels generate predictions (priors) that constrain the representations of lower levels; the residual error is propagated upward.

### The concept

Your architecture already uses **JEPA** as a latent prediction engine and **descending contextual priors**. Hierarchical active inference unifies and strengthens these two flows:

- **Descending predictions (top-down)**: each level N+1 generates a **prediction** of the ignition summary that level N should produce. This prediction is learned by the JEPA of the higher level (the encoder and the predictor).

- **Bottom-up prediction error**: Level N compares the received prediction with its actual ignition (or internal latent). The discrepancy—the **surprise**—is an error signal that propagates upward.

- **GNWT ignition threshold**: Ignition (global broadcast) only occurs when the surprise exceeds an **adaptive threshold** (dependent on the attentional budget, context, history). Below the threshold, the error is locally absorbed by updates to the latents (RPT).

- **Free energy minimization**: The entire system learns to reduce the sum of prediction errors at all levels, leading it to refine its world models (JEPA) and select actions that make the world more predictable.

In this vision, **contextual priors** are no longer fixed vectors sent unidirectionally. They are **active predictions**: the higher level *anticipates* what the lower level should see, and the lower level *adjusts* its representations to match these predictions—or reports an error if the discrepancy is too great.

> **Adaptive threshold**: defined by `threshold = f(attention_budget, Self_Model_confidence)`.
> High budget + high confidence → high threshold (few ignitions).
> Low budget + low confidence → low threshold (maximum reactivity).
> This threshold is learned during the sleep phase via free energy minimization.

### Technical justification

- **Theoretical unification**: JEPA becomes the concrete implementation of prediction in a hierarchy of active inference. It retains the advantages of JEPA (latent prediction, robustness to noise) while benefiting from the formalism of active inference (free energy, permanent top-down causality).

- **Solves the problem of top-down causality** highlighted in the discussion (§3.5): top-down predictions continuously constrain perceptual spaces, and ignition only occurs when the prediction fails.

- **Improves stability and learning**: the prediction error is a dense signal for continuous learning (sleep phase). The system can "dream" by generating its own predictions and minimizing the error on simulated trajectories.

- **Adaptive ignition threshold**: attentional scarcity (budget) and confidence (self-model) can modulate the threshold, making the system less verbose under nominal conditions and more responsive in surprising situations.

### Diagram

```mermaid
flowchart TD
    subgraph NiveauSup ["Level N+1 (ex. N=5 Group)"]
        Pred["Prediction of the summary\n(by JEPA-M)"]
        Seuil["Adaptive threshold\n(budget, confidence)"]
    end

    subgraph NiveauInf ["Level N (ex. N=4 Rafale)"]
        Latent["Internal latent RPT/JEPA"]
        Ignition["Real Ignition summary"]
        Erreur["Prediction error\n(surprise)"]
    end

    Pred -->|"descend"| Erreur
    Ignition -->|"entre"| Erreur
    Erreur -->|"if difference < threshold"| MiseAJour["Local update of the latent\n(RPT, no ignition)"]
    Erreur -->|"if difference ≥ threshold"| GNWT["GNWT Ignition\n(global broadcast)"]

    GNWT -->|"goes up to the higher level"| Pred

    style Pred fill:#e8f5e9,stroke:#43a047
    style Erreur fill:#fff3e0,stroke:#f57f17
    style GNWT fill:#ffebee,stroke:#c62828
```

### Concrete example: catapult anomaly revisited
```

**Nominal situation**: The Rafale's JEPA-M (N=4) predicts that its next ignition summary will be `[nominal_state, thrust=1.0]`. The higher level (N=5) sends this prediction. The Rafale compares it with its actual ignition (same). The error is almost zero → no ignition. The system operates in silent mode, conserving resources.

**Anomaly**: The nozzle is damaged. The Rafale generates an actual ignition `[degraded, asymmetry=0.73]`. The downward prediction (nominal) produces a significant error. Since the error exceeds the adaptive threshold (e.g., 0.5), a **GNWT ignition** is triggered. This is sent to the higher level and updates the prediction for future cycles (learning).

**Learning**: During the sleep phase, the system replays this sequence. The JEPA learns to predict the degraded ignition from the context of the anomaly. The next time a similar asymmetry appears, the downstream prediction will be `[degraded, asymmetry≈0.7]`, the error will remain low, and no ignition will be necessary – unless the anomaly worsens.

### D. Lightweight Architectures for Real-Time: SSMs (Mamba, RWKV, xLSTM)

**Theoretical Foundation**:
[Gu & Dao, *Mamba: Linear-Time Sequence Modeling with Selective State Spaces* (2023)](https://arxiv.org/abs/2312.00752) ;
[Peng et al., *RWKV: Reinventing RNNs for the Transformer Era* (2023)](https://arxiv.org/abs/2305.13048) ;
[Beck et al., *xLSTM: Extended Long Short-Term Memory* (2024)](https://arxiv.org/abs/2405.04517).

**The Concept:** *State Space Models* (SSMs) offer an alternative to Transformers for low-level layers (N=0 to N=3), with crucial properties for embedded systems:

| Architecture | Key Advantage | Target Usage in SoS |
|---|---|---|
| **MLP nano + PID** | µs, deterministic, FPGA | N=0: physical control loop |
| **Mamba-mini** | linear in sequence, low RAM | N=1: smart actuators |
| **Mamba / RWKV** | 5× throughput vs Transformer, continuous | N=2-3: subsystems, perception |
| **JEPA-S** | latent prediction, local RPT | N=3: onset of inner life |
| **JEPA-M/L + GNWT** | workspace, ignition, broadcast | N=4-5: platform awareness |
| **JEPA-XL + LLM** | narrative, strategic, multimodal | N=5-6: command, admiral dialogue |

**Technical Justification:** Mamba demonstrates smoother and physically more plausible control signals than Transformers (which can produce discontinuities in control signals). For layers N=1 to N=3, this is exactly what is needed: smooth, continuous, reactive processing, without the quadratic cost of attention.

### E. Computational Psychopathology and Functional Profiles

**Theoretical Foundation:**
[Friston, *Computational psychiatry: from synapses to sentience* (2022)](https://www.nature.com/articles/s41380-022-01743-z) ;
[Teufel & Fletcher, *The promises and pitfalls of applying computational models to neurological and psychiatric disorders* (2016)](https://academic.oup.com/brain/article/139/10/2600/2196698) ;
[Karl Friston, *Computational psychiatry: from synapses to sentience*](https://www.nature.com/articles/s41380-022-01743-z)
[Nettle, *Personality: What makes you the way you are* (2023)](https://www.researchgate.net/publication/375324828_Personality_What_Makes_You_The_Way_You_Are) for the evolutionary Big Five model ;
[Baron-Cohen, *Autism: the empathizing-systemizing (E-S) theory* (2009)](https://pubmed.ncbi.nlm.nih.gov/19338503/) ;
[Bakiaj, Pantoja Muñoz, Bizzego, Grecucci, *Unmasking the Dark Triad: A Data Fusion Machine Learning Approach to Characterize the Neural Bases of Narcissistic, Machiavellian and Psychopathic Traits* (2025)](https://onlinelibrary.wiley.com/doi/10.1111/ejn.16674).

**The Concept:** Personality traits are modeled as **hyperparameter adjustments** in the processing of error probabilities. These are not "modes" that are activated, but structural biases in salience functions and ignition thresholds.

**Officer Profiles and Their Neuroscientific Basis:**

| Role | Dominant Trait | Mechanism | Preferred Ignition Domain |
|---|---|---|---|
| **Science / Analysis** | Openness + TSA-Systemizing | Strong local connectivity, weak long-range | Anomalies, logical inconsistencies, weak signals |
| **Care / Crew** | High agreeableness, active insula/ACC | Oxytocin, empathy circuits | Human internal states, ethics, cohesion |
| **Engineer** | Very high conscientiousness | Strong PFC, inhibitory control, low impulsivity | Failures, system drifts, execution quality |
| **Tactical** | Persistent + Moderate Dark Triad | Memory of failures, low fear processing | Threats, vulnerabilities, windows of action |
| **Intelligence** | Openness + Low agreeableness | Exploratory dopamine, inconsistency detection | Adverse patterns, deception, information asymmetry |
| **Captain** | Extraversion + Situational neuroticism | DA reward, PFC flexibility, arbitration | Crises, opportunities, global mission narrative |

**Anti-fusion by profile:** Each officer's latent spaces are **non-shared**. They only exchange *ignition summaries* via the command channel. Each officer's episodic memory is their identity — that's what is preserved, like craniopagus twins who maintain distinct wills despite partially shared circuits.

**Technical Justification:** Computational autism (overweighting of sensory precision over contextual expectations) is injected into the low radar layers (N=3) to isolate weak signals without contextual bias. Functional Dark Triad traits: Machiavellianism in cyber deception algorithms (game theory), functional psychopathy in the execution speed of firing effectors (N=4) — cold, non-empathic, but constitutionally constrained.

### F. Exploration through Curiosity and Learning through Play

**Theoretical Foundation:**
[Jürgen Schmidhuber, *Formal Theory of Creativity, Fun, and Intrinsic Motivation*, 1990-2010](https://www.researchgate.net/publication/224155374_Formal_Theory_of_Creativity_Fun_and_Intrinsic_Motivation_1990-2010) ;
[Oudeyer & Kaplan, *What is Intrinsic Motivation? A Typology of Computational Approaches* (2007)](https://doi.org/10.3389/neuro.12.006.2007) ;
[Oudeyer, *Intrinsic Motivation Systems for Autonomous Learning*, 2007](https://web-archive.southampton.ac.uk/cogprints.org/5473/index.html).

**The Concept:** Curiosity is an **intrinsic reward function** based on information gain (reduction of predictive entropy). The agent is rewarded when it explores areas where its world model is still imprecise — neither too simple (boring) nor too chaotic (incomprehensible). The optimal learning zone is where *learning progress* is maximal.

**The game as a training protocol:** Non-operational phases are structured as *wargames* with variable rules. The system plays against itself (MCTS variant in the JEPA latent space), against simulated parametric adversaries, and against past versions of itself. Each gaming session generates *surprise vectors* that feed the Dreaming phase (see Learning Cycle, §3.C).

**Technical Justification:** This prevents system brittleness in *Out of Distribution* situations. A system trained solely on real mission data will struggle with unseen situations. Gaming generates low-cost experience diversity.

### G. Continuous Episodic Memory (MeMo / Continuous Online Training)

**Theoretical Foundation:**
[Quek et al., *MeMo: Memory as a Model* (2026)](https://arxiv.org/abs/2605.15156) ; [Kirkpatrick et al., *Overcoming Catastrophic Forgetting* (2017)](https://arxiv.org/abs/1612.00796) ; [Walker, *The Role of Sleep in Cognition and Emotion* (2017)](https://pubmed.ncbi.nlm.nih.gov/19338508/).

**The Concept:** Episodic memory is not just a log of events, but a **continuous flow of compressed latent vectors** that captures only moments of high salience (ignitions). Each significant event becomes a **rich episodic memory**: JEPA latent state + contextual metadata.

**Concrete Example: Catapult Anomaly**

```mermaid
flowchart TD
    subgraph Mission ["Phase 1 : Real-Time Mission"]
        A["T=14h23\nIgnition N=4 (Rafale)"] 
        B["Catapult anomaly detected\nsalient = 0.87"]
        C["MeMo Capture\n→ Episodic Vector"]
    end

    Mission -->|"Transfer of black boxes"| Sleep

    subgraph Sleep ["Phase 2 : Sleep & Daydreaming"]
        D["Generative Replay JEPA\n(Simulation of variants)"]
        E["Recalibration of ignition thresholds\n(PISTE Module)"]
        F["Consolidation\n→ Long-Term Memory (RAG)"]
    end

    Sleep -->|"Update + Consolidation"| Consultation

    subgraph Consultation ["Phase 3 : Subsequent Consultation\n(T+30 days)"]
        G["New similar anomaly detected"]
        H["Episodic RAG retrieves\nmemory T=14h23"]
        I["Proactive suggestion\n→ Workaround 'catapult_B'"]
    end

    classDef ignition fill:#fff3e0,stroke:#f57f17,stroke-width:2px
    classDef replay fill:#f3e5f5,stroke:#8e24aa
    class A,B,G ignition
    class D replay
```

**Episodic vector detail stored:**

```
Ignition_ID: 2026-05-24_1423_Leader3
Module: PISTE_N4
Salient: 0.87
JEPA latent state: [0.42, -0.17, 0.91, ..., 0.63]
Tags: [catapult_anomaly, thrust_asymmetry, degraded]
Outcome: mission_abort=false
Workaround: catapult_B
Context: 25kt_wind, wet_deck, formation_leader
```

**Technical Justification:** This is the fundamental difference between a system that *performs* and a system that **truly learns** from its experience. The episodic memory MeMo also becomes the support for the **durable identity** of each module or officer — its personal biography of ignitions constitutes its computational "self," preserved even after weight updates.

**MeMo Mechanism:**

- **Mission:** Streaming capture of ignitions (N=3 → N=6)

- **Daydreaming:** Generative Replay in the JEPA latent space

- **Debriefing:** Consolidation and sedimentation in long-term memory (episodic RAG)

This mechanism enables both continuous learning without *catastrophic forgetting* and the preservation of a unique identity for each entity in the SoS.

### H. The Stability of Latent Spaces: Size, Collapse, and Structural Constraints

**Theoretical Foundation:**
LeCun et al., *Joint Embedding Predictive Architectures* (2022–2024);
Assran et al., *Self-Supervised Learning from Images with a Joint-Embedding Predictive Architecture* (2023);
Bardes et al., *VICReg: Variance-Invariance-Covariance Regularization* (2022);
Zhang et al., *LeJEPA: Latent Euclidean JEPA with Isotropic Gaussian Regularization* (2024);
Hafner et al., *World Models* (2021–2024).

#### The Problem: A Latent Space Must Be Bounded… but Not Empty

In the architectures presented earlier — **local RPT**, **predictive JEPA**, **Ignition GNWT summaries** — everything relies on a common principle:
the system encodes the world in a **compact latent space**, exchanged between levels via Markov covers.

But a bounded latent space poses a classic dilemma:

- **Too small** → information loss, poor predictions, unusable Ignition signals.

- **Too large** → the model "cheats", encodes noise, or worse:
**collapse** (all inputs → same vector).

This phenomenon is well documented in JEPAs and modern SSL methods: without structural constraints, the model converges to a trivial solution that minimizes loss without learning useful structure.

#### Current Solutions: Constraining the Latent Distribution

##### 1. Historical Heuristics (BYOL, SimSiam, DINO)

The first generations of self-supervised models avoided collapse through ad hoc mechanisms:

- **Stop-gradient** (BYOL, SimSiam)

- **Teacher–student EMA** (MoCo, DINO)

- **Asymmetric augmentations**

- **Forced normalization** (BatchNorm, LayerNorm)

- **Decorrelation** (VICReg, Barlow Twins)

These methods work, but remain fragile and require fine-tuning of hyperparameters.

##### 2. The Theoretical Turning Point: Gaussian Isotropy (LeJEPA, SIGReg)

Recent work by Zhang et al. (2024) proposes a more principled approach:

> **A useful latent space must follow an isotropic Gaussian distribution.**

Why?
Because an isotropic latent:

- uses **all dimensions**,
- avoids dead or crushed directions,
- remains **well-conditioned** for prediction,
- naturally prevents collapse.

To enforce this property, LeJEPA introduces **SIGReg** (*Sketched Isotropic Gaussian Regularization*):

- project the latents onto many random directions,

- force each projection to follow a **N(0,1)**,

- by the Cramér–Wold theorem, the multivariate distribution becomes isotropic.

**Effect:**
a latent space **full**, **bounded**, **stable**, without stop-gradient or special architecture.

##### 3. LeWM: Minimalist and Stable JEPA World Model

LeWM (2024) applies this principle to a **JEPA world model**:

- encoder → latent

- predictor → future latent

- only two losses:
**prediction** (MSE),
**isotropy** (SIGReg)

Result:
a compact, stable predictive model, usable for **latent daydreaming** (generative replay).

#### Application to Our Architecture: RPT, JEPA, and Ignition Summaries

In our hierarchy, three latent spaces coexist:

- **Internal RPT Latent (N=2–3)**
  local recurrent loop
  encodes the "inner life" of the module
  must be compact but expressive

- **Predictive JEPA Latent (N=3–4)**
  abstract world model
  must be stable for prediction and dreaming

- **Ignition Summary GNWT (N=3→4→5)**
  short vector exchanged between levels
  statistical API between Markov blankets

All three suffer from the same risk:
**internal collapse + excessive compression = loss of critical information.**

Using isotropic regularization (like LeJEPA) allows:

- to avoid collapse in internal latents,

- to ensure that each dimension carries information,

- to stabilize inter-level exchanges,

- to make Ignition summaries more reliable and comparable.

#### Current Obstacles and Open Questions

Despite these advances, several challenges remain open:

- **Optimal latent dimension**: no analytical formula exists.

- **Multi-level propagation**: how to ensure that isotropy is maintained across Markov blankets?

- **Ignition compression**: risk of "double collapse" if the internal latent is already poor.

- **Ethical/legal constraints**: how to encode them in a regularized latent space?

- **JEPA daydreaming**: computational cost still high, even in latent.

These points constitute essential **experimental validation axes** for the continuation of the project.

## I. Self-modeling and metacognition: the self-schema (Higher-Order Thought)

### Theoretical foundation

- **Higher-Order Thought (HOT)**: Rosenthal (2005) – a mental state becomes conscious when it is accompanied by a higher-order thought about it.

- **Self‑Model Theory of Subjectivity** : [Metzinger (2003)](https://mitpress.mit.edu/9780262528193/being-no-one/) – the phenomenal self is a model that the brain constructs of itself in real time.

- **Metacognition in AI** : confidence models, performance prediction, decision calibration.

- **Recent applications** : [Bahrami et al., *Metacognitive reinforcement learning* (2024)](https://arxiv.org/abs/2401.08099) – self-assessment improves adaptation.

### The concept

In your architecture, each conscious module (N≥4) has a **Self‑Model** : a small network (MLP or lightweight transformer) attached to its GNWT workspace.
At each ignition, the Self‑Model generates a **meta-vector** that encodes:

- a **confidence score** in the ignition (derived from local prediction error),

- an **ignition context** (type of anomaly, origin),

- an **expected salience** for the higher level.

This meta-vector is then:

- stored in episodic memory (MeMo) alongside the memory,

- used to modulate decisions of the higher level (e.g.: the Captain officer weighs ignitions by their confidence),

- sent to the human interface (N=6) for explainability.

The Self-Model is trained **during the sleep phase**: it is asked to predict the actual salience that occurred after each past ignition, or to predict the error of a neighboring module. Thus, it learns to know the strengths and weaknesses of the system – a form of **computational metacognition**.

### Technical Justification

- Fills a major gap identified in the discussion (§3.3): the absence of agentive self-modeling.

- Allows the system to signal its own biases (e.g., "I am the Tactical Officer, my confidence is low on this scenario").

- Improves robustness: if the Self-Model detects a generalized drop in confidence, it can trigger a **targeted daydream** to relearn.

- Makes the architecture more explainable for human operators (N=6 can query the Self-Model via the LLM).

### Diagram

```mermaid
flowchart TD
    subgraph Workspace ["GNWT Workspace (N=4 or N=5)"]
        I["Current Ignition\n(latent vector)"]
        SM["Self-Model\n(MLP)"]
        M["Meta-vector\n[confidence, context, expected salience]"]
    end

    I -->|"feeds"| SM
    SM --> M

    M -->|"storage"| MeMo["Episodic Memory\n(MeMo)"]
    M -->|"modulation"| Decision["Higher-level arbitration"]
    M -->|"explainability"| LLM["N=6 Interface (LLM)"]

    style SM fill:#f3e5f5,stroke:#8e24aa
    style M fill:#e1bee7
```

### Concrete example: catapult anomaly (reusing the MeMo example)

During the *Catapult Anomaly* ignition (salient 0.87), the Self-Model of the Rafale (N=4) generates a meta-vector:

```
confidence: 0.82
context: "thrust_asymmetry, catapult_workaround_B"
expected_salience: 0.85
```

This vector is stored with the episodic memory.
Later, when a similar anomaly occurs, the Self-Model is consulted: its high confidence allows the workaround to be reused without waiting for validation from the higher level.
Conversely, if the confidence had been low (e.g., 0.35), the system would have required human confirmation.

## J. Competitive Attention and Budget: The Attention Schema (Attention Schema Theory)

### Theoretical Foundation

- **Attention Schema Theory (AST)**: Graziano & Webb (2015) – the brain constructs a simplified model of its own attention process, called an *attention schema*, which allows controlling and predicting the focus of attention.

- **Attentional resources**: Kahneman (1973) – attention is a limited resource, shareable between tasks, with a budget that recharges.

- **Cognitive inhibition**: Aron (2011) – inhibitory control is essential to avoid saturation and conflicts.

- **AI application**: attention models with computational cost, *sparse attention*, *budgeted attention* (Clark et al., 2022).

### The concept

Your architecture has a **global workspace (GNWT)** where ignitions are broadcasted. Without limits, the system risks **attentional inflation**: too many simultaneous ignitions would saturate the workspace, degrade decision quality, and blur prioritization.

To avoid this, each conscious level (N≥4) is equipped with an **Attention Scheduler** that manages a **global attentional budget** (example: 100 "attentional tokens").
Operation:
[/SOURCE TEXT]

- Each ignition consumes a certain number of tokens (for example, 5 tokens for a normal ignition, 10 for a critical ignition).

- The budget recharges linearly over time (example: +1 token per second).

- If the budget is insufficient, the ignition is **deferred** (queued) or **inhibited** (lost).

- The **salience threshold** required to trigger an ignition can be dynamically adjusted by the scheduler depending on the load (when the budget is low, only the most salient ignitions pass).

The Attention Scheduler does not decide *what* to ignite – that is the responsibility of the RPT modules – but it **allocates the resource** and can **prioritize** between concurrent ignitions. It relies on an AST component that models the state of the budget and predicts future costs.

### Technical Justification

- Fills a major gap in the current architecture (section 3.2 of the discussion): the lack of an inhibitory mechanism. Without a budget, the system risks *narrative drift* and loss of reactivity.

- Allows simulation of metabolic constraints (a biological brain cannot process everything at once).

- Facilitates arbitration between officers: the Captain does not need to compare all ignitions; the scheduler has already filtered them.

- Improves combat robustness: in stressful situations (low budget), only immediate threats pass – non-critical ignitions are postponed.

### Diagram

```mermaid
flowchart TD
    subgraph Inputs ["Sub-systems (N≤3)"]
        A["Local RPT\n(moderate anomaly)"]
        B["Local RPT\n(imminent threat)"]
        C["Local RPT\n(minor failure)"]
    end

    subgraph Scheduler ["Attention Scheduler (N=5)"]
        Budget["Attention budget\n(100 tokens, recharge +1/s)"]
        AST["AST module\n(predicts cost/benefit)"]
        File["Queue (deferred)"]
        Seuil["Adaptive threshold"]
    end

    subgraph Workspace ["GNWT Workspace"]
        Ignition["Broadcasted ignition"]
    end

    A -->|"request (5 tokens)"| Scheduler
    B -->|"request (10 tokens)"| Scheduler
    C -->|"request (3 tokens)"| Scheduler

    Budget -->|"consumption if sufficient"| Ignition
    Budget -->|"if insufficient"| File
    AST -->|"adjusts threshold"| Seuil
    Seuil -->|"filters"| Workspace

    File -.->|"resumed when budget recharged"| Workspace

    style Scheduler fill:#fff3e0,stroke:#f57f17
    style Budget fill:#ffe0b2
```

### Concrete example: intense combat

During an engagement phase, the attention budget of the Group (N=5) drops to 15 tokens (recharge +1/s). The Tactical Officer receives three simultaneous ignitions:

- **Ignition A** (missile threat, salience 0.95, cost 10 tokens) – accepted, budget → 5 tokens.

- **Ignition B** (secondary radar anomaly, salience 0.60, cost 5 tokens) – rejected due to lack of budget, queued.

- **Ignition C** (drone scout engine failure, salience 0.70, cost 5 tokens) – also rejected.

The scheduler prioritizes the imminent threat. When the budget rises again (after 5 seconds), the radar anomaly is processed – but if a new threat arrives in the meantime, it will take priority. This mechanism prevents saturation and ensures that critical decisions are not drowned out by noise.

## K. Causal integration: the Φ thermometer (sleep phase)

### Theoretical foundation

- **Integrated Information Theory (IIT)** : Tononi (2004, 2015) – consciousness is identified with a system's ability to integrate information, measured by Φ (phi). A system with a high Φ has a unified experience.

- **Perturbational Complexity Index (PCI)** : Massimini et al. (2005, 2009) – experimental measure of causal integration in humans (magnetic stimulation + EEG). PCI distinguishes conscious states from unconscious states.

- **Application to artificial systems** : measures of causal integration in neural networks (Barrett & Seth, 2011; Luppi et al., 2022).

### The concept

Your architecture already exchanges **ignition summaries** between levels via Markov covers, and you have anti-collapse mechanisms to prevent the degeneration of latents. However, you do not measure whether the information conveyed by these summaries is **causally integrated** – that is, whether a local perturbation propagates significantly through the hierarchy.

During the **sleep phase** (artificial daydreaming), a **Φ-estimator** module is activated at level N=5 (or N=6). Its operation:

- **Selection** of a sample of past ignitions (from MeMo).

- **Perturbation**: injection of controlled Gaussian noise into certain ignition summaries (or into the internal latents) – simulating an informational micro-lesion.

- **Measurement** of the variation in the predictive error of the JEPA model (or surprise in the sense of active inference) between the original trajectory and the perturbed trajectory.

- **Calculation of a proxy Φ̂** (simplified formula):
  `Φ̂ = Var(Δ predictive error) / (σ²_noise + ε)`
  – the greater the variation, the more integrated the system is (a small perturbation greatly changes the overall dynamics).

- **Alert threshold**: if Φ̂ falls below a critical value (calibrated experimentally), the system detects an *integration collapse*: the ignitions have become too independent, the hierarchy is disintegrating.

This mechanism is **non-invasive** (performed in latent simulation) and **periodic** (for example, at the end of each sleep cycle). It does not modify real-time decisions but alerts operators or triggers corrective actions: recalibration of compression, increase in the dimension of ignition summaries, or targeted daydreaming to re-learn integration.

### Technical Justification

- **Diagnostic tool** rather than a permanent component: IIT is difficult to calculate online; in offline phases, it is feasible and useful.

- **Complements variance metrics** (anti-collapse) by adding a **causal measure**: two systems may have the same latent variance but very different integrations.

- **Predicts silent drifts**: before performance drops, Φ̂ can gradually decrease, signaling a weakening of functional consciousness.

- **Aligned with the literature**: Recent studies (Luppi et al., 2022) show that Φ̂ correlates with the performance of deep networks on integration tasks.

### Diagram

```mermaid
flowchart TD
    subgraph Sleep ["Sleep Phase (JEPA Daydreaming)"]
        A["Loading a batch of ignitions\n(MeMo memories)"]
        B["Injecting noise\n(local perturbation)"]
        C["Calculating predictive error\nbefore/after perturbation"]
        D["Φ̂ = Var(Δ error) / (σ²_noise+ε)"]
    end

    subgraph Alert ["Decision"]
        E{Φ̂ < threshold ?}
        F["OK: satisfactory integration"]
        G["Alert: integration collapse\n(corrective actions)"]
    end

    A --> B --> C --> D --> E
    E -->|no| F
    E -->|yes| G

    G --> H["Possible actions:\n- Increase summary size\n- Recalibrate compression\n- Enriched daydreaming"]

    style D fill:#ffebee,stroke:#c62828
    style G fill:#ffcdd2
```

### Concrete example: drift of an officer

The N=5 level (Group) has several officers (Tactical, Intelligence, etc.). After several combat cycles, the Intelligence officer begins to ignore weak signals from N=4, as their ignition thresholds have increased in an uncoordinated manner.

During the next sleep, the Φ-estimator randomly perturbs a few ignition summaries from the Intelligence memory. The variation in the global predictive error is abnormally low: a small local perturbation changes almost nothing in the group's dynamics. Φ̂ drops below the threshold.

The alert triggers a **targeted daydream**: the system replays scenarios where Intelligence must collaborate with Tactical, forcing shared ignitions. The thresholds are recalibrated. In the end, Φ̂ rises again. The group regains its coherence.

> ✨ Translated automatically with [**Do-My-Work**](https://github.com/AlainCo/do-my-work) — a tool designed to make projects speak globally.
