# Trust Boundaries

## 1. Conceptual Definition
A trust boundary separates components with different security assumptions, privilege levels, and operational constraints. In critical infrastructure, trust boundaries are not purely network-based; they also include:

- identity and authorization boundaries,
- operational responsibility boundaries,
- and policy/decision boundaries (who is allowed to do what, and when).

This document defines the trust boundaries modeled in this repository and explains their research relevance.

---

## 2. Primary Trust Boundaries in the Model

### Boundary A: External Inputs → Business Operations 
Business operations units interface with external inputs and are therefore modeled with a higher exposure surface. This boundary motivates research on:
- trust abuse,
- user interaction risk,
- and initial foothold acquisition without advanced exploitation.

### Boundary B: Business Operations → Enterprise IT
Business operations commonly require enterprise services, creating a boundary defined by:
- identity reliance,
- shared resources,
- and cross-unit permissions.

This boundary is central to enterprise domain intrusion studies because it often provides an adversary with a possible transition path into the core IT environment.

### Boundary C: Enterprise IT → OT Access Mediation Zone 
This boundary represents the deliberate separation between enterprise systems and industrial environments. The access mediation zone acts as a conduit, enforcing:
- protocol restriction,
- authentication controls,
- and operational monitoring.

This boundary is the primary structural defense against IT-to-OT pivoting.

### Boundary D: OT Access Mediation Zone → OT Internal Zones

Even within OT, internal separation is modeled to reflect zoning practice.

This boundary supports research on:
- limited blast radius,
- privilege compartmentalization,
- and constrained movement within industrial environments.

---

## 3. Trust as a Graph (Research Abstraction)
For doctoral research, trust can be formalized as a graph:

- Nodes represent roles, systems, or zones
- Edges represent authorized interactions and dependencies
- Edge weights can represent strength of trust or required privileges

This representation supports quantitative and comparative research:
- identifying “high-leverage” trust relationships,
- assessing which edges enable disproportionate adversary progress,
- and evaluating how architectural changes reduce risk.

The repository does not prescribe a specific metric, but the abstraction is
provided for research extension.

---

## 4. Boundary Failure Modes (Behavioral)
Trust boundaries fail less often due to “open ports” and more often due to:

- excessive privileges granted for operational convenience,
- credential reuse and token exposure,
- weak separation of duties,
- automation workflows that bypass human review,
- and decision-layer responses that amplify disruption.

These failure modes align with multiple real-world incidents where enterprise compromise caused operational impact without direct OT exploitation.

---

## 5. Relationship to Adversary Simulation
Trust boundaries define adversary objectives:
- crossing boundaries is the primary measure of adversary progress,
- boundaries shape what behaviors are feasible,
- and boundary enforcement determines the need for stealth and adaptation.

Therefore, in this repository, trust boundaries are treated as core research artifacts rather than implementation details.

---

## 6. Ethical Considerations
This repository documents trust boundaries conceptually and avoids:
- deployable configuration guidance,
- step-by-step boundary bypass instructions,
- or reproduction procedures.

The purpose is to support academic understanding and defensive improvement.

---

## 7. Extensions for Doctoral Research
Possible extensions include:

- modeling boundary controls as experimental variables (strict vs permissive),
- integrating decision-layer variables (shutdown choice under uncertainty),
- formalizing boundary strength metrics,
- or evaluating how policy changes alter adversary feasibility.
