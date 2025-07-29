---
title: Maritime Cyber Security :investigating cyber incidents
type: docs
sidebar:
  open: true
---

Of course. Investigating a cyber incident in the maritime domain is a complex process that blends traditional digital forensics with the unique operational, environmental, and jurisdictional challenges of the sea.

Here is a comprehensive guide to investigating maritime cyber incidents, broken down into key phases and considerations.

---

### **The Unique Challenges of Maritime Cyber Incident Investigation**

Before diving into the process, it's crucial to understand why a maritime investigation is different from a typical corporate one:

*   **Remote & Isolated Environment:** The primary location of the incident (the vessel) is often at sea, with limited or high-latency satellite connectivity, making remote analysis and support difficult.
*   **IT/OT Convergence:** Ships are a blend of Information Technology (IT) systems (crew email, administrative PCs) and Operational Technology (OT) systems that control physical processes. An attack on OT can have severe safety and environmental consequences. Key OT systems include:
    *   **ECDIS** (Electronic Chart Display and Information System)
    *   **GPS/GNSS** (Global Navigation Satellite System)
    *   **AIS** (Automatic Identification System)
    *   **Propulsion and Machinery Control Systems**
    *   **Ballast Water and Cargo Management Systems**
*   **Jurisdictional Complexity:** An incident can occur in international waters, but the vessel has a Flag State, is owned by a company in another country, operated by a third, and is heading to a port in a fourth. This creates a maze of legal and reporting requirements.
*   **The Human Factor:** The crew are the first responders, but they are not typically cyber security experts. Their primary focus is the safe operation of the vessel.
*   **Evidence Volatility:** On a ship, power cycles are common, and systems may need to be rebooted to restore functionality, potentially destroying crucial volatile evidence (like data in RAM). The Voyage Data Recorder (VDR) also has a limited recording loop (e.g., 12-48 hours).
*   **Complex Supply Chain:** The source of a breach could be a third-party vendor, a port agent, a technician who came aboard with an infected laptop, or even a crew member's personal device.

---

### **The Incident Response Lifecycle (Adapted for Maritime)**

The investigation follows the standard six-phase incident response lifecycle, but each phase has specific maritime considerations. This plan should be part of the vessel's **Cyber Security Plan**, as required by IMO Resolution MSC.428(98).

#### **Phase 1: Preparation (Before an Incident Occurs)**

This is the most critical phase. Without preparation, an effective investigation is nearly impossible.

*   **Maritime-Specific Actions:**
    *   **Asset Inventory:** Create and maintain a detailed inventory of all IT and OT systems on board. Know what’s on the network.
    *   **Define Roles & Responsibilities:**
        *   **Onboard:** Who is the designated cyber security lead? (e.g., Captain, Chief Engineer, or ETO). What are their immediate responsibilities?
        *   **Ashore:** Who is the 24/7 point of contact? (e.g., Company Security Officer - CSO, Designated Person Ashore - DPA, IT support).
    *   **Develop an Incident Response Plan:** This plan must be accessible offline on the bridge and in the engine control room. It should include simple, checklist-style instructions for the crew.
    *   **Deploy Tools:** Where possible, deploy monitoring tools (like network intrusion detection systems). Have an "Incident Response Fly-Away Kit" ready ashore, containing forensic laptops, network taps, write-blockers, and necessary cables.
    *   **Crew Training:** Train crew on identifying suspicious activity (e.g., strange GPS behavior, slow systems, ransom notes) and their first-step reporting duties.

#### **Phase 2: Identification (An Incident is Suspected)**

This phase is about detecting the incident and making an initial assessment.

*   **Potential Indicators on a Vessel:**
    *   **Navigation:** GPS/GNSS showing incorrect position, ECDIS charts not loading, or showing ghost vessels.
    *   **Machinery:** Inability to control engines, pumps, or steering from the control station. Alarms failing or triggering falsely.
    *   **Communications:** Loss of satellite communications (SATCOM) or VHF.
    *   **IT Systems:** Ransomware message on a screen, unusually slow network, inability to access files or systems.
    *   **Physical:** An unknown USB drive found plugged into a bridge console.
*   **First Steps for the Crew:**
    1.  **Don't Panic.** Prioritize the safety of the crew, vessel, and environment.
    2.  **Report Immediately.** Contact the designated onboard lead and the 24/7 ashore contact. Provide clear information: What system is affected? What are the symptoms? When did it start?
    3.  **Do NOT Reboot or Turn Off Devices Unless Instructed.** This preserves volatile evidence. If a system must be rebooted for safety, document it thoroughly.
    4.  **Isolate, Don't Eliminate:** Disconnect the affected system from the network if it can be done safely without impacting vessel operations (e.g., unplugging a non-critical PC's network cable).

