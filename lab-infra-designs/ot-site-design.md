# OT Site Design

## 1. Research Role of the OT Segment
The OT segment models the industrial environment where monitoring and control functions occur. It is characterized by:

- high availability requirements,
- constrained change management,
- legacy protocol prevalence,
- and strong segmentation expectations.

For adversary simulation, the OT segment enables study of:
- constrained entry pathways (IT → OT),
- discovery and movement within OT zones,
- and conceptual cyber–physical impact modeling.

The repository intentionally treats OT behavior at a research abstraction level to remain ethically appropriate.

---

## 2. Zoning Model and Internal Segmentation
A central principle in OT security is **zoning and conduits**. Accordingly, the OT segment is modeled as internally segmented into:

- an OT access mediation zone (often a DMZ-like boundary zone),
- a supervisory/engineering zone (operator interfaces and engineering functions),
- and a control/process zone (controllers and process simulation components).

This structure supports realistic reasoning about:
- why direct enterprise access is typically prohibited,
- how controlled pathways emerge operationally,
- and how adversaries may attempt to exploit those pathways.

---

## 3. Access Mediation and the “Conduit” Concept
Industrial environments often require administrative access for maintenance. Rather than permitting direct enterprise access to OT assets, deployments commonly require access to occur through a mediated conduit.

In this repository, the conduit is modeled conceptually as:
- a controlled access point,
- subject to authentication and policy,
- with restricted protocol exposure.

The conduit is a research focus because it becomes:
- the primary legitimate bridge between trust zones,
- and therefore a primary adversary objective in cross-domain movement.

---

## 4. Representative OT Roles (Abstracted)
The OT segment is modeled through abstract roles:

### Operator Interface Role
Represents monitoring and supervisory interaction. It supports research on:
- situational awareness,
- operator trust,
- and the consequences of manipulated visibility.

### Engineering Role
Represents configuration and maintenance capabilities. This role is central to research on privilege boundaries within OT, because engineering workflows often carry elevated authority.

### Control/Process Role
Represents the process execution surface (controllers and process simulation). For ethical reasons, the repository models cyber–physical effects conceptually (e.g., “process parameters”) rather than providing operational manipulation steps.

---

## 5. OT-Specific Constraints
OT environments are constrained by:
- availability requirements,
- limited patch windows,
- and safety-critical operational considerations.

These constraints are modeled as assumptions that shape adversary behavior:
- adversaries may prefer stealth over disruption,
- may rely on legitimate workflows,
- and may avoid actions that produce immediate operator suspicion.

This supports doctoral questions about the interaction between adversary OpSec
and OT operational realities.

---

## 6. Impact Modeling (Conceptual and Non-Destructive)
Cyber–physical impact is treated as a **risk model**, not an execution plan. The
repository focuses on:

- how control visibility and authority relate to risk,
- how constrained access affects feasibility,
- and how organizational response decisions amplify impact.

This approach aligns with ethical requirements for public academic work and is
compatible with research that seeks to improve resilience without enabling harm.

---

## 7. Extensions for Doctoral Research
Potential PhD extensions include:

- formalizing OT zones and conduits using graph models,
- measuring attack feasibility under different conduit policies,
- integrating safety constraints and response decision variables,
- expanding to multi-site OT architectures or vendor diversity (conceptually).
