---
title: Maritime Cyber Security :recovery plan
type: docs
sidebar:
  open: true
---

Of course. A Maritime Cyber Security Recovery Plan is a critical component of a vessel's or company's Safety Management System (SMS), as mandated by the IMO 2021 (MSC.428(98)) regulations. It's not just about restoring IT systems; it's about ensuring the safety of the crew, vessel, cargo, and the environment after a cyber incident.

Here is a comprehensive framework for developing a Maritime Cyber Security Recovery Plan, broken down into key components, specific scenarios, and best practices.

---

### **Maritime Cyber Security Recovery Plan: A Framework**

This plan outlines the procedures to recover from a cyber incident, restore critical systems, and return to normal operations in a safe and timely manner.

#### **1. Core Principles**

*   **Safety First:** The safety of life at sea, the vessel, and the marine environment is the absolute priority. All recovery actions must be evaluated against this principle.
*   **OT before IT:** Operational Technology (OT) systems (e.g., propulsion, navigation, steering) take precedence over Information Technology (IT) systems (e.g., crew email, business networks).
*   **Resilience over Restoration:** The primary goal is to maintain essential functions, even if in a degraded or manual mode. Full restoration is a secondary goal.
*   **Clear Chain of Command:** A clear command structure, both onboard and ashore, is essential to prevent confusion during a crisis.

---

### **Key Components of the Recovery Plan**

A robust plan should be a formal, controlled document and include the following sections.

#### **Section A: Introduction & Scope**

*   **Purpose:** State the plan's objective: to guide recovery efforts following a cyber incident.
*   **Scope:** Define which vessels, systems, and shore-side facilities this plan covers. Specify if it applies to IT, OT, or both.
*   **Activation Criteria:** Clearly define what constitutes a "cyber incident" that triggers this plan (e.g., ransomware on a critical system, loss of GPS signal, unresponsive engine controls).

#### **Section B: Roles and Responsibilities (The Cyber Recovery Team)**

This is the most critical section. Everyone must know their role.

| Role | Onboard/Ashore | Key Responsibilities |
| :--- | :--- | :--- |
| **Ship Master** | Onboard | Overall commander of the incident response on the vessel. Makes final decisions regarding safety and manual operations. |
| **Chief Engineer** | Onboard | Leads recovery efforts for all OT systems (propulsion, power management, ballast, etc.). |
| **Navigational Officer** | Onboard | Leads recovery for navigation systems (ECDIS, GPS, Radar). Responsible for initiating manual/alternative navigation. |
| **Company Security Officer (CSO)** | Ashore | Overall coordinator of the recovery effort, liaising between the vessel, management, and external parties. |
| **IT/OT Superintendent** | Ashore | The technical lead for the recovery. Guides onboard crew, coordinates with vendors, and manages backup restoration. |
| **Communications Lead** | Ashore | Manages all external communications (Flag State, Port State, insurers, charterers, media). |

#### **Section C: Recovery Phases (The Action Plan)**

This is the step-by-step process to follow once the plan is activated.

**Phase 1: Initial Assessment & Damage Control**
*   **Isolate:** Immediately disconnect the affected system(s) from the network to prevent the incident from spreading. This could mean physically unplugging network cables from critical equipment.
*   **Assess Impact:** Determine which systems are affected. The Master and Chief Engineer conduct a rapid assessment of OT systems.
*   **Activate Manual Overrides:** If automated controls are compromised, immediately switch to manual or emergency backup controls (e.g., manual steering, local engine control).
*   **Report:** The Master reports the incident to the CSO ashore using a reliable, out-of-band communication method (e.g., Satphone).

**Phase 2: System Triage & Prioritization**
Not all systems are equal. Recovery must be prioritized.

1.  **Tier 1 (Mission Critical):** Systems essential for safety and propulsion.
    *   Navigation (GPS, ECDIS, Gyro)
    *   Steering & Propulsion Control
    *   Power Management & Generation
    *   Onboard Safety & Alarm Systems
2.  **Tier 2 (Operation Critical):** Systems for efficient operation.
    *   Cargo Management (pumps, cranes, monitoring)
    *   Ballast Water Systems
    *   GMDSS (Global Maritime Distress and Safety System)
3.  **Tier 3 (Business Support):** Systems for administrative tasks.
    *   Crew Welfare Networks (Wi-Fi)
    *   Vessel Business LAN
    *   Administrative Software

**Phase 3: Restoration & Recovery**
*   **Use the Recovery Kit:** Access the pre-prepared "Cyber Recovery Kit," which should contain:
    *   Clean, tested backups of system software and configurations on isolated storage (e.g., encrypted USBs, DVDs).
    *   System installation media and license keys.
    *   Network diagrams and system manuals (in print!).
    *   Contact lists for vendors and support.
