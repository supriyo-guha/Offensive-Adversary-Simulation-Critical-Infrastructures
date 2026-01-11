# ICS and SCADA Attack Literature Review

## Introduction
Industrial Control Systems (ICS) and Supervisory Control and Data Acquisition (SCADA) environments present unique security challenges due to their cyber–physical nature, legacy protocols, and operational constraints.

This document reviews academic, industrial, and governmental literature relevant to ICS security, with a focus on **offensive research perspectives**.

---

## Categories of Existing Research

### Defensive Security Studies
The majority of ICS literature focuses on:
- anomaly detection,
- network segmentation,
- intrusion detection systems,
- and resilience engineering.

While valuable, these works often assume attacker behavior rather than systematically modeling it.

---

### Incident Analysis and Post-Mortem Studies
Several studies analyze historical ICS incidents, including:
- malware reverse engineering,
- forensic reconstruction,
- and impact assessment.

These analyses provide insight into attacker capabilities but rarely offer **reproducible simulation methodologies**.

---

### Protocol Vulnerability Research
Research on protocols such as Modbus, DNP3, and IEC 60870 highlights:
- lack of authentication,
- weak integrity guarantees,
- and legacy design assumptions.

However, protocol-focused studies often neglect enterprise-to-OT attack pathways.

---

### Red Team and Adversary Simulation Research
Academic work explicitly addressing offensive simulation in ICS contexts remains limited. Existing studies frequently:
- isolate OT from enterprise environments,
- focus on tool development,
- or avoid IT–OT convergence entirely.

---

## Identified Limitations in Existing Literature
The literature reveals several limitations:

- Fragmentation between IT and OT research communities
- Limited modeling of trust relationships
- Minimal consideration of adversary operational security
- Ethical hesitancy leading to over-abstraction

---

## Relevance to This Research
This repository positions itself as a **bridging effort**, integrating enterprise adversary models with OT security research under controlled, ethical constraints.

---

## Conclusion
The literature demonstrates strong defensive foundations but exposes a clear need for **structured offensive simulation research** to complement existing approaches. This work contributes toward that direction.
