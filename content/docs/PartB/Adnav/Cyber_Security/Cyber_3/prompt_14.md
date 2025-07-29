---
title: Maritime Cyber Security :establish contingency plans
type: docs
sidebar:
  open: true
---

Of course. Establishing robust contingency plans is a critical and mandatory component of maritime cyber risk management, as required by IMO Resolution MSC.428(98). A well-structured contingency plan ensures that a vessel or facility can respond effectively to a cyber incident, prioritizing safety, environmental protection, and operational continuity.

Here is a comprehensive guide to establishing maritime cyber security contingency plans, broken down into a framework, key components, and specific scenarios.

---

### **Framework for Establishing Contingency Plans**

A contingency plan shouldn't be a standalone document. It must be integrated into the existing Safety Management System (SMS) for vessels and the Port Facility Security Plan (PFSP) for ports. The process follows the classic risk management cycle: **Identify -> Protect -> Detect -> Respond -> Recover.** The contingency plan is the heart of the **Respond** and **Recover** phases.

#### **Step 1: Form a Cross-Functional Team**
You cannot create this plan in an IT silo. The team must include:
*   **Onshore:** Company Security Officer (CSO), Designated Person Ashore (DPA), IT/OT Manager, Fleet Superintendent.
*   **Onboard:** Master (Captain), Chief Engineer, Chief Officer, Electro-Technical Officer (ETO).
*   **For Ports:** Port Facility Security Officer (PFSO), Harbour Master, Operations Manager, IT/OT specialists.

#### **Step 2: Conduct a Cyber Risk Assessment**
Before you can plan for contingencies, you must know what you're planning for.
*   **Identify Critical Systems:** List all systems whose failure or compromise would threaten safety, operations, or the environment.
    *   **Navigation:** GPS/GNSS, ECDIS, RADAR/ARPA, AIS.
    *   **Propulsion & Machinery:** Engine Control System, Power Management, Steering Gear.
    *   **Cargo Management:** Ballast Water Treatment System (BWTS), Tank Level Gauges, Crane/Ramp Controls.
    *   **Communications:** GMDSS, Satellite Communications (VSAT).
    *   **Crew & Admin:** Crew Management Systems, Ship's Business Network.
*   **Identify Threats:** Map potential cyber threats to these systems (e.g., malware, ransomware, phishing, GPS spoofing, insider threat).
*   **Determine Impact:** For each threat/system combination, define the potential consequences (e.g., loss of position, collision, oil spill, financial loss).

#### **Step 3: Define Activation Triggers**
The plan must clearly state **when** it should be activated. An incident is not just a successful attack; it can be a suspected event. Triggers could include:
*   Unexplained loss of a critical signal (e.g., GPS).
*   Unresponsive or erratic behavior of control systems (e.g., ECDIS, Engine Control).
*   A ransomware message appearing on a screen.
*   Discovery of unauthorized devices connected to the network.
*   Alerts from cybersecurity monitoring software.
*   Credible threat intelligence received from authorities.

---

### **Key Components of a Maritime Cyber Contingency Plan**

Your documented plan should be clear, concise, and actionable, even under extreme stress. Use checklists and simple language.

#### **1. Roles and Responsibilities (The Cyber Response Team)**
Define a clear chain of command for a cyber incident.
*   **Incident Commander (Master/PFSO):** Has overall command. Focuses on the safety of the crew, vessel, and environment. Makes the final decisions on operational responses (e.g., shifting to manual control, aborting maneuvers).
*   **Technical Lead (ETO/IT Officer):** Leads the technical investigation and response. Responsible for isolating systems, preserving evidence, and restoration.
*   **Operations Lead (Chief Engineer/Chief Officer):** Manages the physical response. Organizes the shift to manual/backup operational modes for machinery, navigation, and cargo.
*   **Communications Lead (Onshore CSO/DPA):** Manages all external and internal communications to prevent misinformation and panic.

#### **2. Immediate Actions (The First 30 Minutes)**
This is the "first aid" section. Actions must be reflexive and well-rehearsed.
*   **ASSESS:** What is the immediate safety or environmental impact?
*   **ISOLATE:** Disconnect the affected system from the network to prevent the threat from spreading. **This is the single most important immediate action.** This could mean physically unplugging network cables from a bridge console or server rack.
*   **SHIFT TO MANUAL/BACKUP:** Immediately revert to backup or manual control procedures for affected critical systems. (e.g., switch from ECDIS to paper charts, use manual engine controls).
*   **INFORM:** The Master immediately informs the Company Security Officer (CSO) / Designated Person Ashore (DPA).

