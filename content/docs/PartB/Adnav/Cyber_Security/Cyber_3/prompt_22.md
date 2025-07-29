---
title: Maritime Cyber Security :establish contingency plans (Maritime Cyber Security
  Incident Response)
type: docs
sidebar:
  open: true
---

Of course. Establishing a robust Maritime Cyber Security Incident Response Plan (CSIRP) is a critical requirement under the IMO's Resolution MSC.428(98), which mandates that cyber risks be addressed within a vessel's Safety Management System (SMS).

This guide will provide a comprehensive framework for establishing these contingency plans, tailored specifically for the maritime environment (covering both vessels and shoreside operations).

---

### **Maritime Cyber Security Incident Response Plan (CSIRP): A Framework**

A CSIRP is not just a technical document; it's an operational plan that integrates people, processes, and technology to manage the aftermath of a cyber attack. The primary goals are:
*   **Safety First:** Ensure the safety of the crew, vessel, cargo, and the marine environment.
*   **Containment:** Limit the operational, financial, and reputational damage.
*   **Resilience:** Restore critical systems and return to normal operations as quickly and safely as possible.
*   **Compliance:** Meet regulatory and legal reporting requirements.

The plan should be structured around the internationally recognized incident response lifecycle.

---

### **Phase 1: Preparation - The Foundation**

This is the most crucial phase. Effective response is impossible without thorough preparation.

**1. Identify Critical Systems & Data:**
*   **Operational Technology (OT):**
    *   **Navigation:** GPS/GNSS, ECDIS (Electronic Chart Display), AIS (Automatic Identification System), RADAR.
    *   **Propulsion & Machinery:** Engine Control Systems, Power Management, Ballast Water Systems.
    *   **Cargo Management:** Crane controls, tank monitoring, reefer container systems.
    *   **Safety & Security:** CCTV, vessel access control systems.
*   **Information Technology (IT):**
    *   Crew and Business Networks (Wi-Fi).
    *   Administrative Systems (e.g., payroll, purchasing).
    *   Communication Systems (Satcom, VoIP).
    *   Cargo Manifests and Stowage Plans.

**2. Establish the Cyber Security Incident Response Team (CSIRT):**
Define clear roles and responsibilities. The team should have both onboard and shoreside members.

| Role | Onboard Responsibility | Shoreside Responsibility |
| :--- | :--- | :--- |
| **Incident Coordinator** | **Captain/Master:** Overall command, safety of vessel. | **Designated Person Ashore (DPA) / CISO:** Coordinates entire response, liaises with management. |
| **Technical Lead** | **Chief Engineer / ETO:** Manages onboard OT/IT systems. | **IT/OT Security Manager:** Leads technical investigation, forensics, and recovery. |
| **Communications Lead** | **Senior Officer:** Manages internal crew communication. | **PR/Communications Officer / Legal Counsel:** Manages external comms (authorities, clients, media). |
| **Team Members** | Other officers, relevant crew. | IT staff, legal, HR, insurance representative, third-party experts. |

**3. Develop an Incident Classification System:**
Categorize incidents by severity to dictate the level of response.

*   **Level 3 (Low):** Isolated malware on a non-critical crew laptop. No impact on operations.
*   **Level 2 (Medium):** Phishing attack compromises business email. Potential data breach but no immediate safety risk.
*   **Level 1 (High):** Ransomware on the cargo planning system. Major operational disruption.
*   **Level 0 (Critical):** GPS spoofing or loss of engine control. Immediate threat to safety of life at sea (SOLAS).

**4. Tools & Resources:**
*   Ensure offline access to the CSIRP, contact lists, and system diagrams.
*   Maintain clean, offline backups of critical data and system configurations.
*   Have contracts in place with third-party forensic and incident response firms.

---

### **Phase 2: Detection & Identification**

How do you know an incident has occurred?

*   **Technical Indicators:**
    *   Alerts from antivirus, firewalls, or intrusion detection systems.
    *   Unusual network traffic or system behavior (e.g., ECDIS showing incorrect position).
    *   Ransomware notes or locked files.
    *   System failures or unresponsiveness.
*   **Human Indicators:**
    *   Crew member reports a suspicious email or pop-up.
    *   Physical tampering with equipment.
    *   Reports from shoreside of unusual vessel data transmissions.

**Action:** Once a potential incident is detected, the first person to notice must immediately report it to the designated onboard lead (e.g., the Officer of the Watch), who then activates the CSIRP and notifies the Captain.

