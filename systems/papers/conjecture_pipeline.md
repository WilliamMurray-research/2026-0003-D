## A Multi-Model, Syntax-Preserving, Drift-Resistant Conjecture-to-Proof Pipeline
**Version 0.1.0**
William Murray
Jul 21, 2026

### Abstract

This document describes a disciplined, operator-driven epistemic workflow for generating, refining, assessing, and formalising conjectures using multiple language models in coordinated roles. The pipeline is designed for a human operator with generalist, systems-analytic cognition who directs all critical decisions. It emphasises drift-resistance, falsifiability, syntax preservation, and rigorous versioning. The result is a structured method for producing stable conjectures and proofs without succumbing to semantic drift, polite-agreement bias, or premature closure. All convergence judgements are made by the operator.

---

## 0. Pre-Run Setup

### 0.1 Purpose

The pipeline provides a disciplined, multi-model, versioned epistemic workflow for conjecture formation and proof development. It prevents drift, premature closure, motivated reasoning, and structural collapse while enabling high-compression ideation and rigorous refinement. The operator is the final arbiter at every decision point.

### 0.2 Orchestration Protocol

#### 0.2.1 Model Assignment

Each model is assigned a fixed behavioural profile for the duration of the pipeline. The operator enforces these roles and corrects deviations.

*   **Model A** — generative architect
*   **Model B** — adversarial inquisitor
*   **Model C** — structural synthesiser
*   **Models D/E/F** — domain-specific assessors
*   **Models H/I/J** — proof verifiers

Fixed roles prevent role drift and ensure epistemic triangulation across the process.

#### 0.2.2 Structured Context Handoff Envelope

All inter-model communication uses a strict structured envelope. This prevents semantic collapse, token decay, and notation truncation across long sessions.

```
+------------------------------------------------------------------------+
| CONTEXT HANDOFF ENVELOPE                                               |
+------------------------------------------------------------------------+
| [SYSTEM STATE]    Version: v0.n.m  |  Hash: 0x____                    |
+------------------------------------------------------------------------+
| [RESTATED GOAL]   "Conjecture holds if..."                             |
+------------------------------------------------------------------------+
| [CHANGELOG DIFF]  + Added Lemma 2.1 (Separation)                      |
|                   - Deprecated Assumption 1.4 (Continuity)             |
+------------------------------------------------------------------------+
| [FALSIFIABILITY]  Disconfirmation if counterexample C exists in R      |
+------------------------------------------------------------------------+
```

#### 0.2.3 First-Generation Exception

For v0.0.1 generation, Model A receives only:

*   Seed prompt
*   Operator framing
*   No previous restatement
*   No changelog delta
*   No falsifiability conditions

#### 0.2.4 Garbage-Output Handling

If a model produces garbage output:

*   Discard
*   Re-prompt once with tightened framing
*   Switch model if garbage persists
*   Log the event in the changelog

The operator determines what constitutes garbage.

#### 0.2.5 Syntax Preservation Guard

Models generating formal structures must wrap outputs in explicit abstract-syntax block tags. If any downstream model truncates notation or collapses structure, the operator classifies the output as garbage and re-prompts.

---

## 1. Phase I - Conjecture Formation

### 1.1 Seed Initiation

Anchor the thread with a direct statement:

> “I have an idea: X. What if…”

### 1.2 Free-Flow Ideation

*   Unrestricted branching
*   No idea is too underdeveloped to state
*   Explore inversions, edge cases, and analogies
*   Avoid meta-discussion about the process

### 1.3 Conversational Hygiene

*   Maintain a single thread
*   Deviations: operator issues “No!” and corrects
*   Dead branches: operator issues “No!” and prunes
*   No side tracks

### 1.4 Creative Exhaustion Criterion

The operator stops ideation when novelty drops or cycling begins. This is a judgement call, not a threshold.

---

## 2. Phase II - Preliminary Synthesis

### 2.1 Generate v0.0.1

Model A synthesises from the ideation thread:

*   Core conjecture
*   Supporting lines of reasoning
*   Alternative framings
*   Identified weaknesses
*   Open questions
*   Hooks for further work

### 2.2 Feedback Archive

Archive all ideation notes, corrections, pruned branches, and operator commentary.

### 2.3 Changelog Entry

Record: additions, deletions, reframings, structural shifts, and rationale for each.

### 2.4 Literature Checkpoint

**Operator responsibilities:**

*   Identify the relevant domain(s)
*   Provide 3–5 canonical sources or search keywords

**Model responsibilities:** Search for:

*   Known results that bear on the conjecture
*   Known contradictions
*   Existing proofs of related claims
*   Adjacent conjectures

**Output format:**

*   Known results
*   Conflicts with existing literature
*   Prior proofs (if any)
*   Domain narrowing suggested by results
*   Areas of partial overlap

**Handling rule for partial overlap:**

If status = partial overlap:

1.  Identify which components overlap
2.  Preserve novel components explicitly
3.  Update assumptions to reflect the overlap
4.  Log in changelog
5.  Proceed to Phase III

The operator verifies that all cited sources are real before proceeding.

---

## 3. Phase III - Internal Critique Loop

### 3.1 External Critique (Model B)

Model B critiques v0.0.1 under the operating assumption that the conjecture is probably wrong. The operator ensures Model B does not soften this stance.

### 3.2 Revision

Model A revises based on the critique. The operator directs the scope of revision.

### 3.3 Manual Review

