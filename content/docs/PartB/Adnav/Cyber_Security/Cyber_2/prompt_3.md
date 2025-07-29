---
title: 'Maritime Cyber security and safety management: dangers associated with emails
  (dangerous attachments, hoaxes, etc.);'
type: docs
sidebar:
  open: true
---

Of course. This is an excellent and critical topic. The integration of cyber security into the maritime Safety Management System (SMS), as mandated by the IMO, is crucial for modern vessel operations. Email remains one of the most significant and persistent threats.

Here is a detailed breakdown of the dangers associated with emails in the maritime context, structured for clarity within a safety management framework.

---

### **Maritime Cyber Security & Safety Management: Dangers Associated with Emails**

The International Safety Management (ISM) Code requires shipping companies to assess all identified risks to their ships, personnel, and the environment and to establish appropriate safeguards. Following IMO Resolution MSC.428(98), this now explicitly includes cyber risks. Email is a primary vector for these risks, capable of bridging the gap between shoreside IT systems and the vessel's critical Operational Technology (OT).

### **Why Email is a High-Risk Area in the Maritime Industry**

The maritime sector has unique vulnerabilities that amplify the danger of email-based threats:

*   **High "Trust" Environment:** Vessels constantly receive legitimate emails with attachments from port agents, charterers, suppliers, and manning agencies (e.g., berthing instructions, crew manifests, cargo documents). Attackers exploit this by creating convincing fakes.
*   **IT/OT Convergence:** An infected office computer (IT) on the bridge can potentially transfer malware to the ECDIS, cargo planning system, or engine control monitoring system (OT), often via a USB stick.
*   **Limited Onboard Expertise:** The crew are maritime professionals, not necessarily IT security experts. They may not be trained to spot sophisticated phishing attempts.
*   **Intermittent & Low-Bandwidth Connectivity:** Satellite connections can make it difficult to receive large security updates or use cloud-based scanning services effectively, leaving systems vulnerable.
*   **Crew Rotation:** A constantly changing crew increases the challenge of maintaining a consistent security culture and training standard.

---

### **Specific Dangers Associated with Emails**

#### **1. Dangerous Attachments (Malware Delivery)**

This is the most direct method of attack. The goal is to trick a user into opening an attachment that executes malicious code.

*   **Payloads:**
    *   **Ransomware:** This is a top threat. The malware encrypts critical files on a computer or network (e.g., cargo loading computer, administrative files). The attackers then demand a ransom, usually in cryptocurrency, for the decryption key.
        *   **Maritime Impact:** A locked cargo computer could delay port operations, costing thousands of dollars per hour. A locked ECDIS could render the primary means of navigation unusable, creating a major safety hazard.
    *   **Spyware/Keyloggers:** This software secretly records keystrokes, screenshots, and other user activity.
        *   **Maritime Impact:** Can capture login credentials for vessel management portals, financial systems, or secure communication platforms, leading to data breaches or financial fraud.
    *   **Trojans & Worms:** Trojans disguise themselves as legitimate software, creating a "backdoor" for attackers to access the system. Worms can self-replicate and spread across the vessel's network without human interaction.
        *   **Maritime Impact:** Can spread from the ship's business LAN to critical systems if networks are not properly segmented, potentially compromising navigation or machinery control systems.

*   **Common Malicious File Types:**
    *   **Executable Files:** `.exe`, `.scr`, `.bat` (Often disguised with a fake icon, like a PDF or Word document).
    *   **Compressed Files:** `.zip`, `.rar` (Used to hide malicious files from basic email scanners).
    *   **Microsoft Office Documents with Macros:** `.docm`, `.xlsm` (A very common method. The document prompts the user to "Enable Content" to view it properly, which executes a malicious script).
    *   **Image or PDF Files:** Can contain embedded malware that exploits vulnerabilities in the viewing software.

#### **2. Phishing and Social Engineering**

Phishing attacks use deceptive emails to trick the recipient into revealing sensitive information or taking a harmful action.

*   **Types of Phishing:**
    *   **General Phishing:** A mass email sent to many recipients with a generic message (e.g., "Your mailbox is full, click here to upgrade").
    *   **Spear Phishing (Highly Dangerous):** A targeted, well-researched attack on a specific person or vessel. The email will appear to be from a known, trusted source and contain specific, plausible information.
        *   **Maritime Example:** An email sent to a ship's Master, appearing to be from the port agent of the next port of call. The subject might be "URGENT: Revised Pilot Boarding Instructions" and contain a malicious Word document attachment.
    *   **Whaling:** Spear phishing aimed at senior executives (e.g., the CEO or CFO of the shipping company).