#### **3. Communication Plan**
Define who to contact, when, and what to say.
*   **Internal:** Crew, company management.
*   **External (as required):**
    *   **Flag State:** Mandatory reporting.
    *   **Port State / Coastal State:** Especially if the incident affects navigational safety.
    *   **Classification Society:** If the integrity of certified systems is affected.
    *   **Insurers (P&I, H&M):** To ensure coverage is not voided.
    *   **Third-Party Responders:** Cybersecurity firms, equipment manufacturers.
    *   **Cargo Owners/Charterers:** If cargo operations or delivery schedules are impacted.
*   **Have pre-drafted message templates ready.**

#### **4. Technical Response & Recovery Procedures**
This section provides specific guidance for the Technical Lead.
*   **Evidence Preservation:** Do not immediately wipe and restore. Take forensic images of affected hard drives or memory if possible. Document everything with photos and logs.
*   **Identification:** Determine the nature of the attack (malware, DoS, etc.).
*   **Eradication:** Remove the threat from the system.
*   **Recovery:**
    *   Restore systems from clean, trusted backups.
    *   Verify that the system is fully functional and the data is correct before reconnecting it to the network.
    *   If no backups exist, the plan must outline procedures for a full system rebuild, including sourcing software from original manufacturers.

#### **5. Post-Incident Review**
*   Conduct a "lessons learned" analysis after every incident or drill.
*   What went well? What didn’t?
*   Update the contingency plan, risk assessment, and crew training based on the findings.

---

### **Scenario-Specific Contingency Playbooks (Mini-Plans)**

For high-impact scenarios, create simple, one-page playbooks.

#### **Scenario 1: GPS/GNSS Jamming or Spoofing**
*   **Detection:**
    *   Alarm on GPS unit ("Lost Signal" or "Low Accuracy").
    *   Vessel position on ECDIS/RADAR does not match visual or other indicators.
    *   Drastic, impossible jump in vessel position.
*   **Contingency Response:**
    1.  Master immediately notified.
    2.  Bridge team cross-references position using all available means:
        *   RADAR/ARPA bearings and ranges to fixed objects.
        *   Visual bearings to land/buoys.
        *   Echo sounder readings compared to chart depths.
        *   Celestial navigation (if trained and equipped).
    3.  Report to coastal authorities (e.g., USCG) about suspected jamming.
    4.  Log the event in detail.

#### **Scenario 2: Ransomware on the Bridge ECDIS**
*   **Detection:**
    *   Ransom note displayed on the ECDIS screen.
    *   System is locked and unresponsive.
*   **Contingency Response:**
    1.  **Do NOT pay the ransom.**
    2.  **Isolate:** Immediately disconnect the ECDIS terminal(s) from the ship's network (unplug Ethernet cables).
    3.  **Shift to Backup:** Immediately switch to the backup ECDIS terminal. If both are affected, revert to the official, corrected inventory of **paper charts**.
    4.  Master informs CSO/DPA.
    5.  Technical Lead prepares to restore the system from a clean backup once operationally safe to do so.

#### **Scenario 3: Malware in the Cargo/Ballast Water Control System**
*   **Detection:**
    *   Valves opening/closing without command.
    *   Tank level readings are erratic or incorrect.
    *   System alarms are triggered for no reason.
*   **Contingency Response:**
    1.  Chief Officer/Engineer immediately informed.
    2.  **Isolate:** Disconnect the control system's computer from the network.
    3.  **Shift to Manual:** Use local, manual overrides at the pump room or valve stations.
    4.  Manually verify all tank levels and valve positions ("walking the deck").
    5.  Suspend all cargo/ballast operations until the system is verified as safe and under control.

### **Training, Testing, and Maintenance**

A plan is useless if it sits on a shelf.
*   **Training:** All crew members must be trained on their specific roles in the plan and on general cyber hygiene.
*   **Drills & Exercises:** Regularly test the plan through:
    *   **Tabletop Exercises:** Talk through a scenario in a conference room.
    *   **Live Drills:** Simulate a real event (e.g., unplug the primary GPS and force the bridge team to use backups).
*   **Plan Maintenance:** Review and update the contingency plan annually, after any incident, or whenever a new critical system is installed. Ensure contact lists are always up-to-date.