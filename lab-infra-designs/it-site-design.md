# IT Site Design

## 1. Research Role of the IT Segment
The Enterprise IT segment models the administrative and identity-centric infrastructure typically found in organizations operating critical infrastructure. In real deployments, this segment commonly includes:

- centralized identity services,
- administrative workstations,
- file and application services,
- and policy enforcement mechanisms.

From an adversary simulation perspective, the IT segment is critical because it often functions as:
- the primary environment for credential acquisition,
- the control plane for policy and access,
- and the staging area for cross-segment movement.

This segment is therefore designed to support research questions regarding enterprise domain intrusion and trust abuse.

---

## 2. Conceptual Components
The IT segment is modeled using a minimal but representative set of roles:

### Identity and Policy Services
A centralized identity provider (e.g., directory service) is modeled to support:
- authentication and authorization workflows,
- centralized policy and account management,
- group-based privilege and role assignment.

The model emphasizes that identity infrastructure is both operationally necessary and a high-value adversary target.

### Administrative Workstations
Administrative endpoints are modeled to represent systems that:
- perform maintenance and administration,
- hold elevated credentials or tokens,
- and interact with cross-segment gateways.

This supports research on credential exposure risk and privilege boundaries.

### Enterprise Data Services
File or data services are modeled to represent:
- operational data handling,
- automated workflows (e.g., scheduled tasks, synchronization),
- and legitimate data movement that can create abuse opportunities.

---

## 3. Security Assumptions and Constraints
To remain faithful to realistic enterprise environments, the IT segment assumes:

- role-based access is present but imperfect,
- privileged workflows exist for operational reasons,
- segmentation prevents direct access to OT zones,
- boundary access is permitted only through designated conduits.

The threat model excludes unknown vulnerabilities; therefore, this segment is designed such that adversary progress primarily depends on:
- trust misuse,
- credential compromise,
- policy weaknesses,
- and misaligned privileges.

In another word abusing features. 

---

## 4. Adversary-Relevant Attack Surface (Behavioral)
The IT segment is not defined by “open ports” or tool artifacts in this repository. Instead, the relevant research surfaces are behavioral:

- Identity and Credential Lifecycles (issuance, reuse, delegation),
- Administrative Trust Relationships,
- Automation and Scheduled Workflows,
- and Cross-Domain Access Mediation Patterns.

These surfaces map naturally to ATT&CK enterprise behaviors (see `mappings/`), but the repository intentionally avoids operational mapping.

---

## 5. Experimentation Support
The IT segment is designed to support controlled experimental questions such as:

- How does compromise of a user-facing segment translate into enterprise domain access under segmentation constraints?
- Which trust relationships disproportionately enable privilege escalation?
- How does the presence of automation (e.g., replication/synchronization) affect adversary persistence opportunities?

For doctoral research, these questions can be operationalized through:
- comparative studies (segmentation strict vs relaxed),
- privilege policy variations,
- or changes in dependency structure.

---

## 6. Logging and Research Observability (Minimal Assumption)
While defensive engineering is out of scope, research requires interpretability.
Therefore, a minimal assumption is made that:
- boundary events are observable (e.g., authentication and access logs),
- system-level events are available for post-hoc analysis.

No vendor-specific monitoring stack is prescribed in this repository.

---

## 7. Scope Boundaries
This design intentionally excludes:
- weaponized payloads,
- exploit procedures,
- and operational runbooks.

The IT segment is documented at an architectural and behavioral level to remain ethically appropriate for public academic dissemination.

---

## 8. Extensions for Doctoral Research
Possible PhD-level extensions include:

- modeling identity federation or hybrid identity,
- integrating detection-aware constraints without building a full blue-team,
- formalizing privileges and trust as a graph for quantitative analysis,
- and comparing adversary pathways under different identity governance models.
