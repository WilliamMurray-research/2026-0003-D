# Unified Operator Architecture Mathematics Curriculum    
v0.0.2 

**Date:** 2026‑08‑06  

---

## **Phase 0: Prerequisites (Foundation — 4–6 months)**

| Area | Core Topics | Standard Texts | Target Competency |
| :--- | :--- | :--- | :--- |
| **Real Analysis & Metric Spaces** | Completeness, compactness, uniform spaces, contraction operators | Rudin *Principles* Ch. 1–3, 7; Bourbaki *General Topology* | Banach fixed-point; operator contraction arguments |
| **Linear Algebra & Functional Analysis** | Banach/Hilbert spaces, spectral theory, operator norms | Axler; Conway Ch. 1–4 | Spectral gap; bounded linear operators |
| **General Topology** | Product topology, ultrametrics, Cantor space | Munkres; Willard | Cantor space operators; ultrametric continuity |
| **Abstract Algebra (Light)** | Lattices, closure operators, fixed points | Davey & Priestley | Knaster–Tarski; closure operators |
| **Measure/Information Theory (Basics)** | Shannon entropy, mutual information | Cover & Thomas Ch. 1–2 | Compute $H_{Sh}$, $I(X;Y)$ |

**Milestone 0:** Prove Banach contraction on compact subsets; derive Knaster–Tarski; show Cantor space ≅ $\{0,1\}^\mathbb{N}$.

---

## **Phase 0.5: Differential Geometry Primer (1–2 months)**  
*(New in v0.0.2)*

| Area | Topics | Texts | Competency |
| :--- | :--- | :--- | :--- |
| **Manifolds** | Charts, atlases, tangent bundles | Lee *Introduction to Smooth Manifolds* | Work with flows on manifolds |
| **Differential Forms** | Exterior calculus, symplectic forms | Lee; Tu *Differential Geometry* | Understand $ω$, $dω$, Hamiltonian vector fields |

**Milestone 0.5:** Compute symplectic form on $T^*\mathbb{R}^n$ and verify non-degeneracy.

---

## **Phase 1: Dynamical Systems & Ergodic Theory (4–6 months)**

| Module | Topics | Primary Texts | Corpus Links |
| :--- | :--- | :--- | :--- |
| **1A: Smooth Dynamics** | Flows, invariant manifolds, Hartman–Grobman | Katok & Hasselblatt Ch. 1–3 | A1 contraction |
| **1B: Center Manifold Theory** | Existence, reduction | Carr Ch. 1–3 | Tier-1 contraction |
| **1C: Normal Forms & Bifurcations** | Poincaré–Dulac, Sternberg | Arnold; Golubitsky–Schaeffer | A5 jet transversality |
| **1D: Ergodic Theory Basics** | Invariant measures, entropy | Walters Ch. 1–4 | $K_I$ complexity |

**Operator Spine Additions (New):**  
- Koopman operator basics  
- Transfer operators for expanding maps  

**Milestone 1:** Reproduce center-manifold derivation; verify Lemma 6.1 scaling.

---

## **Phase 2: Symplectic Geometry & Hamiltonian Mechanics (4–6 months)**

| Module | Topics | Primary Texts | Corpus Links |
| :--- | :--- | :--- | :--- |
| **2A: Symplectic Linear Algebra** | Lagrangian subspaces, Williamson form | McDuff & Salamon Ch. 1–2 | $T^*(S^1)^N$ |
| **2B: Hamiltonian Mechanics** | Hamiltonian flows, momentum maps | Abraham & Marsden; Arnold | $J = \sum p_i$ |
| **2C: Symplectic Reduction** | Marsden–Weinstein quotient | Ortega & Ratiu | $J^{-1}(\mu)/S^1$ |
| **2D: Cotangent Lifts & Embeddings** | Hamiltonian embedding of dissipative systems | Bloch; Holm | §4 embedding |

**Operator Spine Additions (New):**  
- Hamiltonian operators  
- Symplectic transfer operators  

**Milestone 2:** Reproduce `TieredEmergence` §4–5; explain embedding as device.

