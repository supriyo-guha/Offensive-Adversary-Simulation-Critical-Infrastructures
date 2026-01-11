# Architecture Overview

## 1. Purpose and Research Role
This repository models a segmented critical infrastructure environment to support **ethical adversary simulation research**. The architecture is designed to enable controlled study of:

- Enterprise compromise and lateral movement dynamics,
- Cross-domain trust abuse (IT → business operations → OT),
- The influence of segmentation on adversary feasibility,
- and conceptual Cyber–Physical impact pathways.

The objective is not to replicate a specific organization, but to provide a repeatable **research abstraction** that preserves the structural properties commonly observed in real-world critical infrastructure deployments.

---

## 2. Design Principles
The architecture follows five guiding principles:

### (P1) Segmentation as a First-Class Research Variable
Network segmentation is modeled explicitly so that adversary movement must occur through constrained pathways. This ensures that the simulation can examine how attack chains evolve under realistic barriers.

### (P2) Trust Boundaries and Conduits
The environment is organized into distinct trust zones, connected through defined conduits (controlled access pathways). This mirrors common industrial security guidance emphasizing zoning, mediation, and least privilege.

### (P3) Plausible Operational Dependencies
The environment includes dependency relationships typical of real systems:
file flows, identity dependencies, and administrative workflows that—while legitimate—may be abused.

### (P4) Research Safety and Non-Operational Abstraction
Operational details that could enable misuse (e.g., live infrastructure configurations, credentials, exploit steps) are intentionally excluded from public documentation. The focus is on architecture, assumptions, and behavior.

### (P5) Auditability for Research Interpretation
The architecture is designed so that simulation outcomes can be interpreted in a research context. Minimal telemetry assumptions are included (e.g., logs, boundary events), without turning the work into a defensive engineering project.

---

## 3. High-Level Segments
The environment is decomposed into three primary segments:

1. **Enterprise IT Segment**  
   Represents identity services, administrative endpoints, and corporate infrastructure. This segment is typically a high-value target because it provides access to credentials, policy enforcement, and data.

2. **Business Operations / Customer Support Segment**  
   Represents user-facing workstations and operational data handling. This segment is modeled as a plausible initial compromise point due to exposure to external interactions and social engineering pressure.

3. **Operational Technology (OT) Segment**  
   Represents industrial monitoring and control environments. This segment is modeled as highly constrained and segmented internally to reflect industrial zoning practices and safety considerations.

Each segment is documented in dedicated files:
- `it-site-design.md`
- `customer-support-site.md`
- `ot-site-design.md`

---

## 4. Boundary Enforcement and Access Mediation
Critical infrastructure environments rarely permit direct enterprise-to-control network access. Therefore, the architecture includes a **mediated access pattern** where OT access is restricted and monitored through a controlled gateway or jump pathway.

The purpose of modeling mediated access is to study adversary behavior under constraints:
- how an attacker discovers approved conduits,
- how they exploit legitimate workflows,
- and how boundary enforcement shapes attack progression.

---

## 5. Virtualized Testbed Considerations (Non-Operational)
The environment is assumed to be hosted in a virtualized testbed to support:
- isolation from real-world systems,
- snapshotting and rollback for repeatable experiments,
- controlled variability for comparative studies.

Resource constraints may be intentionally applied to emulate realistic performance limits, but this is treated as a research control rather than an implementation prescription.

---

## 6. Relationship to Threat Model and Research Questions
This architecture is directly aligned with:
- the threat model constraints (`docs/threat-model.md`),
- ethics and scope boundaries (`docs/ethics-and-scope.md`),
- and core research questions (`docs/research-questions.md`).

In particular, segmentation and trust boundaries serve as the central mechanisms through which IT-to-OT feasibility and adversary adaptation are studied.

---

## 7. Limitations and External Validity
This architecture is an abstraction. It does not claim to represent all critical infrastructure deployments. Key limitations include:

- simplified representation of vendor diversity,
- absence of real operator workflows and safety systems,
- intentional omission of operational configurations to prevent misuse.

Nevertheless, the architecture preserves structurally important properties:
segmentation, trust, dependency, and constrained access—supporting meaningful
research in adversary simulation.

---

## 8. Diagram Guidance (Repository Usage)
Diagrams should be stored under `lab-infra-designs/diagrams/` as either:
- `.drawio` sources (preferred for reproducibility), and/or
- exported `.png` images for quick viewing.

Diagrams should remain conceptual and avoid disclosing operational details.

Recommended diagram types:
- logical architecture (zones and conduits),
- trust boundary map,
- adversary pathway abstraction (high-level stages only).
