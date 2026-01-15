## Standards Referenced

This research aligns offensive adversary simulation with internationally recognized cybersecurity standards and frameworks to ensure scientific rigor, reproducibility, and ethical compliance.

The frameworks listed below are referenced for **modeling, mapping, and analysis** purposes only. No proprietary methodologies are reverse engineered or violated.

---

## 1. MITRE ATT&CK Frameworks (Core Research Backbone)

### 1.1 MITRE ATT&CK for Enterprise
MITRE ATT&CK for Enterprise is used to model adversary behavior across
Windows, Active Directory, cloud, and enterprise IT environments.

**Usage in this research:**
- Mapping reconnaissance, initial access, persistence, and lateral movement
- Structuring multi-stage adversary kill chains
- Standardized terminology for attack techniques
- Comparative analysis of red-team tradecraft

**Reference:**
- MITRE ATT&CK Enterprise Matrix

---

### 1.2 MITRE ATT&CK for Industrial Control Systems (ICS)
MITRE ATT&CK for ICS is used to model adversary techniques targeting
Operational Technology (OT) and critical infrastructure environments.

**Usage in this research:**
- Mapping IT-to-OT pivot paths
- Modeling HMI, historian, and PLC attack techniques
- Aligning simulated attacks with real-world ICS incidents
- Ensuring OT-specific constraints and safety considerations

**Reference:**
- MITRE ATT&CK for ICS Matrix

---

### 1.3 MITRE D3FEND (Reference Mapping Only)
MITRE D3FEND is referenced to contextualize defensive controls corresponding
to offensive techniques.

**Usage in this research:**
- Analytical mapping only
- No blue-team implementation is performed

---

## 2. NIST Cybersecurity & ICS Standards

### 2.1 NIST SP 800-82 Rev. 3 – Guide to ICS Security
Primary reference for ICS security architecture, segmentation, and risk modeling.

### 2.2 NIST SP 800-53 Rev. 5 – Security and Privacy Controls
Referenced for control taxonomy alignment during impact and risk discussion.

### 2.3 NIST SP 800-61 Rev. 2 – Incident Handling Guide
Referenced to frame adversary impact timelines and response considerations.

---

## 3. ISO/IEC Information Security Standards (IT & Enterprise Security)

### 3.1 ISO/IEC 27001 – Information Security Management System (ISMS)
ISO/IEC 27001 provides the organizational and governance foundation
for enterprise information security.

**Relevance to this research:**
- Establishes baseline security governance assumptions
- Defines scope boundaries for enterprise environments
- Supports risk-based adversary modeling

---

### 3.2 ISO/IEC 27002 – Information Security Controls
ISO/IEC 27002 complements ISO 27001 by providing detailed security controls.

**Usage in this research:**
- High-level control mapping
- Analytical reference for attack surface assumptions

---

### 3.3 ISO/IEC 27005 – Information Security Risk Management
Referenced to align adversary simulations with formal risk assessment models.

---

## 4. Industrial & Critical Infrastructure Standards

### 4.1 IEC 62443 Series – Industrial Automation & Control System Security
Primary international standard for securing industrial control systems.

**Usage in this research:**
- Modeling OT segmentation and trust boundaries
- Validating ICS security assumptions

---

### 4.2 CISA & ENISA Guidance
Public advisories and threat landscape reports are used for contextual analysis
of real-world critical infrastructure attacks.

---

## 5. Framework Integration Strategy

This research integrates the above standards as follows:

| Layer | Framework |
|------|----------|
| Adversary Behavior | MITRE ATT&CK (Enterprise & ICS) |
| Enterprise Governance | ISO/IEC 27001 |
| Security Controls | ISO/IEC 27002, NIST SP 800-53 |
| ICS Architecture | NIST SP 800-82, IEC 62443 |
| Risk Modeling | ISO/IEC 27005 |

This multi-framework approach ensures that adversary simulation remains technically accurate, ethically grounded, and academically defensible.
