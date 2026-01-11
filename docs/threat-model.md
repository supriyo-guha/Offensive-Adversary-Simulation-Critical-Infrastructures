# Threat Model Assumptions

## Purpose of the Threat Model
This document defines the threat model used throughout this repository to support **controlled, ethical adversary simulation research**. The purpose of the threat model is not to represent any specific real-world actor, but to abstract **classes of adversary behaviors** relevant to critical infrastructure security research.

A clearly defined threat model is essential to ensure:
- methodological consistency,
- ethical boundaries,
- reproducibility across academic studies.

---

## Adversary Characterization
The simulated adversary represents a **well-resourced, persistent external threat actor** operating without insider privileges. The adversary is assumed to possess:

- Proficiency in enterprise IT environments
- Familiarity with identity and access management systems
- Understanding of segmented network architectures
- Awareness of operational technology (OT) environments
- Emphasis on stealth, persistence, and long-term access

The adversary’s objective is **situational awareness and operational influence** rather than immediate disruption or financial gain.

---

## Capability Assumptions
The adversary is assumed to have the following capabilities:

- Use of publicly documented techniques and misconfigurations
- Ability to chain multiple low-complexity actions into higher-impact outcomes
- Capability to adapt behavior in response to environmental constraints
- Knowledge of standard industrial security practices (e.g., zoning and conduits)

The adversary **does not** rely on unknown vulnerabilities or proprietary access.

---

## Initial Access Assumptions
Initial access is constrained to **non-destructive and realistic vectors**, including:

- User interaction and trust abuse
- Credential exposure or reuse
- Misconfigured access pathways

Zero-day exploitation, hardware compromise, and physical access are explicitly excluded to maintain academic and ethical validity.

---

## Environmental Assumptions
The modeled environment assumes:

- Proper network segmentation between IT and OT domains
- Firewall-enforced access control
- Logging and monitoring infrastructure present but not analyzed in depth
- Standard enterprise identity services

These assumptions reflect **baseline industrial security posture**, not worst-case misconfiguration.

---

## Explicit Exclusions
The following are out of scope:

- Insider threats
- Supply-chain compromise
- Safety-system sabotage
- Destructive or irreversible actions
- Real-world infrastructure targeting

These exclusions are intentional to align with responsible research norms.

---

## Role of the Threat Model in This Research
This threat model serves as a **research scaffold**. All architectural designs,
attack lifecycle models, and analytical conclusions in this repository are
interpreted **only within the bounds of these assumptions**.

Any extension or reuse of this work should explicitly state deviations from this model.
