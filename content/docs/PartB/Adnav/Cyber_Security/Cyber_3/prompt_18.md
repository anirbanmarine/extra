---
title: Maritime Cyber Security :risk assessment made by the company
type: docs
sidebar:
  open: true
---

Of course. A maritime company's cyber security risk assessment is a critical process for ensuring the safety, security, and operational continuity of its vessels and business. It's not a one-time event but a continuous cycle mandated by regulations like the IMO's Resolution MSC.428(98).

Here is a detailed breakdown of how a maritime company would conduct this risk assessment, from process and tools to the people involved.

---

### **Maritime Cyber Security: A Company's Risk Assessment Framework**

The primary goal is to identify, analyze, and evaluate cyber risks to the company's Information Technology (IT) and, most critically, its Operational Technology (OT) systems, both onboard vessels and ashore.

The process generally follows a standard risk management lifecycle, adapted for the unique maritime environment.

#### **Phase 1: Preparation and Scoping**

**Objective:** Define the scope and context of the assessment.

1.  **Form a Cross-Functional Team:** This is not just an IT task. The team must include:
    *   **IT Department:** For corporate networks, email, and business systems.
    *   **OT/Engineering Department:** The Chief Engineer and technical superintendents who understand the vessel's machinery and control systems.
    *   **Deck Department/Operations:** Captains and Chief Mates who operate bridge systems.
    *   **Senior Management/DPA (Designated Person Ashore):** To ensure support, provide resources, and integrate the assessment into the company's Safety Management System (SMS).
    *   **Crewing/HR:** To address training and personnel-related risks.

2.  **Define Scope:** The company must decide what's in scope. This will always include:
    *   **Vessels:** Specific ships or the entire fleet.
    *   **Shore-based Offices:** Head office, port offices.
    *   **Third-party Connections:** Vendors, port authorities, classification societies.

3.  **Adopt a Framework:** Companies don't start from scratch. They typically base their assessment on established guidelines, such as:
    *   **The Guidelines on Cyber Security Onboard Ships (BIMCO, CLIA, etc.)**
    *   **NIST Cybersecurity Framework (Identify, Protect, Detect, Respond, Recover)**
    *   **ISO/IEC 27001 (Information Security Management)**

---

#### **Phase 2: Asset, Threat, and Vulnerability Identification**

**Objective:** Create a comprehensive inventory of what needs protection and what could harm it.

1.  **Identify Critical Systems (Asset Inventory):** The team lists all systems where a cyber incident could have an impact. This is broken into two key categories:

    *   **Operational Technology (OT) - *Highest Priority***
        *   **Bridge Systems:** ECDIS (Electronic Chart Display), GPS/GNSS, AIS (Automatic Identification System), RADAR/ARPA.
        *   **Propulsion & Machinery Management:** Main engine controls, power management, ballast water systems.
        *   **Cargo Management Systems:** Crane controls, tank level monitoring, reefer container controls.
        *   **Safety & Security Systems:** CCTV, vessel access control systems.

    *   **Information Technology (IT)**
        *   **Shipboard Networks:** Crew Wi-Fi, business LAN.
        *   **Communication Systems:** Satellite comms (VSAT), FleetBroadband.
        *   **Administrative Systems:** E-logs, planned maintenance systems (PMS), crew/portage management software.
        *   **Shore-based Systems:** Chartering software, financial systems, corporate email.

2.  **Identify Threats:** What are the potential sources of harm?
    *   **Malicious/External:** Hackers, cyber-criminals (ransomware), state-sponsored actors, activists.
    *   **Malicious/Internal:** Disgruntled current or former employees/crew.
    *   **Non-Malicious/Unintentional:** Untrained crew clicking a phishing link, a technician using an infected USB drive for a software update, a misconfigured firewall.
    *   **System Failures:** Software bugs, hardware failure, power loss.

3.  **Identify Vulnerabilities:** How could a threat compromise an asset?
    *   **Technical Vulnerabilities:**
        *   Outdated software/firmware on ECDIS or engine controls (unpatched systems).
        *   Lack of network segmentation between the crew network and critical bridge systems.
        *   Weak or default passwords on equipment.
        *   Unsecured remote access points used by vendors for maintenance.
        *   Reliance on unencrypted GPS signals (vulnerable to spoofing).
    *   **Procedural/Human Vulnerabilities:**
        *   Lack of crew awareness and training on cyber hygiene.
        *   Uncontrolled use of USB sticks.
        *   No formal policy for software updates or system changes.
        *   Inadequate background checks for personnel with high-level access.

