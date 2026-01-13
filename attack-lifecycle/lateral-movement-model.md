# Lateral Movement Model

## 1. Conceptual Definition
Lateral movement is defined as adversary behavior that expands influence across systems or roles **with and without escalating privilege vertically**.

In critical infrastructure environments, lateral movement is primarily a function of **trust relationships**, not network reachability.

---

## 2. Identity-Centric Movement
The model emphasizes identity and authorization as the dominant enablers of lateral movement. Access expansion occurs through:
- reuse of existing trust,
- delegated privileges,
- and shared operational dependencies.

This reflects modern enterprise environments where network isolation
alone is insufficient.

---

## 3. Segmentation-Aware Movement
Segmentation shapes lateral movement by:
- limiting available paths,
- increasing dependency on approved conduits,
- and forcing adversaries to adapt movement strategies.

The adversary is modeled as identifying **least-resistance pathways** that align with legitimate use.

---

## 4. Behavioral States
Lateral movement is modeled as transitions between:
- single-system influence,
- multi-system influence within a trust zone,
- and cross-zone influence through mediated access.

Each transition increases capability while also increasing risk.

---

## 5. Research Implications
This abstraction supports analysis of:
- which trust edges enable disproportionate adversary expansion,
- how segmentation policies affect attack feasibility,
- and how identity governance alters movement patterns.

---

## 6. Ethical Framing
The repository avoids operational guidance. Lateral movement is represented as a **state expansion problem**, suitable for formal analysis and simulation.
