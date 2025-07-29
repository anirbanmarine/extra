---
title: Maritime Cyber Security :removable media controls
type: docs
sidebar:
  open: true
---

Of course. Here is a comprehensive overview of Removable Media Controls within the context of Maritime Cyber Security.

---

### **Maritime Cyber Security: A Deep Dive into Removable Media Controls**

Removable media (USB drives, external hard drives, SD cards, CDs/DVDs) represent one of the most significant and persistent cyber threats to the maritime industry. While seemingly innocuous, these devices can bypass traditional network defenses and introduce malicious software directly into critical vessel systems.

Effective removable media controls are a cornerstone of any robust maritime cyber security plan, as mandated by IMO 2021 regulations.

---

### **1. Why is this a CRITICAL Issue for a Vessel?**

The maritime environment presents a unique set of challenges that amplify the risk from removable media:

*   **Convergence of IT and OT:** A ship's systems are a mix of Information Technology (IT) for administration and communication, and Operational Technology (OT) for navigation, propulsion, and safety (e.g., ECDIS, Engine Control, Ballast Water Management). A USB stick can act as a bridge, carrying malware from a crew member's infected personal laptop (IT) to the vessel's critical navigation system (OT).
*   **The "Air Gap" Fallacy:** Many critical OT systems are believed to be "air-gapped" or isolated from the internet. However, they require updates, patching, and data transfer (e.g., electronic chart updates, performance data extraction). This is almost always done via removable media, creating a physical bridge across the supposed air gap.
*   **Diverse and Transient Workforce:** A vessel interacts with numerous third parties:
    *   **Technicians & Surveyors:** Bring their own laptops and USB drives to service specific equipment.
    *   **Port Officials & Pilots:** May need to transfer data.
    *   **Crew:** Use personal USBs for movies, music, and personal files, often shared among themselves.
*   **Remote and Isolated Operations:** If a vessel is infected at sea, there is no on-site IT support team. The crew must handle the incident alone, potentially thousands of miles from shore, with limited connectivity for assistance.

---

### **2. The Risks: What Can Go Wrong?**

Uncontrolled use of removable media can lead to severe consequences:

| Risk                     | Description                                                                                                                                                             | Maritime Example                                                                                                                                                                                                                                        |
| ------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Malware Infection**    | The most common risk. Viruses, worms, trojans, and spyware can be unknowingly introduced.                                                                                 | A technician's infected USB drive introduces a virus to the ECDIS (Electronic Chart Display and Information System), causing it to crash or display incorrect information during critical navigation.                                                            |
| **Ransomware Attack**    | Malware that encrypts files on a system, making them inaccessible until a ransom is paid.                                                                                | A crew member's USB stick, carrying ransomware from a downloaded movie, infects the ship's cargo management system. The crew is locked out of ballast and stowage plans, delaying port operations and incurring massive financial penalties.                 |
| **Data Breach / Theft** | Unauthorized transfer of sensitive data off the vessel's systems.                                                                                                       | A disgruntled employee copies the entire voyage plan, cargo manifest (including high-value goods), and crew PII (Personally Identifiable Information) onto a personal USB drive and sells it to pirates or competitors.                                     |
| **System Disruption**    | Introducing unauthorized software or scripts that conflict with existing systems, causing them to become unstable or inoperable.                                         | A well-meaning engineer uses a USB with a "performance tuning" script downloaded from an online forum. The script is incompatible with the engine control software, causing the main engine to shut down unexpectedly at sea.                                  |
| **Bridging Networks**    | Transferring malware from a less secure network (e.g., Crew Wi-Fi) to a highly secure, critical network (e.g., the Bridge OT network).                                    | Malware is transferred from a personal laptop to a USB drive, which is then used on the ship's administrative PC. That same USB is later used to transfer a report to the Bridge, infecting the entire navigation network.                                |

---

### **3. Core Components of an Effective Removable Media Control Policy**

A multi-layered approach combining policy, technology, and people is essential.

#### **A. Policy and Governance (The Rules)**

1.  **Formal Written Policy:** Create a clear, simple, and strict policy on the use of all removable media. This policy should be part of the ship's Safety Management System (SMS).
2.  **Prohibit Personal Media:** Strictly forbid the use of personal USB drives or external hard drives on any ship's business (IT) or operational (OT) system.
3.  **Define Roles & Responsibilities:** Clearly state who is responsible for enforcing the policy (e.g., Captain, Chief Officer, ETO/IT Officer).
4.  **Vendor/Technician Management:** The policy must explicitly apply to all third parties. They must be informed of the procedure *before* boarding.

#### **B. Procedural and Physical Controls (The Process)**

1.  **Use Company-Issued Media:** Maintain a small inventory of company-controlled, encrypted, and regularly scanned USB drives. These are the *only* drives permitted for use.
2.  **Designated Scanning Station (The "Kiosk"):**
    *   Set up a standalone, hardened laptop or PC that is isolated from all critical networks.
    *   This PC should have up-to-date, powerful antivirus/anti-malware software.
    *   **The Procedure:** Any data from an external source (e.g., a technician's drive) *must* first be inserted into this scanning station. If clean, the data is then transferred to a company-issued USB drive for use on the target system.
3.  **Physical Port Blocking:** Use physical USB port locks (small plastic or metal devices) to block unused USB ports on critical equipment, especially on the bridge and in the Engine Control Room. This provides a visual and physical deterrent.
4.  **Secure Disposal:** Establish a procedure for securely destroying old or compromised USB drives (e.g., physical destruction).

#### **C. Technical Controls (The Technology)**

1.  **Endpoint Security:** Install and maintain up-to-date antivirus/anti-malware software on all computers where possible. Ensure auto-scan features for removable media are enabled.
2.  **Disable AutoRun/AutoPlay:** Use Group Policy (on Windows systems) to disable the AutoRun and AutoPlay features, which automatically execute files when a drive is inserted. This is a common infection method.
3.  **Device Whitelisting:** For high-security systems, configure the operating system to only accept specific, pre-approved USB devices (based on their serial numbers), blocking all others.

#### **D. The Human Element (The People)**

1.  **Training & Awareness:** This is the most critical layer. Conduct regular, role-specific training for all crew on the dangers of removable media. Use real-world examples.
2.  **Drills and Simulations:** Run periodic drills, such as leaving a "lost" USB drive in a common area to see if a crew member picks it up and plugs it into a system. Use this as a training opportunity.
3.  **Clear Communication:** Post reminders and posters near critical workstations (Bridge, ECR, Cargo Control Room) about the removable media policy.

---

### **4. Regulatory Context**

*   **IMO Resolution MSC.428(98):** Requires cyber risks to be appropriately addressed in Safety Management Systems (SMS) no later than the first annual verification of the company’s Document of Compliance after 1 January 2021.
*   **Industry Guidelines:** Bodies like **BIMCO**, **OCIMF (TMSA3)**, and **IACS** provide detailed guidelines on cyber security, all of which heavily emphasize the need for stringent removable media controls.

By implementing these controls, a shipping company can significantly reduce its cyber risk profile, protecting its assets, crew, and cargo from a simple but potentially devastating threat.