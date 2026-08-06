# Mathematics Curriculum for the Unified Operator Architecture Corpus

This corpus sits at the intersection of **dynamical systems, symplectic geometry, symbolic dynamics, domain theory, and transfinite topology**. Below is a structured curriculum organized by dependency layers, with concrete resources, time estimates, and milestone checkpoints.

---

## Phase 0: Prerequisites (Foundation — 2–3 months)

| Area | Core Topics | Standard Texts | Target Competency |
| :--- | :--- | :--- | :--- |
| **Real Analysis & Metric Spaces** | Completeness, compactness, Baire category, uniform spaces | Rudin *Principles* Ch. 1–3, 7; Bourbaki *General Topology* Ch. 1–2 | Prove Banach fixed-point; work in uniform spaces |
| **Linear Algebra & Functional Analysis** | Banach/Hilbert spaces, operators, spectral theory | Axler *Linear Algebra Done Right*; Conway *Functional Analysis* Ch. 1–4 | Spectral gap arguments; operator norms |
| **General Topology** | Product topology, Tychonoff, ultrametrics, Cantor space | Munkres *Topology* Ch. 2–4, 7; Willard *General Topology* | Cantor space homeomorphisms; ultrametric properties |
| **Abstract Algebra (Light)** | Lattices, fixed-point theorems (Tarski–Knaster), monoids | Davey & Priestley *Lattices and Order* Ch. 1–2 | Closure operators; Knaster–Tarski |
| **Measure/Information Theory (Basics)** | Entropy, mutual information, data-processing inequality | Cover & Thomas *Elements of Information Theory* Ch. 1–2, 8 | Compute $H_{Sh}$, $I(X;Y)$; DPI |

**Milestone 0:** Prove Banach contraction on compact subsets with Hausdorff metric; derive Knaster–Tarski for $\mathcal{P}(M)$; show Cantor space is homeomorphic to $\{0,1\}^\mathbb{N}$.

---

## Phase 1: Dynamical Systems & Ergodic Theory (3–4 months)

| Module | Topics | Primary Texts | Corpus Links |
| :--- | :--- | :--- | :--- |
| **1A: Smooth Dynamics** | Flows, invariant manifolds, Hartman–Grobman, stable/center/unstable manifolds | Katok & Hasselblatt *Introduction to the Modern Theory of Dynamical Systems* Ch. 1–3, 6 | A1 contraction; $I^{(1)}_*$ attractor |
| **1B: Center Manifold Theory** | Center manifold existence, reduction, finite-dim approximation | Carr *Applications of Centre Manifold Theory* Ch. 1–3; Guckenheimer & Holmes Ch. 3 | Tier-1 fast contraction; $M$ graph |
| **1C: Normal Forms & Bifurcations** | Poincaré–Dulac, Sternberg linearization, transversality | Arnold *Geometrical Methods*; Golubitsky & Schaeffer *Singularities and Groups* | A5 jet transversality; genericity |
| **1D: Ergodic Theory Basics** | Invariant measures, entropy, variational principle | Walters *Ergodic Theory* Ch. 1–4, 8 | $K_I$ complexity measure |

### Key Exercises
* Prove center manifold theorem for $\dot{x}=Ax+f(x)$ with $f(0)=Df(0)=0$
* Compute spectral gap for complete graph Laplacian ($\lambda_2 = K$)
* Construct a $C^\infty$ bump function perturbation off a submanifold (A5 proof technique)

**Milestone 1:** Read and reproduce the center-manifold derivation in `TieredEmergence` §3; verify Lemma 6.1 scaling $h_0 = O(\|\omega\|/K)$.

---

## Phase 2: Symplectic Geometry & Hamiltonian Mechanics (3–4 months)

