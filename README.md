# Offensive Adversary Simulation on Critical Infrastructures

## Abstract
This repository presents an **academic adversary simulation framework** for the ethical study of **offensive cyber operations targeting critical infrastructure environments**. The work emphasizes **adversary behavior modeling, attack lifecycle abstraction, and IT–OT interaction analysis**, rather than exploit development or operational tooling.

This repository is derived from an M.Tech (Cyber Security) dissertation and is structured to support **doctoral (PhD) research** in Red Teaming and Adversary Simulation.

---

## Research Contributions
This repository makes the following **research contributions**:

- Proposes a **behavior-centric adversary simulation framework** for
  critical infrastructure environments, abstracting adversary actions
  as decision-driven lifecycle states rather than procedural attack
  steps.

- Introduces **trust-boundary–oriented modeling** to analyze adversary
  movement across segmented enterprise IT and operational technology
  (OT) environments.

- Treats **operational security (OpSec)** as a first-class research
  variable, modeling trade-offs between stealth, persistence, and
  detection risk.

- Provides an **ethically safe abstraction layer** derived from a
  practical and implementation-driven M.Tech dissertation, enabling
  academic reuse without exposing operational attack code.

These contributions are intended to support reproducible, analytical,
and doctoral-level research into adversary behavior and cyber–physical
risk.

---

## Research Motivation
The increasing convergence of Information Technology (IT) and Operational Technology (OT) has expanded the attack surface of critical infrastructure systems. While defensive mechanisms and incident response strategies are widely studied, **controlled offensive simulations that model realistic adversary behavior across segmented IT–OT environments remain limited in academic literature**.

This work frames **offensive simulation as a research methodology**, enabling systematic analysis of trust abuse, attack progression, and cyber–physical risk under clearly defined ethical and institutional constraints.

---

## Repository Organization
The repository is organized into research-focused components:

- `research-notes/` — literature review and research gap analysis  
- `lab-infra-designs/` — system architecture and segmentation rationale  
- `attack-lifecycle/` — adversary behavior and lifecycle modeling  
- `opsec/` — operational security as a research variable  
- `mappings/` — alignment with MITRE ATT&CK and ATT&CK for ICS  
- `docs/` — threat model, ethics, research questions, and usage guidance  
- `citation/` — citation metadata for academic reuse  

---

## Intended Audience
This repository is intended for:
- PhD supervisors and research committees
- Doctoral and postgraduate researchers
- Cyber Security researchers studying adversary behavior
- Defensive practitioners seeking attacker-centric insights

It is **not intended for operational offensive use**.

---

## Ethics and Responsible Research
All contents in this repository is restricted to **authorized, laboratory-based academic research**. No weaponized code, live infrastructure, or real-world targets are included.

---

## Citation
The original *M.Tech* dissertation contains full practical implementations, including experimental setup and technical scripts. This repository presents an **abstracted research framework** derived from that work, intentionally excluding operational code to support ethical academic dissemination and Doctoral-level research.

If this repository contributes to academic work (such as a thesis, dissertation, conference paper, or journal article), please refer to the citation guidance provided under the `citation/` directory.

---

## License
This work is licensed under the **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)** license.

This license permits non-commercial use, sharing, and adaptation with appropriate attribution, provided that derivative works are distributed under the same license.

---

## Disclaimer
This repository is provided solely for **academic and research purposes**. Unauthorized or illegal cyber activity is neither supported nor endorsed.


---

© 2025–2026 Supriyo Guha. All rights reserved except where otherwise noted.