*   **Wipe & Rebuild (if necessary):** For compromised systems, the safest method is often to wipe the system completely and reinstall from a known-good, "golden" image or backup.
*   **Restore from Backup:** Restore data from the most recent, clean backup. Adhere to the pre-defined **Recovery Point Objective (RPO)**—the maximum acceptable amount of data loss.
*   **Patch & Harden:** Before reconnecting the system to any network, ensure all available security patches are applied.

**Phase 4: Verification & Monitoring**
*   **Test in Isolation:** Test the restored system thoroughly while it is still isolated from the network.
*   **Supervised Reconnection:** Reconnect the system to the network under close supervision. Monitor for any signs of reinfection or abnormal behavior.
*   **Full Functional Test:** The crew performs a full functional test to confirm the system is operating per specifications. For example, testing the ECDIS by plotting a test route.

**Phase 5: Post-Incident Activities**
*   **Declare "All Clear":** The Master and CSO formally declare the recovery complete and the vessel returned to normal operations.
*   **Forensic Analysis:** Preserve evidence (infected drives, log files) for later forensic analysis to understand the attack's root cause.
*   **Lessons Learned:** Conduct a debriefing session with all involved parties. Update the recovery plan based on what worked and what didn't.
*   **Formal Reporting:** Submit required reports to Flag State, insurers, and other relevant authorities.

---

### **Scenario-Specific Recovery Strategies**

**Scenario 1: Ransomware on the Cargo Management System**
*   **Impact:** Inability to monitor or control cargo pumps, valves, or tank levels. High commercial and environmental risk.
*   **Recovery Steps:**
    1.  **Isolate:** Immediately disconnect the cargo computer from the network.
    2.  **Manual Ops:** Switch all cargo operations to local, manual control at the pump/valve stations.
    3.  **Do Not Pay:** Follow company policy, which should be to *never* pay the ransom.
    4.  **Restore:** Use the ashore IT/OT team to guide the crew. Wipe the affected machine and restore the operating system and software from the Cyber Recovery Kit. Restore cargo data from the last known-good backup.
    5.  **Verify:** Before resuming automated operations, run a full diagnostic and test all sensors and actuators.

**Scenario 2: GPS/GNSS Spoofing or Jamming**
*   **Impact:** Loss of position fixing, erroneous vessel position on ECDIS, potential for collision or grounding.
*   **Recovery Steps:**
    1.  **Alert:** The Bridge team immediately alerts the Master.
    2.  **Verify:** Cross-reference position with other means: Radar overlay on charts, visual bearings, celestial navigation (if trained).
    3.  **Manual Plotting:** Revert to plotting the vessel's position on paper charts.
    4.  **Communicate:** Inform VTS (Vessel Traffic Services) and nearby ships of the navigation difficulty.
    5.  **Isolate:** If spoofing is suspected, disconnect the GPS antenna from the network to prevent the false signal from propagating to other systems (e.g., AIS, GMDSS).

**Scenario 3: Malware in the Engine Control System (OT)**
*   **Impact:** The most dangerous scenario. Loss of propulsion control, erratic engine behavior, potential for catastrophic failure.
*   **Recovery Steps:**
    1.  **Emergency Stop/Control:** Immediately transfer control to the Emergency Telegraph or Local Control Station in the engine room. This decouples the bridge controls from the engine.
    2.  **Isolate:** Power down and physically disconnect the affected control consoles and PLCs from the network.
    3.  **DO NOT ATTEMPT IT FIXES:** The engineering crew should **not** attempt to "clean" the system with standard antivirus. This is a specialist OT task.
    4.  **Contact Vendor:** The ashore team must contact the engine manufacturer/automation vendor for emergency support. Their technicians will have the proprietary tools and knowledge to safely restore the system.
    5.  **Restore:** The vendor will likely have to perform a low-level format and reinstall the proprietary firmware from a clean source.

---

### **Best Practices for a Successful Plan**

*   **Test, Test, Test:** A plan that hasn't been tested is a plan that will fail. Conduct regular drills and tabletop exercises, both onboard and with the shore team.
*   **Keep it Simple:** The plan should be clear, concise, and easy to follow by a crew under immense stress. Use checklists and flowcharts.
*   **Make it Accessible:** Keep printed copies in secure, accessible locations (Bridge, Engine Control Room, Company Office). Digital copies may be inaccessible during an incident.
*   **Integrate with SMS:** The Cyber Recovery Plan must be a living document, fully integrated with the ship's existing Safety Management System and emergency procedures.
*   **Maintain Your Backups:** Backups are the cornerstone of recovery. Test them regularly to ensure they can be restored successfully. Follow the 3-2-1 rule: 3 copies of your data, on 2 different media, with 1 copy off-site (or off-system).