| Module | Topics | Primary Texts | Corpus Links |
| :--- | :--- | :--- | :--- |
| **2A: Symplectic Linear Algebra** | Symplectic vector spaces, Lagrangian subspaces, Williamson normal form | McDuff & Salamon *Introduction to Symplectic Topology* Ch. 1–2 | Cotangent bundle $T^*(S^1)^N$ |
| **2B: Hamiltonian Mechanics** | Hamiltonian flows, momentum maps, Noether's theorem | Abraham & Marsden *Foundations of Mechanics* Ch. 3–4; Arnold *Mathematical Methods of Classical Mechanics* | $J = \sum p_i$; $S^1$ action |
| **2C: Symplectic Reduction** | Marsden–Weinstein quotient, coisotropic reduction, singular reduction | Marsden & Weinstein 1974 (original); Ortega & Ratiu *Momentum Maps* Ch. 6–7 | $J^{-1}(\mu)/S^1 \simeq T^*S^1$ |
| **2D: Cotangent Lifts & Embeddings** | Canonical symplectic structure, Hamiltonian embedding of dissipative systems | Bloch *Nonholonomic Mechanics* Ch. 5; Holm et al. *Geometric Mechanics* | §4 embedding $H = \sum p_i f_i + \frac12\sum p_i^2$ |

### Key Exercises
* Derive Marsden–Weinstein reduction for $T^*\mathbb{T}^N // S^1$ explicitly
* Show reduced symplectic form is $d\Theta \wedge dP$
* Verify $H_{red} = P^2/2N$ on $J^{-1}(N\bar{\omega})$

**Milestone 2:** Reproduce `TieredEmergence` §4–5 from scratch; explain why the embedding is a *device* not intrinsic property.

---

## Phase 3: Symbolic Dynamics & Combinatorics (3–4 months)

| Module | Topics | Primary Texts | Corpus Links |
| :--- | :--- | :--- | :--- |
| **3A: Shift Spaces** | Full shifts, subshifts of finite type (SFT), sofic shifts, sliding block codes | Lind & Marcus *Symbolic Dynamics and Coding* Ch. 1–3, 6–7 | $X = A^\mathbb{Z}$, $\mathcal{B}_k$, CHL theorem |
| **3B: Forbidden Patterns & Entropy** | Forbidden sets $\mathcal{F}$, topological entropy, factor maps | Lind & Marcus Ch. 4, 9; Walters Ch. 7 | Non-local subshifts; $r_{min}$ |
| **3C: Combinatorial Genericity** | Asymptotic density in $\mathcal{B}_k$, independence arguments, exponential bounds | No standard text — see `UnifiedAlgebra` §4; complement with Alon & Spencer *Probabilistic Method* Ch. 1–2 | Theorem 4.1; witness lemma |
| **3D: Even Shift & Sofic Theory** | Even shift, Fischer cover, minimal right-resolving presentations | Lind & Marcus §1.2, 3.3; Marcus *Sofic Systems* | Appendix B example; $r_{min}=3$ |

### Key Exercises
* Prove Curtis–Hedlund–Lyndon theorem
* Show even shift is sofic but not SFT; construct its Fischer cover
* Implement exhaustive enumeration of $\mathcal{B}_k$ for $k \le 3$ on binary alphabet; verify density decay

**Milestone 3:** Reproduce `UnifiedAlgebra` Theorem 4.1 proof including the v0.0.61 witness lemma; run the even-shift numerical validation (§4.5).

---

## Phase 4: Domain Theory, Order Theory & Transfinite Constructions (3–4 months)

| Module | Topics | Primary Texts | Corpus Links |
| :--- | :--- | :--- | :--- |
| **4A: Domain Theory Basics** | DCPOs, Scott topology, continuous domains, ideal completion | Abramsky & Jung *Domain Theory* (Handbook); Gierz et al. *Continuous Lattices and Domains* Ch. 1–3 | $\widehat{B}$, Scott continuity, EP-pairs |
| **4B: EP-Pairs & Embedding-Projection** | Embedding-projection pairs, retracts, coherence | Abramsky & Jung §4; Abramsky *Domain Theory in Logical Form* | Part III Coherence Axiom |
| **4C: Transfinite Constructions** | Ordinal-indexed colimits/limits, inverse limits, $\omega_1$ | Jech *Set Theory* Ch. 1–2; Adámek & Rosický *Locally Presentable Categories* | Part IV $D_\lambda = \varinjlim D_\alpha$ |
| **4D: Ultrametrics in Domain Theory** | Ultrametric domains, Smyth completion, proper ultrametrics | Majewski *Ultrametric Domains*; Weihrauch *Computable Analysis* | $C_{\mathcal{Y}}$ proper ultrametric |
| **4E: Formalization (Lean 4)** | Mathlib topology, order, metric spaces; formalizing ultrametrics | *Mathematics in Lean*; Mathlib docs `Topology.MetricSpace`, `Order.CompleteLattice` | §1.2 Lean sketch; Part X.1 |