---

### **Phase 3: Containment**

The goal is to stop the incident from spreading and causing more damage.

*   **Immediate Actions (Onboard):**
    *   **Isolate the affected system:** Disconnect the system from the network (unplug the network cable). **Do not turn it off** unless instructed by the technical lead, as this can destroy forensic evidence in memory.
    *   **Segment networks:** If a business network is compromised, disconnect it from critical operational networks. This might involve physically disconnecting switches or activating pre-configured firewall rules.
    *   **Consider "Cyber Air-Gapping":** In a severe attack, consider disconnecting the entire vessel from the internet (shutting down the Satcom data link) to prevent remote command-and-control.
*   **Shoreside Actions:**
    *   Block malicious IP addresses at the shoreside firewall.
    *   Disable compromised user accounts.
    *   Preserve logs and evidence from all related systems.

---

### **Phase 4: Eradication**

Remove the threat and its root cause from the environment.

*   **Onboard & Shoreside:**
    *   Identify and remove malware.
    *   Identify and patch the vulnerability that was exploited (e.g., an unpatched OS, a weak password).
    *   If necessary, wipe and rebuild the affected system from a known-good backup or baseline image.
    *   Conduct a full scan of all related systems to ensure the threat is completely removed.

---

### **Phase 5: Recovery**

Restore systems and return to normal, safe operations.

*   **Prioritized Restoration:** Bring critical systems back online first. Safety systems (Navigation, Propulsion) take precedence over administrative systems.
*   **Manual Fallbacks:** During recovery, rely on established manual procedures (e.g., using paper charts, celestial navigation, sound-powered phones, manual engine control).
*   **Testing & Verification:** Before bringing a system back into full operational use, carefully test and monitor it to ensure it is clean and functioning correctly.
*   **Communication:** Keep all stakeholders (crew, shoreside management, authorities, charterers) informed of the recovery progress.

---

### **Phase 6: Post-Incident Activity (Lessons Learned)**

This is vital for improving future resilience.

*   **Conduct a Post-Incident Review:** Within two weeks of the incident, the full CSIRT should meet to discuss what happened.
*   **Analyze the Incident:**
    *   What was the root cause?
    *   How was it detected?
    *   What went well in the response?
    *   What could have been done better?
    *   Were the procedures clear and effective?
*   **Update the Plan:** Revise the CSIRP, technical defenses, and training based on the findings.
*   **Reporting:** Complete all required reports for flag states, insurers, and other regulatory bodies. The DPA is typically responsible for this.

### **Scenario-Specific Playbooks (Examples to include in the CSIRP)**

Your plan should contain mini-plans, or "playbooks," for specific, high-probability scenarios.

**Example 1: GPS/GNSS Spoofing or Jamming**
*   **Detection:** Vessel position on ECDIS/GPS deviates significantly from other indicators; GPS alarm; erratic speed/course readings.
*   **Immediate Actions:**
    1.  Immediately notify the Master.
    2.  Cross-verify position using alternate means: RADAR fixes, visual bearings, celestial navigation.
    3.  Shift to manual steering.
    4.  Broadcast a warning to nearby vessels about navigation uncertainty if necessary.
*   **Recovery:** Attempt to restart the GPS unit; switch to backup units; rely on manual navigation until the signal is reliable.

**Example 2: Ransomware on Vessel's Cargo/Administrative Computer**
*   **Detection:** Ransom note on screen; files are encrypted and inaccessible.
*   **Immediate Actions:**
    1.  **Do not pay the ransom.**
    2.  Immediately disconnect the infected computer from the network.
    3.  Notify the Master and Shoreside Technical Lead.
*   **Containment:** Scan all other computers on the same network.
*   **Eradication/Recovery:** Wipe the machine and restore from a known-good, offline backup. Inform shoreside to ensure the same malware has not propagated to company systems.

### **Implementation and Maintenance**

*   **Training:** Train all crew and relevant shoreside staff on their roles in the CSIRP. This should be part of their onboarding and annual refresher training.
*   **Drills & Exercises:** Regularly conduct tabletop exercises and full-scale drills to test the plan. Simulate a GPS failure or a phishing attack and walk through the response.
*   **Review & Update:** The CSIRP must be reviewed and updated at least annually, or after any significant system change, drill, or actual incident.

By establishing this comprehensive contingency plan, a maritime organization moves from a reactive to a proactive and resilient posture, safeguarding its crew, assets, and operations in the face of modern cyber threats.