#### **Phase 3: Containment (Stopping the Spread)**

The goal is to prevent the incident from escalating while maintaining safe vessel operations.

*   **Short-Term Containment (At Sea):**
    *   **Network Segmentation:** Isolate critical networks from non-critical ones. For example, ensure the Crew Wi-Fi network is disconnected from the Ship's Operational Network.
    *   **Manual Override:** If an OT system is behaving erratically (e.g., steering, propulsion), switch to manual/local control if possible. This is a safety-critical decision made by the Captain and Chief Engineer.
    *   **Blocking:** If the source is known (e.g., a malicious IP address), block it at the ship’s firewall (if available).
*   **Long-Term Containment (Often in Port):**
    *   Systematically identify and isolate all affected systems. This may require a specialist team to come on board.

#### **Phase 4: Eradication (Removing the Threat)**

This involves eliminating the root cause of the incident.

*   **Maritime Challenges:** This is extremely difficult to do at sea. Eradication often has to wait until the vessel reaches a port with expert support.
*   **Actions:**
    *   **Remove Malware:** Use antivirus tools on sanitized systems or run specialized removal scripts.
    *   **Disable Breached Accounts:** Change all passwords, especially for administrative accounts.
    *   **Rebuild Systems:** The most effective method is to wipe the affected system and restore it from a known-good, pre-incident backup. This highlights the importance of having reliable, offline backups.

#### **Phase 5: Recovery (Restoring Normal Operations)**

This phase focuses on bringing systems back online safely.

*   **Maritime Actions:**
    *   **Phased Restoration:** Bring critical systems back online first (e.g., Navigation, then Propulsion Control, then Cargo systems).
    *   **Validation:** Before fully integrating a restored system, test it in a controlled manner. For example, check the GPS input to the ECDIS is valid before re-engaging the autopilot.
    *   **Monitoring:** Intensely monitor the restored systems for any sign of reinfection or abnormal behavior. This may continue for days or weeks.

#### **Phase 6: Lessons Learned (Post-Incident Activity)**

This is a formal process to improve future resilience.

*   **Investigation Report:** Create a detailed report covering:
    *   Timeline of the incident.
    *   Root cause analysis (how did the attacker get in?).
    *   Impact on vessel operations, safety, and business.
    *   Effectiveness of the response.
    *   Recommendations for improvement.
*   **Reporting:**
    *   **Internal:** Share lessons with the entire fleet.
    *   **External:** Report the incident to the Flag State, insurers (P&I Club), and potentially Port State Control or law enforcement, as required by law and policy. Sharing anonymized data with an industry ISAC (Information Sharing and Analysis Center) helps protect others.
*   **Update Plans:** Update the Ship Cyber Security Plan, crew training modules, and technical defenses based on the findings.

---

### **Digital Forensics: Key Considerations for Evidence Collection**

Forensic investigation aims to collect and preserve evidence in a way that is admissible in legal proceedings.

1.  **Preserve the Scene:** The crew's main forensic duty is preservation.
    *   **Photograph/Video:** Take pictures of screens (especially ransom notes), connected cables, and the physical environment.
    *   **Isolate the Device:** If a PC is the target, leave it on but disconnect its network cable.
    *   **VDR Data:** The Voyage Data Recorder contains critical navigation, communication, and bridge audio data. The master must take steps to **save the VDR data** immediately to prevent it from being overwritten.
2.  **Chain of Custody:** This is a log that tracks the evidence from the moment of collection. Every person who handles the evidence (e.g., a hard drive) must sign for it. This is vital for legal admissibility.
3.  **Data Acquisition:** This is typically performed by specialists.
    *   **Volatile Data:** Capturing data from system memory (RAM) is the first priority, as it contains running processes, network connections, and encryption keys. This is often lost on reboot.
    *   **Non-Volatile Data:** Creating a forensic image (a bit-for-bit copy) of hard drives and other storage media using a write-blocker to ensure the original is not altered.
    *   **Log Files:** Collect logs from firewalls, servers, network switches, and individual applications.

By understanding these unique challenges and following a structured, maritime-specific plan, shipping companies can effectively investigate and respond to cyber incidents, minimizing the impact on safety, the environment, and their operations.