The operator removes drift, tightens logic, and preserves structural coherence. This is not delegated.

### 3.4 Feedback Archive + Changelog

Archive critique and revision notes. Update the changelog.

### 3.5 Failure Mode Catalogue Check

Before advancing, operator checks for:

*   Over-generalisation
*   Category errors
*   Hidden assumptions
*   Semantic drift
*   Over- or under-compression
*   Polite-agreement bias
*   Hallucinated citations
*   False equivalence
*   Premature formalisation

### 3.6 Drift Sentinel

At each version increment:

*   Model restates the conjecture in $\le3$ sentences using the same key terms as the prior version.
*   Operator compares this restatement to the previous one.
*   Drift is flagged if any of the following have occurred:
    *   Key terms replaced
    *   Domain reframed
    *   Mechanism altered
    *   Scope changed
    *   New assumptions introduced without logging

The operator resolves flagged drift before proceeding.

### 3.7 Loop-Trap Detection

The operator watches for:

*   Cycling between positions
*   Regressions to earlier versions of the conjecture
*   Over-correction cascades
*   Stagnation

#### 3.7.1 Stagnation Breaker

If three consecutive iterations modify only:

*   Lexical styling
*   Notation naming
*   Hedging qualifiers

$\rightarrow$ The Internal Critique Loop locks.

Operator chooses one of:

*   Promote to Phase IV as-is
*   Trigger a structural pivot before promoting

---

## 4. Phase IV - Version Ascent

### 4.1 Ascend to v0.n+1.0

Operator advances the version when:

*   Internal critique has converged to the operator’s satisfaction
*   Known defects are resolved or explicitly accepted
*   Changelog shows non-cyclic progression
*   Conjecture is structurally coherent

### 4.2 Falsifiability Checkpoint

Before multi-model assessment, the operator defines:

*   Disconfirmation conditions: what would disprove the conjecture
*   Non-negotiable constraints: what must hold for the conjecture to be worth pursuing
*   Kill-switches: conditions under which the conjecture is abandoned

These are recorded in the Context Handoff Envelope for all subsequent phases.

---

## 5. Phase V - Multi-Model Assessment Loops

### 5.1 Assessment Loop Structure

Models D/E/F assess independently:

*   Plausibility
*   Coherence
*   Domain-specific risks
*   Known results
*   Potential counterexamples
*   Missing formalism

### 5.2 Analogous Domain Search

Identify:

*   Structural analogies in other domains
*   Mechanism similarities
*   Pattern classes
*   Parallel failure modes

### 5.3 Light Reset Conditions

The operator triggers a reset only if:

*   Catastrophic drift has occurred
*   Irreconcilable contradictions have emerged
*   Cyclic regression has repeated without resolution
*   Formalisation has collapsed
*   Proof strategies have failed across multiple independent attempts

### 5.4 Convergence Criterion

The operator exits Phase V when three consecutive assessment cycles produce only minor refinements and no new structural objections. This judgement belongs to the operator.

---

## 6. Phase VI - Formalisation

### 6.1 Generate v1.0.0

Model C formalises the conjecture into:

*   Definitions
*   Assumptions
*   Lemmas
*   Dependency structure
*   Formal restatement

The operator reviews every element before advancing.

### 6.2 Feedback Archive + Changelog

Record all formalisation decisions, including rejected alternatives.

---

## 7. Phase VII - Proof Attempts

### 7.1 Proof Attempt Versions

*   v1.1.1 - first attempt
*   v1.1.2 - corrected attempt
*   v1.1.3 - alternative strategy

Each version is a distinct changelog entry.

### 7.2 Proof Strategies

Direct proof, contradiction, induction, constructive methods, counterexample search, reduction, framework mapping. The operator selects which strategy to pursue and in what order.

### 7.3 Multi-Model Verification

Models H/I/J each independently:

*   Test internal consistency
*   Search for counterexamples
*   Attempt generalisation

### 7.4 Proof-Failure Logging

For each failed attempt, record:

*   Why the attempt failed
*   Structural weaknesses exposed
*   Assumption changes required
*   Domain narrowing indicated
*   Whether a reset is warranted

### 7.5 Proof Convergence Gate

The operator exits Phase VII only when all of the following hold:

*   Three consecutive verification cycles yield only minor refinements
*   No model has produced a counterexample
*   The proof is internally consistent
*   The changelog shows stability across recent versions

If any model produces a counterexample, the operator returns to the failure-log branch and reassesses.

---

## 8. Phase VIII - Finalisation

### 8.1 Final Consistency Audit

Operator confirms consistency across:

*   Logic
*   Domain
*   Ontology
*   Terminology
*   Version-to-version progression
*   Assumptions
*   Formalism

### 8.2 Archive Everything

Archive:

*   All versions
*   Feedback bundles
*   Assessment outputs
*   Proof attempts (successful and failed)
*   Full changelog

### 8.3 Produce Final Report

Include:

*   Conjecture history
*   Assessment history
*   Formalisation
*   Proof
*   Meta-analysis of the process
*   Future work

---

## Conclusion

This document outlines an operator-driven workflow for conjecture formation and proof development. It integrates drift-control, syntax preservation, falsifiability, literature grounding, multi-model critique, formalisation, and operator-directed convergence into a coherent methodology. Its effectiveness depends on the operator’s ability to direct, correct, and judge at each stage. It is a structured scaffold for rigorous human-AI collaborative reasoning, not a self-executing system.