### Key Exercises
* Prove ideal completion of a poset yields a DCPO
* Construct EP-pair between finite prefix domains and Cantor space
* Formalize proper ultrametric instance in Lean 4 (Mathlib `Dist` + `UltrametricSpace`)

**Milestone 4:** Formalize the deviation metric $C_{\mathcal{Y}}$ and prove it's a proper ultrametric in Lean 4; sketch EP-pair coherence diagram.

---

## Phase 5: Information Theory & Cross-Domain Synthesis (2–3 months)

| Module | Topics | Primary Texts | Corpus Links |
| :--- | :--- | :--- | :--- |
| **5A: Advanced Information Theory** | Fisher information, Kolmogorov complexity, rate-distortion, normalized information distance | Cover & Thomas Ch. 11, 14; Li & Vitányi *Kolmogorov Complexity* | $K_{domain}$ measures: $H_{Sh}, J_{Fisher}, K_{kol}$ |
| **5B: Quantum Information (Light)** | Von Neumann entropy, holographic entropy bounds, Ryu–Takayanagi | Wilde *Quantum Information Theory* Ch. 11; Harlow *TASI Lectures* | QG track $K$ table |
| **5C: IIT & Consciousness Measures** | $\Phi$ measures, IIT 4.0 postulates, critiques | Tononi et al. 2016 (IIT 4.0); Aaronson critique; Bayne 2018 | Consciousness track category error |
| **5D: Collective Behavior Data Analysis** | Kernel density estimation, order parameters, Cavagna starling data | Cavagna et al. 2010 PNAS; Vicsek & Zafeiris 2012 Phys Rep | Collective Biology track M5 |

### Key Exercises
* Compute normalized Fisher information for a simple quantum state
* Show $\Phi \neq I(\mathcal{Y})$ for a small Boolean network
* Estimate $K_{domain}$ from simulated Kuramoto data (reproduce `TieredEmergence` §6.3)

**Milestone 5:** Produce empirical $K$ estimate from Crazyswarm or Cavagna data (CrossDomain M4/M5).

---

## Phase 6: Specialized Advanced Topics (Parallelizable, 2–3 months each)

| Track | Topics | Key Papers | Corpus Application |
| :--- | :--- | :--- | :--- |
| **Jet Transversality** | Thom–Abraham transversality, Whitney $C^\infty$ topology, Fréchet spaces | Abraham *Transversality*; Hirsch *Differential Topology* Ch. 3 | A5 genericity proof |
| **Fenichel Theory** | Normally hyperbolic invariant manifolds, persistence | Fenichel 1971; Hirsch–Pugh–Shub 1977; Bates et al. *Invariant Manifolds* | Lemma 6.1 stable-fibre contraction |
| **Persistent Homology** | Vietoris–Rips, barcodes, stability theorem | Edelsbrunner & Harer *Computational Topology*; Chazal et al. *Persistence Theory* | Decentralized Biology $P$ |
| **Consensus/Control on Graphs** | Laplacian dynamics, distributed averaging, flocking algorithms | Olfati-Saber et al. 2007; Bullo *Lectures on Network Systems* | Swarm Engineering $B, G, C$ |
| **Ordinal Analysis** | Countable ordinals, $\omega_1$, Bachmann–Howard | Rathjen *Ordinal Analysis*; Schütte *Proof Theory* | Conjecture X.2.1 location |

---

## Integrated Learning Roadmap (18–24 Months)
