# Initial Access Model

## 1. Research Framing
Initial access is modeled as the **first breach of trust**, rather than a technical exploit. This framing reflects real-world incidents in which adversaries gain footholds through:
- credential exposure,
- trust abuse,
- or user interaction.

Zero-day exploitation and highly technical attack vectors are explicitly excluded to maintain ethical and academic focus.

---

## 2. Trust-Centric Access Assumption
The model assumes that initial access is achieved through:
- legitimate authentication pathways,
- misuse of granted privileges,
- or manipulation of operational workflows.

This reflects the reality that many critical infrastructure incidents originate from enterprise environments rather than OT systems.

---

## 3. Behavioral States
Initial access is modeled as a transition between states:

- No Access → Limited User Context  
- Limited User Context → Persistent Foothold  

The transition is driven by:
- trust relationships,
- policy enforcement gaps,
- and organizational behavior.

The specific mechanisms are intentionally abstracted.

---

## 4. Constraints and Risk Considerations
The adversary is assumed to:
- avoid actions that trigger immediate alerts,
- prefer persistence over rapid expansion,
- and accept partial access if it enables long-term objectives.

This reflects operational discipline observed in advanced adversaries.

---

## 5. Research Questions Enabled
This model supports research into:
- minimal capability required for meaningful access,
- the influence of organizational workflow on exposure,
- and the relationship between user privileges and attack progression.

---

## 6. Ethical Boundary
No procedural guidance, tooling, or execution steps are included. Initial access is treated purely as a **conceptual transition** within the adversary lifecycle.