*   **The Goal:**
    *   **Credential Harvesting:** The email contains a link to a fake login page (e.g., a fake Microsoft Office 365 or company portal login). Once the user enters their username and password, the attacker captures it.
    *   **Instilling Urgency:** Phishing emails often use language like "Urgent," "Final Notice," or "Security Alert" to rush the recipient into making a mistake without thinking.

#### **3. Business Email Compromise (BEC)**

This is a sophisticated scam targeting companies that perform wire transfers. It's a form of spear phishing that has cost the shipping industry millions.

*   **The Scenario:**
    1.  An attacker compromises the email account of a supplier, port agent, or even someone within the shipping company.
    2.  They monitor email exchanges to understand billing cycles and relationships.
    3.  At the right moment, they send an email from the compromised (or a very similar, spoofed) address, instructing the accounts department to send payment for a legitimate invoice to a new, fraudulent bank account.

*   **Maritime Impact:** Direct and significant financial loss. This can involve payments for bunker fuel, port fees, or ship supplies being diverted to criminals.

#### **4. Hoaxes and Scams**

While some hoaxes don't contain malware, they are still a threat to safety and operations.

*   **Purpose:** To spread misinformation, cause panic, or waste time and resources.
*   **Maritime Examples:**
    *   A fake security alert about a new pirate action group in a specific area, causing a vessel to deviate from its route unnecessarily.
    *   A chain email with false information about new crew visa regulations, causing administrative chaos ashore and onboard.
    *   "Virus" hoaxes that instruct the user to delete essential system files, believing they are removing a threat.
*   **Impact:** Can clog limited satellite bandwidth, cause operational disruptions based on false information, and reduce vigilance by creating "alert fatigue."

---

### **Integration with the Safety Management System (SMS): Mitigation Strategies**

Cyber risks from emails must be managed with the same rigor as traditional maritime risks (e.g., fire, collision).

1.  **Risk Assessment:**
    *   **Identify Threats:** Recognize that emails are a primary attack vector.
    *   **Identify Vulnerabilities:** Acknowledge lack of crew training, flat networks (no separation between IT and OT), and reliance on trusted communications.
    *   **Assess Impact:** Determine the potential consequences: loss of navigation, propulsion, cargo data, financial loss, reputational damage, and port state control detention.

2.  **Procedures and Policies (The "How-To" Guide):**
    *   **Email Handling Policy:**
        *   NEVER open attachments from unknown or unsolicited senders.
        *   ALWAYS verify unexpected instructions or changes to payment details via a secondary method (e.g., a phone call to a known number).
        *   Disable macros from running by default in Microsoft Office.
        *   Scan all attachments before opening, especially those transferred via USB.
    *   **Incident Response Plan:** A clear, step-by-step plan for what to do if a suspicious email is received or a potential infection occurs. Who does the crew member report it to immediately (e.g., DPA, IT department)?

3.  **Technical Controls:**
    *   **Email Filtering:** Use advanced spam and phishing filters on the shore-side mail server.
    *   **Antivirus/Anti-Malware:** Ensure all onboard computers have up-to-date antivirus software.
    *   **Network Segmentation:** This is CRITICAL. Isolate the critical OT systems (ECDIS, engine control) from the business/crew welfare LAN. Data transfer between them should be strictly controlled (e.g., via a single, hardened "DMZ" computer).

4.  **The Human Element (The "Human Firewall"):**
    *   **Training & Awareness:** This is the most effective defense. Conduct regular, practical training for all crew and shore staff. Use real-world maritime examples.
    *   **Phishing Simulations:** Send fake (but safe) phishing emails to crew and staff. This provides a safe way to test and improve their awareness and reporting skills.
    *   **Promote a "No-Blame" Culture:** Encourage crew to report suspicious emails or mistakes (like clicking a bad link) immediately without fear of punishment. Early reporting is key to containing a breach.

By treating email-based cyber threats as a core safety issue within the SMS, shipping companies can move from a reactive to a proactive posture, protecting their vessels, crew, cargo, and reputation in an increasingly connected world.