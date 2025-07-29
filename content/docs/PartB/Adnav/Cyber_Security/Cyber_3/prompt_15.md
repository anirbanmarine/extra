---
title: Maritime Cyber Security :respond to and recover from cyber security incidents
type: docs
sidebar:
  open: true
---

Of course. Responding to and recovering from cybersecurity incidents in the maritime domain is a critical and unique challenge due to the convergence of Information Technology (IT) and Operational Technology (OT), the remote nature of vessels, and the high stakes involving safety, environmental protection, and international commerce.

Here is a comprehensive guide on how to respond to and recover from maritime cybersecurity incidents, structured around the industry-standard Incident Response Lifecycle.

---

### **The Maritime Cyber Incident Response Lifecycle**

An effective response follows a structured plan. The internationally recognized phases are: **Preparation, Identification, Containment, Eradication, Recovery, and Lessons Learned.**

#### **Phase 1: Preparation (The Most Critical Phase)**

Effective response is impossible without thorough preparation. This happens long before an incident occurs.

*   **Develop a Vessel-Specific Incident Response Plan (IRP):** This is not a generic IT plan. It must be tailored to each vessel or class of vessels. It should:
    *   Define what constitutes a cyber incident (e.g., unresponsive ECDIS, GPS spoofing, ransomware on a cargo system, loss of network).
    *   Establish clear roles and responsibilities (**Onboard:** Master, Chief Engineer, ETO; **Ashore:** Company Security Officer (CSO), CISO, IT/OT support, Designated Person Ashore (DPA)).
    *   Create a simple, clear contact list for immediate communication (ashore team, flag state, insurers, P&I Club).
    *   Outline immediate action "battle cards" for specific scenarios (e.g., "In Case of GPS Jamming," "In Case of Ransomware").
*   **Conduct Drills and Training:** Regularly drill the IRP with both ship and shore personnel. These drills should simulate realistic scenarios, such as a compromised ballast water management system or a phishing attack that captures the Captain's credentials.
*   **System Hardening and Segmentation:**
    *   **Network Segmentation:** Ensure critical OT systems (ECDIS, radar, propulsion control) are on a separate, isolated network from the crew/business IT network. A firewall should strictly control any necessary traffic between them.
    *   **Backups:** Maintain regular, tested, and isolated backups of critical data and system configurations. This includes backups for navigation systems, cargo plans, and administrative files. Keep at least one backup offline or "air-gapped."
*   **Inventory and Baseline:** Know what systems you have, what "normal" performance looks like, and what their dependencies are. Without a baseline, you can't identify a deviation.

---

#### **Phase 2: Identification & Analysis**

This is the "detective" phase where you confirm an incident is happening and determine its scope.

*   **Detection Sources (Onboard & Ashore):**
    *   **System Alarms:** Unexpected alarms from propulsion, navigation (e.g., "GPS Signal Lost"), or machinery control systems.
    *   **Anomalous Behavior:** ECDIS showing the vessel in the wrong location, slow or unresponsive systems, inability to access files, or strange pop-ups (ransom notes).
    *   **Crew Reports:** A crew member reporting a suspicious email or a non-functioning computer.
    *   **Shore-side Monitoring:** A Security Operations Center (SOC) detecting unusual traffic originating from the vessel's satellite connection.
*   **Initial Analysis & Triage (The "What, Where, and How Bad?" questions):**
    1.  **Notify:** The designated onboard officer (e.g., Master) immediately notifies the designated shore contact (e.g., CSO/DPA) using a pre-agreed, potentially out-of-band communication method (satellite phone, emergency comms).
    2.  **Assess Impact:**
        *   Is it affecting the safety of navigation (e.g., GPS, ECDIS, Radar)?
        *   Is it affecting the safety of the vessel (e.g., propulsion, stability, power management)?
        *   Is it affecting commercial operations (e.g., cargo computer, communications)?
        *   Is it contained to a single system, or has it spread?
    3.  **Preserve Evidence:** Do not immediately turn off or wipe affected systems unless they pose an immediate safety risk. Isolate them and, if possible, preserve their state (memory, disk image) for later forensic analysis. The Voyage Data Recorder (VDR) may also contain crucial data.

---

#### **Phase 3: Containment**

The goal is to stop the bleeding and prevent the incident from spreading further.

*   **Short-Term Containment (Immediate Actions):**
    *   **Isolate the Affected System:** Disconnect the compromised computer or device from the network (unplug the Ethernet cable). **Do not use the software 'disconnect' function**, as malware can fake this.
    *   **Isolate Networks:** If the breach is on the IT network, immediately sever any connection to the critical OT network. This is where network segmentation proves its value.
    *   **Isolate the Vessel:** Consider temporarily restricting or severing the vessel's primary connection to the internet to prevent remote command-and-control by the attacker. Switch to backup communication channels.