---

#### **Phase 3: Risk Analysis and Evaluation**

**Objective:** Determine the level of risk for each identified scenario.

The company uses a formula: **Risk = Likelihood x Impact**

1.  **Analyze Impact:** If an incident occurs, what are the consequences? Impact is rated on several scales (e.g., from 1-5, Negligible to Catastrophic).
    *   **Safety:** Injury or loss of life (e.g., collision from GPS spoofing, loss of propulsion).
    *   **Environmental:** Pollution (e.g., manipulation of ballast water or cargo systems).
    *   **Operational:** Vessel downtime, delivery delays, charter party breaches.
    *   **Commercial/Financial:** Data theft (cargo manifests), financial fraud, cost of remediation, ransomware payments.
    *   **Reputation:** Loss of customer trust, negative media attention.

2.  **Analyze Likelihood:** How likely is it that the vulnerability will be exploited by the threat? (e.g., from 1-5, Rare to Almost Certain). This is based on:
    *   Historical incident data (if any).
    *   Threat intelligence reports.
    *   The attractiveness of the company/vessel as a target.
    *   The level of existing security controls.

3.  **Evaluate and Prioritize Risk:** The results are plotted on a **Risk Matrix** (a heat map).

| **Likelihood**  | **Negligible** | **Minor** | **Moderate** | **Major** | **Catastrophic** |
| :-------------- | :------------- | :-------- | :----------- | :-------- | :--------------- |
| **Almost Certain**| Medium         | High      | High         | Critical  | Critical         |
| **Likely**      | Low            | Medium    | High         | High      | Critical         |
| **Possible**    | Low            | Medium    | Medium       | High      | High             |
| **Unlikely**    | Low            | Low       | Medium       | Medium    | High             |
| **Rare**        | Low            | Low       | Low          | Low       | Medium           |

Risks falling into the "High" and "Critical" categories become the top priority for treatment.

---

#### **Phase 4: Risk Treatment**

**Objective:** Implement measures to control the prioritized risks.

For each high-priority risk, the company decides on a treatment strategy:

1.  **Mitigate (Reduce):** This is the most common strategy. The company implements security controls.
    *   **Technical Controls:**
        *   Install firewalls and segment networks (e.g., physically separating the bridge network from the crew network).
        *   Implement a robust patching program for all OT and IT software.
        *   Enforce strong password policies and multi-factor authentication.
        *   Deploy endpoint protection (antivirus) on applicable systems.
        *   Use encrypted communication channels.
    *   **Procedural Controls:**
        *   Develop and enforce a strict policy on USB and removable media usage.
        *   Conduct mandatory, regular cyber security awareness training for all crew and shore staff.
        *   Create and drill an **Incident Response Plan**. Who does the Captain call? What are the first steps?
        *   Implement a formal process for managing remote access by third-party vendors.

2.  **Transfer (Share):** Transferring some of the financial impact of a risk.
    *   **Action:** Purchase a specific cyber security insurance policy. This doesn't reduce the likelihood, but it helps with the financial recovery.

3.  **Accept:** If the cost of mitigation is higher than the potential impact, and the risk is low, the company may formally accept it. This decision must be documented and approved by senior management.

4.  **Avoid:** Stop doing the activity that causes the risk. (e.g., decommissioning a vulnerable legacy system and replacing it with a secure alternative).

---

#### **Phase 5: Documentation and Monitoring (The Living Process)**

**Objective:** Maintain a record of the assessment and continuously monitor the environment.

1.  **The Risk Register:** This is the key output document. It's a spreadsheet or database that lists every identified risk and includes:
    *   Risk ID & Description
    *   Affected Asset(s)
    *   Likelihood & Impact scores
    *   Overall Risk Level (Low, Medium, High, Critical)
    *   Treatment Plan (e.g., "Implement network segmentation by Q4")
    *   Risk Owner (e.g., "Technical Superintendent")
    *   Status (Open, In Progress, Closed)

2.  **Continuous Monitoring:** The threat landscape is always changing. The company must:
    *   **Review the risk assessment annually** or whenever there is a significant change (e.g., new vessel acquisition, new critical system installed).
    *   **Conduct regular vulnerability scans** and penetration tests.
    *   **Stay updated on threat intelligence** specific to the maritime sector.
    *   **Review and update the Incident Response Plan** after drills or actual incidents.

This entire process is integrated into the ship's **Safety Management System (SMS)**, making cyber security an integral part of the vessel's overall safety culture, not just an IT problem.