# Mapping to MITRE ATT&CK (Enterprise)

## 1. Purpose of This Mapping
This document provides a structured, **non-operational alignment**
between the adversary simulation framework developed in this repository
and the MITRE ATT&CK® (Enterprise) knowledge base.

The purpose of this mapping is to:
- contextualize the research within an established threat taxonomy,
- enable analytical comparison with documented adversary behavior,
- demonstrate coverage of the enterprise attack surface,
- support academic discussion without enabling misuse.

This mapping is **behavior-centric**, not technique-driven.

---

## 2. Methodology and Scope
MITRE ATT&CK enumerates tactics and techniques observed in real-world
intrusions. In contrast, this research focuses on:

- adversary **decision logic**,
- **trust-boundary traversal**,
- lifecycle-level progression,
- operational security (OpSec) constraints.

Accordingly:
- mappings emphasize **tactics and high-level technique classes**,
- no tools, exploits, commands, or procedures are referenced,
- focus remains on *why* behaviors occur rather than *how* they are executed.

---

## 3. Conceptual Mapping by Attack Phase

### 3.1 Reconnaissance
**ATT&CK Tactic:** Reconnaissance

Reconnaissance in this research is modeled as a **continuous activity**
rather than a discrete pre-compromise phase. It aligns with ATT&CK’s
reconnaissance tactic but extends it by incorporating trust inference
and organizational context.

**Mapped behaviors (conceptual):**
- information gathering for organizational understanding,
- identification of externally visible dependencies,
- inference of trust relationships and access patterns.

---

### 3.2 Initial Access
**ATT&CK Tactic:** Initial Access

Initial access is modeled primarily as **trust abuse** rather than
technical exploitation alone. This aligns with multiple ATT&CK initial
access categories without enumerating specific techniques.

**Mapped behaviors (conceptual):**
- misuse of legitimate access paths,
- exploitation of organizational workflows,
- dependency on identity and role-based access.

---

### 3.3 Execution and Persistence
**ATT&CK Tactics:** Execution, Persistence

Execution and persistence are treated as **presence management
strategies** influenced by OpSec considerations. The model abstracts
away execution mechanisms and focuses on persistence decisions under
detection pressure.

**Mapped behaviors (conceptual):**
- ephemeral versus durable presence,
- selective persistence to reduce observability,
- lifecycle continuity planning.

---

### 3.4 Privilege Escalation and Lateral Movement
**ATT&CK Tactics:** Privilege Escalation, Lateral Movement

These phases are represented as **trust expansion processes**, where the
adversary navigates role hierarchies and access mediation mechanisms.

**Mapped behaviors (conceptual):**
- role and permission abuse,
- movement along existing trust relationships,
- constrained navigation under segmentation policies.

---

### 3.5 Command and Control
**ATT&CK Tactic:** Command and Control

Command and control behavior is abstracted as a **communication risk
surface**, focusing on how adversaries balance responsiveness and
stealth.

**Mapped behaviors (conceptual):**
- adaptive communication behavior,
- reliance on trusted or permitted infrastructure,
- risk-aware signaling strategies.

---

### 3.6 Impact
**ATT&CK Tactic:** Impact

Impact is treated as a **decision outcome**, not merely a terminal
action. This aligns with ATT&CK’s impact tactic while emphasizing
organizational and operational consequences.

**Mapped behaviors (conceptual):**
- operational disruption,
- data or service availability impact,
- cascading organizational effects.

---

## 4. Summary Mapping Table (Enterprise)

| Research Phase               | ATT&CK Tactic(s)           | Conceptual Mapping Focus              |
|-----------------------------|----------------------------|---------------------------------------|
| Continuous Reconnaissance   | Reconnaissance             | Context and trust inference           |
| Trust-Based Entry           | Initial Access             | Legitimate access abuse               |
| Presence Management         | Execution, Persistence     | OpSec-driven lifecycle continuity     |
| Trust Expansion             | Privilege Escalation       | Role and identity abuse               |
| Internal Navigation         | Lateral Movement           | Segmentation-aware movement           |
| Communication Management    | Command and Control        | Risk-aware signaling                  |
| Outcome Realization         | Impact                     | Organizational disruption             |

---

## 5. Research Implications
This mapping demonstrates that the proposed adversary simulation:

- aligns with empirically observed enterprise attack behavior,
- extends ATT&CK by modeling **decision-making and trust dynamics**,
- complements ATT&CK without duplicating its technique catalog.

---

## 6. Ethical Boundary
This document intentionally avoids:
- technique identifiers,
- procedural detail,
- tool or exploit references.

The mapping is provided solely to support **academic analysis and
doctoral research**.
