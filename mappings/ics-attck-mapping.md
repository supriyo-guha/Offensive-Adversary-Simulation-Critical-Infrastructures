# Mapping to MITRE ATT&CK for ICS

## 1. Purpose of This Mapping
This document provides a **conceptual alignment** between the adversary
simulation framework and the MITRE ATT&CK® for Industrial Control Systems
(ICS) knowledge base.

The objective is to:
- contextualize IT–OT adversary behavior within ICS threat models,
- analyze cyber–physical risk pathways,
- support academic reasoning about critical infrastructure security.

This mapping does not simulate physical harm or device manipulation.

---

## 2. Scope and Constraints
ATT&CK for ICS focuses on adversary behavior targeting operational
environments. This research extends that perspective by:

- modeling **enterprise-to-OT transitions**,
- emphasizing mediated access paths,
- focusing on decision-layer and organizational constraints.

Mappings are therefore **high-level and analytical**.

---

## 3. Conceptual Mapping by ICS Attack Phase

### 3.1 Initial Access (ICS Context)
**ATT&CK for ICS Tactic:** Initial Access

Initial access to ICS environments is modeled as the result of **IT-side
compromise combined with trust-based mediation**, rather than direct
interaction with field devices.

**Mapped behaviors (conceptual):**
- access via intermediary systems,
- dependence on authorized operational workflows,
- policy-controlled entry points.

---

### 3.2 Lateral Movement Within OT
**ATT&CK for ICS Tactic:** Lateral Movement

Lateral movement in the OT environment is constrained by safety,
availability, and reliability requirements. The model emphasizes careful
navigation rather than rapid expansion.

**Mapped behaviors (conceptual):**
- movement through operationally approved paths,
- avoidance of disruptive actions,
- sensitivity to process stability.

---

### 3.3 Inhibit Response Function
**ATT&CK for ICS Tactic:** Inhibit Response Function

Rather than manipulating devices directly, the adversary is modeled as
impacting **visibility and response capability** at an abstract level.

**Mapped behaviors (conceptual):**
- degradation of monitoring effectiveness,
- delayed or impaired situational awareness,
- interference with response decision-making.

---

### 3.4 Impact (ICS)
**ATT&CK for ICS Tactic:** Impact

Impact in ICS environments is framed as **cyber–physical risk
realization**, including disruption of operational continuity and
potential safety implications.

This research avoids simulation of physical damage and instead focuses
on analytical understanding.

**Mapped behaviors (conceptual):**
- process disruption,
- operational downtime,
- indirect physical consequences.

---

## 4. Summary Mapping Table (ICS)

| Research Phase              | ATT&CK for ICS Tactic      | Conceptual Mapping Focus              |
|----------------------------|----------------------------|---------------------------------------|
| IT–OT Transition           | Initial Access             | Mediated operational entry            |
| OT Navigation              | Lateral Movement           | Safety-aware movement                 |
| Visibility Degradation     | Inhibit Response Function  | Loss of situational awareness         |
| Cyber–Physical Consequence | Impact                     | Operational and safety risk           |

---

## 5. Research Implications
This mapping demonstrates that the proposed framework:

- reflects observed ICS adversary behavior without device-level detail,
- bridges enterprise and ICS threat models,
- supports doctoral research into cyber–physical risk pathways.

---

## 6. Ethical and Safety Considerations
This document intentionally excludes:
- device-specific commands,
- protocol manipulation,
- physical process interaction.

The focus remains on **behavioral modeling and academic analysis** in
compliance with ethical research standards.
