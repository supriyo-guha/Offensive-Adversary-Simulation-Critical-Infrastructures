# Threat Model Assumptions

## Purpose of the Threat Model
This document defines the threat model used throughout this repository to support **controlled, ethical adversary simulation research**. The model does not represent any specific real-world actor; instead, it abstracts **classes of adversary behavior** relevant to the study of critical infrastructure security.

A clearly articulated threat model is necessary to ensure:
- methodological clarity,
- ethical containment,
- and reproducibility across academic research efforts.

---

## Adversary Characterization
The modeled adversary represents a **well-resourced, persistent external threat actor** operating without insider privileges. The adversary is assumed to possess:

- proficiency in enterprise IT environments,
- familiarity with identity and access management systems,
- understanding of segmented network architectures,
- awareness of operational technology (OT) environments,
- and a preference for stealth, persistence, and long-term access.

The adversary’s objective is **situational awareness and potential operational influence**, rather than immediate disruption, destruction, or financial gain.

---

## Capability Assumptions
The adversary is assumed to operate using:

- publicly documented techniques and known misconfigurations,
- chained low-complexity actions leading to higher-level outcomes,
- adaptive behavior in response to environmental constraints,
- knowledge of standard industrial security practices (e.g., zoning and
  conduits).

The adversary **does not rely on unknown vulnerabilities, zero-day exploits, or proprietary access**.

---

## Initial Access Assumptions
Initial access is constrained to **non-destructive, realistic vectors**, including:

- trust abuse and user interaction,
- credential exposure or reuse,
- misconfigured access pathways.

Zero-day exploitation, hardware compromise, and physical access are explicitly excluded to preserve academic validity and ethical safety.

---

## Environmental Assumptions
The modeled environment assumes:

- enforced network segmentation between IT and OT domains,
- firewall-mediated access control,
- the presence of logging and monitoring mechanisms (not evaluated in depth),
- standard enterprise identity and authentication services.

These assumptions represent a **baseline industrial security posture**, rather than worst-case or intentionally vulnerable configurations.

---

## Explicit Exclusions
The following are explicitly out of scope for this research:

- insider threats,
- supply-chain compromise,
- safety-system sabotage,
- destructive or irreversible actions,
- real-world infrastructure targeting.

These exclusions are intentional and align with responsible security research norms.

---

## Role of the Threat Model in This Research This threat model functions as a **research scaffold**. All architectural designs, adversary lifecycle models, and analytical conclusions in this repository are valid **only within the bounds of these assumptions**.

Any extension or reuse of this work should explicitly document deviations from this threat model to maintain methodological transparency.
