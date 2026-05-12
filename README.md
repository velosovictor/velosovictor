<div align="center">

# RationalBloks

### Deterministic Engine for Exhaustive State-Space Verification

</div>

## Overview

[cite_start]RationalBloks is an infrastructure engine designed for overcoming combinatorial explosion in high-ASIL control logic[cite: 2]. [cite_start]By replacing explicit-state simulation with a deterministic mathematical model, the engine serves as an upstream filter for architectural conflicts[cite: 102]. 

[cite_start]The core of the system is a Recursive Discrete Subtraction (RDS) algorithm that mathematically isolates unmodeled logic and rule collisions before downstream V-Cycle simulations begin[cite: 102].

### 📑 Architecture & Proof of Concept
**[View the Technical Briefing & Visual PoC (Canva)](https://canva.link/8jmspsdturwci4l)**

---

## The Verification Pipeline

The engine executes an exhaustive state-space verification through a strict sequential pipeline:

**1. State Machine Translation**
[cite_start]The engine ingests complex control logic from standard state machines and translates every state transition into explicit "when X, then Y" logic[cite: 11, 12]. [cite_start]This establishes the mathematical foundation required to generate input/output parametric tensors[cite: 13].

**2. Requirement Container Assembly**
[cite_start]The logic is assembled into containers mapped by the interdependencies between parameters[cite: 32, 33]. [cite_start]This structure handles the reality that the parameter tensor grows exponentially as parameters grow in number and size[cite: 36].

**3. Gap & Conflict Extraction**
Instead of relying on brute-force testing, the RDS algorithm isolates structural failures geometrically:
* [cite_start]**Undefined Gaps:** Isolates specific subsets of parameter combinations that were left unspecified, consolidating hundreds of thousands of missing points into a single hyperrectangle within the n-dimensional space[cite: 42, 43].
* [cite_start]**Logical Conflicts:** Systematically isolates logical contradictions into finite, manageable blocks, instantly revealing engineering rules that collide[cite: 93, 96].

---

## ISO 26262 Compliance Architecture

[cite_start]The RDS engine functions as a continuous mathematical bridge across the verification lifecycle[cite: 5]:

* [cite_start]**Part 4 (System Level):** Analyzes MBSE state machines to mathematically isolate unmodeled logic strictly during the pre-implementation phase[cite: 6].
* [cite_start]**Part 6 (Software Level):** Applies exhaustive formal verification to prove high-ASIL software units are free of hidden failure modes, preventing architectural flaws from bleeding into the codebase[cite: 7].
* [cite_start]**Part 8 (Supporting Processes):** Automates the extraction of boundary blocks, generating the exact, deterministic verification artifacts required by the standard[cite: 8].
* [cite_start]**Part 9 (Safety Analyses):** Provides the definitive mathematical foundation for risk assessment, ensuring perfectly clean data for Fault Tree and FMEA execution[cite: 9].

---

<div align="center">

**Architected by Victor Veloso Assunção** *Mechanical Engineer | Systems Engineering* [cite: 110, 111]

</div>