*   **Long-Term Containment (System-wide Strategy):**
    *   The ashore team, in coordination with the vessel crew, can start blocking malicious IP addresses at the fleet-wide firewall level.
    *   Review access logs to identify compromised user accounts and disable them immediately.

---

#### **Phase 4: Eradication**

Once contained, the threat must be completely removed from the environment.

*   **Removing the Malware/Threat:** This involves identifying the malicious software or vulnerability and eliminating it. For a ship at sea with limited expertise, this is often the hardest part.
*   **The "Nuke and Pave" Approach:** In many cases, the safest and most reliable method is to completely wipe the affected system and restore it from a known-good backup or a clean factory image. **Never trust a system that has been compromised.**
*   **Vulnerability Patching:** Identify the vulnerability that was exploited (e.g., an unpatched operating system, weak password) and remediate it across all similar systems on the vessel and, potentially, the entire fleet.

---

#### **Phase 5: Recovery**

This phase focuses on restoring systems to normal operation safely and efficiently.

*   **Prioritize Restoration:**
    1.  **Safety & Navigation Systems:** Restore ECDIS, GPS, and propulsion controls first. This may involve switching to redundant systems or, in a worst-case scenario, reverting to manual operations (e.g., using paper charts).
    2.  **Vessel Operations Systems:** Restore power management, ballast water, and other critical machinery systems.
    3.  **Commercial & Administrative Systems:** Restore cargo planning computers and business IT systems last.
*   **Restoration Process:**
    *   **Use Known-Good Sources:** Restore from clean backups that were verified *before* the incident. Have pre-staged, clean software installers and firmware on secure USB drives or a dedicated onboard server.
    *   **Verification and Monitoring:** After restoration, closely monitor the systems for any signs of residual infection or unusual behavior. Ensure they are functioning as expected before declaring them fully operational.
*   **Communication:** Keep all stakeholders (management, charterers, port authorities, flag state) informed of the recovery progress according to the IRP's communication plan.

---

#### **Phase 6: Post-Incident Activity (Lessons Learned)**

This is where you turn a costly incident into a valuable learning experience to improve future resilience.

*   **Forensic Analysis:** If possible, conduct a detailed analysis of the compromised systems and logs to understand the full timeline, the attacker's methods, and the root cause.
*   **Lessons Learned Report:** Hold a post-mortem meeting with all involved parties (ship and shore). Document:
    *   What went well?
    *   What went wrong?
    *   What were the root causes (technical and procedural)?
    *   How can the IRP be improved?
    *   What new training or technology is needed?
*   **Update and Improve:**
    *   Revise the Incident Response Plan (IRP) and the Ship Security Plan (SSP).
    *   Implement new technical controls (e.g., better firewalls, endpoint detection).
    *   Provide updated training to the crew and shore staff based on the incident.
*   **Regulatory and Legal Reporting:** Complete all necessary reports for flag states, port state control, insurers, and other regulatory bodies as required by IMO 2021 guidelines and company policy.

### **Practical Scenario: Ransomware on Vessel's Cargo Planning Computer**

1.  **Identification:** Chief Mate finds the cargo computer is encrypted with a ransom note displayed.
2.  **Response (Onboard):**
    *   Chief Mate immediately informs the Master.
    *   ETO is instructed to physically unplug the computer's network cable.
    *   Master contacts the ashore CSO/DPA via sat phone, reporting a "Code Red Cyber Incident - Ransomware."
3.  **Containment (Ashore & Onboard):**
    *   Ashore IT confirms the ship's business network is isolated from other fleet vessels.
    *   ETO confirms the ship's business (IT) and navigation (OT) networks are physically separated. No containment needed for OT.
4.  **Eradication & Recovery:**
    *   **Decision:** The company policy is **not to pay the ransom**.
    *   **Action:** The crew retrieves the backup laptop, which also has the cargo planning software installed. They use it to continue operations.
    *   The infected computer is kept isolated and powered down to preserve evidence. At the next port, it will be handed to a technical team to be completely wiped and re-imaged.
5.  **Lessons Learned:** The post-incident review finds the ransomware entered via a phishing email opened by a crew member. The company rolls out enhanced phishing training for all crew and implements stricter email filtering for the fleet.

In the maritime world, effective cyber incident response is not just an IT function; it is a core component of modern seamanship and vessel safety.