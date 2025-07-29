---
title: Maritime Cyber security and safety management:phishing, risks regarding removable
  media;
type: docs
sidebar:
  open: true
---

Of course. This is a critical topic in the modern maritime industry. The integration of cyber security into the existing Safety Management System (SMS) framework is no longer optional; it's a mandatory requirement under IMO regulations.

Let's break down phishing and the risks of removable media within the maritime context and how they relate to safety management.

---

### **The Overall Context: Maritime Cyber Security and the Safety Management System (SMS)**

Before diving into the specifics, it's essential to understand the framework. The International Maritime Organization (IMO) Resolution **MSC.428(98)** mandates that cyber risks be appropriately addressed in a ship's Safety Management System (SMS) no later than the first annual verification of the company’s Document of Compliance after January 1, 2021.

This means cyber threats are no longer just an "IT problem"; they are a **safety problem**. A cyber-attack can lead to a physical event, such as a collision, grounding, pollution, or injury to the crew. Therefore, risks like phishing and malware from USB drives must be managed with the same rigor as risks like heavy weather or engine failure.

The core idea is to apply the existing ISM Code principles to cyber risks:
1.  **Identify** Threats (e.g., phishing, removable media).
2.  **Assess** Risks and Potential Impacts (e.g., loss of navigation, loss of propulsion).
3.  **Establish** Safeguards and Barriers (e.g., procedures, technical controls, training).
4.  **Respond** to Incidents.
5.  **Recover** from Incidents.

---

### **1. Phishing in the Maritime Context**

Phishing is the fraudulent attempt to obtain sensitive information such as usernames, passwords, and credit card details by disguising oneself as a trustworthy entity in an electronic communication. In the maritime world, these attacks are uniquely tailored and highly effective.

#### **How Phishing Works on a Ship or in a Shipping Company:**

Phishing attacks are successful because they exploit human psychology—urgency, trust, and curiosity.

*   **Targeting the Crew:** An attacker sends an email to the ship's general email address or a crew member's personal account.
    *   **Scenario:** An email disguised as being from "Crewing Services" with the subject "Urgent: Your Next Contract Details" or "Payroll Discrepancy." The email contains a link or an attachment that, when clicked, installs malware or directs the user to a fake login page to steal credentials.
    *   **Why it's effective:** Crew are often anxious for news about future assignments, pay, or family. They are a high-value target in a high-stress environment.

*   **Targeting Shore-Side Operations:** An attacker targets the ship's agent, charterer, or head office.
    *   **Scenario 1 (Invoice Fraud):** An email that looks like it's from a legitimate port agent or bunker supplier with a slightly altered invoice. The email asks the company to pay the bill to a new bank account. This is a common and costly form of phishing.
    *   **Scenario 2 (Official Documentation):** An email pretending to be from a Port State Control authority or Customs, with an attachment named "Updated Maritime Declaration of Health.zip" or "Port Arrival Forms.pdf". The file contains ransomware or a keylogger.

#### **The Risks to Safety and Operations:**

A successful phishing attack can bridge the gap between the ship's Information Technology (IT) systems (for email, admin) and its critical Operational Technology (OT) systems (for navigation, propulsion).

1.  **Compromise of IT Systems:**
    *   **Result:** Theft of credentials, loss of commercial data (cargo manifests, charter party agreements), financial fraud. While serious, this is primarily a business risk.

2.  **Crossover to OT Systems (The Critical Danger):**
    *   **The Path:** Malware from a phishing attack on an administrative computer could spread across the ship's network. If the networks are not properly segmented (separated), the malware could infect critical systems.
    *   **Safety Risk:**
        *   **ECDIS (Electronic Chart Display and Information System):** Manipulation of charts, deletion of routes, or system shutdown, leading to **grounding or collision**.
        *   **GPS/GNSS:** Spoofing or jamming of the ship's position data, making the ECDIS display a false position.
        *   **Engine Control & Monitoring:** Interference with engine RPM, fuel flow, or disabling safety alarms, potentially leading to **loss of propulsion or engine damage**.
        *   **Ballast Water & Cargo Systems:** Uncontrolled operation of pumps could affect the ship's stability, leading to **capsizing or structural failure**.

#### **Integration into SMS (Phishing):**

*   **Procedure:** A clear policy on handling unsolicited emails. "When in doubt, throw it out."
*   **Training:** Regular, practical training for both crew and shore staff. Use simulated phishing campaigns to test and educate users.
*   **Technical Controls:** Email filters, antivirus software, and crucially, **network segmentation** to keep the Bridge and Engine Control Room networks isolated from the general crew/admin network.

---

### **2. Risks Regarding Removable Media (USB Drives, SD Cards, etc.)**

Removable media is one of the most common vectors for introducing malware into a ship's systems, as it can bypass network firewalls entirely.

#### **How Removable Media Creates Risk on a Ship:**

*   **Crew's Personal Media:** This is the #1 threat. A crew member goes ashore to an internet café, downloads movies or music onto a USB drive, and then plugs it into a ship's computer (e.g., a recreation room PC or, worse, a multi-purpose PC on the bridge). The USB is likely infected with malware.
*   **Third-Party Technicians/Surveyors:** A technician from a manufacturer or a class surveyor may bring a USB drive with software updates or diagnostic tools. If their device is compromised, they can unintentionally infect the ship's systems.
*   **Official Updates:** Sometimes, official updates for systems like ECDIS are delivered on USB sticks. If this supply chain is compromised, it represents a direct attack on a critical navigation system.
*   **"Baiting":** Attackers may intentionally leave infected USB drives in ports or terminals, hoping a curious crew member will pick one up and plug it in.

#### **The Risks to Safety and Operations:**

The risks are very similar to phishing but can be even more direct, as the media might be plugged directly into an OT system.

1.  **Malware Infection (Ransomware):**
    *   **Scenario:** A USB drive infects the computer used for the ship's loading calculations. Ransomware encrypts all files, and the crew can no longer calculate stability, shear forces, or bending moments. The ship is unsafe to sail or conduct cargo operations until the system is restored. In 2020, a major cargo carrier was hit by ransomware that severely disrupted its global operations.
    *   **Safety Risk:** Loss of critical planning and safety calculation tools.

2.  **Bridging the "Air Gap":**
    *   **Scenario:** Many critical OT systems (like propulsion control) are "air-gapped," meaning they are not physically connected to any network. A USB drive completely defeats this protection. An engineer could use a USB to transfer a file from a networked PC to the air-gapped Engine Control Room maintenance laptop, introducing malware directly into the OT environment.
    *   **Safety Risk:** Direct compromise of machinery control, leading to **loss of power, propulsion, or steering**.

#### **Integration into SMS (Removable Media):**

*   **Policy:** A strict and simple policy is required.
    *   **Rule 1:** Absolutely **NO personal USB drives** are to be used in any ship computer connected to operational equipment (Bridge, ECR, Cargo Control Room).
    *   **Rule 2:** All **official/work-related USB drives** must be scanned for malware on a dedicated, isolated "quarantine" computer before being used.
*   **Procedure:** A clear, step-by-step procedure for handling any incoming media from technicians or for system updates.
*   **Technical Controls:**
    *   **Disabling USB Ports:** Physically or through software, disable USB ports on critical workstations (e.g., ECDIS, Machinery Control).
    *   **Antivirus:** Ensure all computers have up-to-date antivirus software with a specific function to automatically scan removable drives.
*   **Awareness:** Posters and briefings to constantly remind crew of the dangers. The message should be about protecting the ship and their colleagues, not just about following rules.