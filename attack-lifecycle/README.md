# Attack Lifecycle Modeling

This section documents the behavior-centric adversary lifecycle used in
this research. The lifecycle is modeled as a sequence of decision-driven
states rather than a procedural attack chain.

## Conceptual Adversary Lifecycle

```text
                +---------------------------+
                |   Continuous              |
                |   Reconnaissance          |
                +-------------+-------------+
                              |
                              v
                +---------------------------+
                |   Initial Access          |
                |   (Trust Abuse)           |
                +-------------+-------------+
                              |
                              v
        +---------------------+---------------------+
        |                                           |
        v                                           v
+---------------------------+         +---------------------------+
|  Lateral Movement         |         |  Persistence & OpSec      |
|  (Trust Relationships)    |         |  (Risk Management)        |
+-------------+-------------+         +-------------+-------------+
              \                               /
               \                             /
                +---------------------------+
                              |
                              v
                +---------------------------+
                |   IT → OT Pivot           |
                |   (Mediated Access)       |
                +-------------+-------------+
                              |
                              v
                +---------------------------+
                |  Cyber–Physical Impact    |
                |  (Operational / Decision) |
                +---------------------------+
