---
title: Maritime Cyber Security :onboard networks
type: docs
sidebar:
  open: true
---

Of course. This is a critical and rapidly evolving area. Here is a comprehensive overview of Maritime Cyber Security focusing specifically on **onboard networks**.

---

### **Maritime Cyber Security: Securing Onboard Networks**

Historically, ship systems were isolated, mechanical, and standalone. Today, modern vessels are highly sophisticated floating data centers with interconnected networks. This "digitalization" has brought immense efficiency and safety gains but has also introduced significant cyber vulnerabilities. Securing these onboard networks is no longer an IT issue; it is a fundamental aspect of vessel safety, security, and operational integrity.

The core challenge lies in the **convergence of Information Technology (IT) and Operational Technology (OT)** in a unique, remote, and often harsh environment.

---

### **1. The Two Worlds of Onboard Networks: IT vs. OT**

Understanding the distinction between these two network types is the first step to securing them.

#### **A. Information Technology (IT) Networks**
These are the systems that manage data and are similar to a typical office environment.

*   **Purpose:** Business and crew welfare.
*   **Systems Include:**
    *   Crew and Passenger Wi-Fi/Internet Access
    *   Administrative PCs (for port documentation, payroll, reporting)
    *   Email Systems
    *   Onboard servers for general administration
*   **Characteristics:** Prioritizes **Confidentiality** and **Integrity** of data. Systems are often updated and replaced regularly.

#### **B. Operational Technology (OT) Networks**
These are the systems that control the physical processes of the ship. An attack here can have catastrophic physical consequences.

*   **Purpose:** Vessel operation and control.
*   **Systems Include:**
    *   **Navigation Systems:** ECDIS (Electronic Chart Display and Information System), GPS/GNSS, AIS (Automatic Identification System), RADAR.
    *   **Propulsion & Machinery Management:** Engine control systems, power management systems (PMS), ballast water systems.
    *   **Safety & Security Systems:** Fire detection, CCTV, vessel access control.
    *   **Cargo Management Systems:** Monitoring and control of liquid cargo, refrigerated containers, etc.
    *   **Bridge Systems:** Integrated Bridge Systems (IBS), Voyage Data Recorder (VDR).
*   **Characteristics:** Prioritizes **Availability** and **Safety**. Systems must run 24/7 without interruption. They often have very long lifecycles (15-25 years) and may run on legacy or proprietary operating systems that are difficult or impossible to patch.

---

### **2. Common Cyber Threats and Attack Vectors Onboard**

Attackers can compromise a vessel's network in numerous ways:

*   **Malware via Removable Media:** The most common vector. An infected USB stick brought onboard by a crew member or a third-party technician is plugged into a bridge or engine control room PC.
*   **Phishing & Social Engineering:** Crew members receive a malicious email and click a link or open an attachment, compromising the IT network. If the networks are not properly segmented, the infection can spread to OT systems.
*   **Lack of Network Segmentation:** A "flat" network where IT and OT systems can communicate freely. This allows a minor infection on a crew laptop to potentially reach and disable the ship's engine controls.
*   **Insecure Remote Access:** Satellite communications (VSAT, FleetBroadband) are a direct link to the outside world. If remote access for maintenance by shoreside vendors is not properly secured (e.g., using default passwords, no VPN), it provides a direct backdoor to critical systems.
*   **GPS/GNSS Spoofing and Jamming:** An external attack that feeds false location data to the ship's navigation systems, causing the vessel to deviate from its intended course without the crew realizing it.
*   **Unpatched Systems:** OT systems, in particular, often go unpatched due to concerns about operational stability. This leaves them vulnerable to known exploits that have long been fixed in the IT world.
*   **Supply Chain Vulnerabilities:** Malware can be embedded in new equipment or software before it is even installed on the vessel.

---

### **3. Consequences of a Cyber Attack on a Vessel**

The impact of a successful attack can range from inconvenient to catastrophic:

| Consequence Type | Example |
| :--- | :--- |
| **Safety** | Manipulation of navigation data (GPS spoofing) leading to collision or grounding. Disabling of steering or propulsion systems, leaving the vessel adrift. |
| **Operational** | Ransomware locking up the ECDIS or cargo planning computer, causing significant delays and inability to load/discharge cargo. |
| **Financial** | Ransom payments, vessel downtime, emergency repair costs, increased insurance premiums, regulatory fines. |
| **Environmental** | Manipulation of the Ballast Water Treatment System or oil discharge monitoring equipment, leading to illegal and harmful discharges. |
| **Commercial** | Theft of sensitive data, such as cargo manifests, route plans, or charter party agreements. |
| **Reputation** | Loss of trust from charterers, partners, and customers. A company known for cyber incidents may lose business. |

---

### **4. Best Practices for Securing Onboard Networks (The "People, Process, Technology" Framework)**

A robust cybersecurity posture requires a multi-layered approach.

#### **A. People: The Human Firewall**

The crew is the first and last line of defense.
*   **Training & Awareness:** Regular, role-specific training on recognizing phishing, proper use of USBs, and basic cyber hygiene.
*   **Access Control:** Enforce the principle of "least privilege." A deck officer does not need access to the engine control system.
*   **Clear Roles & Responsibilities:** Designate a cyber security officer on board and clearly define who is responsible for what during an incident.

#### **B. Process: Policies and Procedures**

*   **Cyber Risk Management:** Integrate cyber risk into the ship's existing Safety Management System (SMS), as required by the **IMO Resolution MSC.428(98) (IMO 2021)**.
*   **Incident Response Plan:** A clear, practiced plan for what to do when an attack happens. Who do you call? Which systems do you disconnect first? How do you operate manually?
*   **Network Management Policy:** Strict rules for network configuration, remote access, and patching.
*   **Vendor Management:** Vet the security practices of third-party vendors who connect to your systems.

#### **C. Technology: The Technical Controls**

*   **1. Network Segmentation (Crucial):** This is the most effective technical control. Isolate critical OT networks from the less-secure IT and crew networks using firewalls and Virtual LANs (VLANs). An infection on the crew Wi-Fi should *never* be able to reach the propulsion system.
*   **2. Firewalls & Intrusion Detection Systems (IDS):** Install and properly configure firewalls between network segments. Use an IDS to monitor for suspicious traffic.
*   **3. Endpoint Protection:** Install and maintain up-to-date antivirus/antimalware software on all PCs and servers (both IT and OT where possible).
*   **4. Patch Management:** Implement a process for testing and deploying security patches, especially for critical OT systems, in a controlled manner (e.g., during dry-dock).
*   **5. Secure Remote Access:** All remote access must be done over a secure, encrypted Virtual Private Network (VPN) with multi-factor authentication.
*   **6. Physical Security:** Lock server rooms and control physical access to USB ports on critical systems.

---

### **The Regulatory Landscape**

*   **IMO 2021 (MSC.428(98)):** Since January 1, 2021, ship owners and managers are required to assess cyber risk and implement relevant measures within their Safety Management System. Compliance is verified by Flag State administrations during annual ISM Code audits.
*   **Classification Societies (DNV, ABS, Lloyd's Register, etc.):** These organizations now offer specific "Cyber Secure" class notations and provide guidelines and services to help ship owners meet regulatory requirements.
*   **BIMCO & Industry Guidelines:** Organizations like BIMCO provide detailed, practical guidelines on how to implement cybersecurity measures onboard.

In conclusion, securing onboard networks is a complex but manageable challenge. It requires a holistic view that treats cyber security as a core element of maritime safety and operational resilience, combining well-trained people, robust processes, and properly configured technology.