---

## **Phase 3: Symbolic Dynamics & Combinatorics (4–5 months)**

| Module | Topics | Primary Texts | Corpus Links |
| :--- | :--- | :--- | :--- |
| **3A: Shift Spaces** | SFTs, sofic shifts, sliding block codes | Lind & Marcus Ch. 1–3 | CHL theorem |
| **3B: Forbidden Patterns & Entropy** | Forbidden sets, entropy | Lind & Marcus Ch. 4, 9 | $r_{min}$ |
| **3C: Combinatorial Genericity** | Density, independence, exponential bounds | UnifiedAlgebra §4; Alon–Spencer | Witness lemma |
| **3D: Even Shift & Sofic Theory** | Fischer cover, right-resolving | Lind & Marcus | Appendix B |

**Operator Spine Additions (New):**  
- Markov operators on symbolic spaces  
- Ruelle–Perron–Frobenius operator for SFTs  

**Milestone 3:** Reproduce Theorem 4.1; run even-shift numerical validation.

---

## **Phase 4: Domain Theory, Order Theory & Ultrametrics (6–9 months)**  
*(Rebalanced in v0.0.2)*

| Module | Topics | Primary Texts | Corpus Links |
| :--- | :--- | :--- | :--- |
| **4A: Domain Theory Basics** | DCPOs, Scott topology | Abramsky & Jung; Gierz et al. | $\widehat{B}$ |
| **4B: EP-Pairs & Retracts** | Embedding-projection pairs | Abramsky §4 | Coherence axiom |
| **4C: Ultrametrics & Completion** | Smyth completion, proper ultrametrics | Majewski; Weihrauch | $C_{\mathcal{Y}}$ |
| **4D: Lean Formalization** | Mathlib topology/order; ultrametrics | *Mathematics in Lean* | Part X.1 |

**Operator Spine Additions (New):**  
- Fixed-point operators in DCPOs  
- Ultrametric contraction operators  
- Domain-theoretic semantics of dynamical operators  

**Milestone 4:** Formalize deviation metric $C_{\mathcal{Y}}$ as proper ultrametric; sketch EP-pair coherence.

---

## **Phase 5: Information Theory & Cross-Domain Synthesis (4–6 months)**

| Module | Topics | Primary Texts | Corpus Links |
| :--- | :--- | :--- | :--- |
| **5A: Advanced Information Theory** | Fisher info, Kolmogorov complexity | Cover & Thomas; Li & Vitányi | $K_{domain}$ |
| **5B: Quantum Information (Light)** | Von Neumann entropy | Wilde; Harlow | QG track |
| **5C: IIT & Consciousness Measures** | $\Phi$ measures, critiques | Tononi; Aaronson | Category error |
| **5D: Collective Behavior Data Analysis** | KDE, order parameters | Cavagna et al.; Vicsek | M5 |

**Operator Spine Additions (New):**  
- Information operators  
- Complexity operators  
- Fisher-information operators  

**Milestone 5:** Produce empirical $K$ estimate from Crazyswarm/Cavagna data.

---

## **Phase 6: Specialized Advanced Topics (Optional Tracks — 2–3 months each)**  
*(Now optional in v0.0.2)*

| Track | Topics | Key Papers | Corpus Application |
| :--- | :--- | :--- | :--- |
| **Jet Transversality** | Thom–Abraham, Whitney topology | Abraham; Hirsch | A5 genericity |
| **Fenichel Theory** | Normally hyperbolic manifolds | Fenichel; HPS | Lemma 6.1 |
| **Persistent Homology** | Barcodes, stability | Edelsbrunner–Harer | Biology $P$ |
| **Consensus/Control** | Laplacian dynamics | Olfati-Saber; Bullo | Swarm $B,G,C$ |
| **Ordinal Analysis** | $\omega_1$, Bachmann–Howard | Rathjen; Schütte | Conjecture X.2.1 |

---

## **Integrated Learning Roadmap (26–36 Months)**  
*(Updated timeline)*

---

