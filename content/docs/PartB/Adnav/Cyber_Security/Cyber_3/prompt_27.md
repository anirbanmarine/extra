---
title: Maritime Cyber Security :target systems
type: docs
sidebar:
  open: true
---

Of course. Maritime cyber security is a critical and complex field because it involves the intersection of Information Technology (IT), Operational Technology (OT), and a unique physical environment.

The target systems can be broadly categorized into three main domains: **Onboard Systems (on the vessel)**, **Shoreside Systems (at the port and corporate offices)**, and the **Communication Links** that connect them. An attack on any one of these can have cascading effects on the others.

Here is a detailed breakdown of the primary target systems in maritime cyber security.

---

### 1. Onboard Systems (Aboard the Vessel)

These are the systems physically located on the ship. They are often the most critical targets from a safety and operational perspective.

#### A. Navigation Systems
A compromise here directly threatens the safety of the vessel, crew, cargo, and the environment.
*   **ECDIS (Electronic Chart Display and Information System):** The digital navigation charts.
    *   **Impact:** Manipulating charts could lead to grounding, collision, or navigating into dangerous/prohibited waters. An attacker could delete charts, rendering the system useless.
*   **GPS / GNSS (Global Navigation Satellite System):** Provides the vessel's precise position, velocity, and time.
    *   **Impact:** **GPS Spoofing** (tricking the receiver into thinking it's somewhere else) or **Jamming** (blocking the signal) can cause the ship to go completely off course without the crew's knowledge.
*   **AIS (Automatic Identification System):** Transmits and receives vessel identification, position, course, and speed to other ships and shore stations.
    *   **Impact:** Attackers can spoof AIS data to create "ghost ships" to cause confusion, hide a vessel's true location, or make a legitimate vessel disappear from traffic monitoring systems, increasing collision risk.
*   **Radar / ARPA (Automatic Radar Plotting Aid):** Detects other vessels and obstacles.
    *   **Impact:** An attack could delete targets, create false targets, or alter tracking data, leading to a flawed understanding of the immediate surroundings.
*   **Gyrocompass / Autopilot:** Systems that maintain the ship's heading.
    *   **Impact:** A malicious actor could subtly or drastically alter the ship's course, potentially leading to a collision, grounding, or deviation into hostile territory.

#### B. Operational Technology (OT) / Industrial Control Systems (ICS)
These systems control the physical machinery of the vessel.
*   **Propulsion and Machinery Management Systems:** Controls the engine, power generation, and steering gear.
    *   **Impact:** An attacker could shut down the engine (leaving the ship adrift), cause it to over-speed (causing catastrophic damage), or disable steering, resulting in a complete loss of control.
*   **Cargo Management and Ballast Water Systems:** Controls the loading/unloading of cargo (especially in tankers and bulk carriers) and the ballast water used for stability.
    *   **Impact:** Manipulating these systems could destabilize the vessel, leading to capsizing. It could also be used to steal cargo (by falsifying sensor readings) or cause environmental damage through illegal ballast water discharge.
*   **Safety and Security Systems:** Fire detection, emergency shutdown systems, and vessel access control.
    *   **Impact:** Disabling these systems would leave the vessel and crew extremely vulnerable in a real emergency.

#### C. Information Technology (IT) Systems
These are the business and crew-related computer systems.
*   **Ship Administrative Network:** Used for port clearance documentation, crew and cargo manifests, and email.
    *   **Impact:** A primary target for **ransomware**, data theft (sensitive cargo details, crew PII), and phishing. It's often the initial entry point for an attack.
*   **Crew Welfare Systems:** The network providing internet and entertainment for the crew.
    *   **Impact:** Typically the least secure network on a ship. A compromised crew member's personal device (BYOD) can be used as a pivot point to attack more critical OT or administrative systems if network segmentation is poor.

---

### 2. Shoreside Systems (Port and Corporate)

These land-based systems are crucial for the logistics and business operations of the entire maritime supply chain.

*   **Terminal Operating System (TOS):** The "brain" of a container terminal. It manages all container movements, from crane operations to yard stacking and truck scheduling.
    *   **Impact:** A ransomware attack on a TOS can shut down an entire port, as seen in the NotPetya attack on Maersk. It can also be manipulated to facilitate cargo theft by directing a specific container to the wrong location.
*   **Port Community System (PCS):** A shared digital platform that allows stakeholders (port authorities, shipping lines, customs, freight forwarders) to exchange information.
    *   **Impact:** A breach could expose sensitive commercial data, disrupt customs clearance, and halt the flow of goods.
*   **Vessel Traffic Services (VTS):** The maritime equivalent of air traffic control, monitoring and managing ship movements in busy waterways.
    *   **Impact:** A compromise could lead to the transmission of false instructions to ships, causing chaos and a high risk of collision.
*   **Shipping Company Corporate Networks:** The central IT infrastructure of a shipping line, handling finance, booking, vessel scheduling, and human resources.
    *   **Impact:** Prime target for corporate espionage, large-scale ransomware, and financial fraud. Disruption here can paralyze the entire company's global operations.

---

### 3. Communication Systems (The Link)

These are the data links that connect the vessel to the shore and the outside world, making them a critical vector for attacks.

*   **Satellite Communications (SATCOM):** The primary channel for broadband data and voice for ships at sea (e.g., VSAT, Inmarsat).
    *   **Impact:** Vulnerable to eavesdropping, man-in-the-middle attacks, and denial-of-service. An attacker could intercept sensitive data or cut off the ship's connection to the outside world.
*   **VHF/HF Radio:** Used for voice communication, distress calls (GMDSS), and low-bandwidth data.
    *   **Impact:** Can be used to issue fake distress calls or transmit malicious instructions to a vessel's crew.
*   **Public Networks (Wi-Fi, 4G/5G):** When a vessel is in port or near the coast, it often connects to shore-based public or semi-public networks.
    *   **Impact:** These networks are often insecure and provide an easy entry point for malware to infect onboard systems if proper firewalls and security measures are not in place.

### Summary Table: Target Systems and Impact

| Category | Specific Target System | Potential Impact of Compromise |
| :--- | :--- | :--- |
| **Onboard Navigation** | ECDIS, GPS, AIS, Radar | Collision, Grounding, Vessel Tracking Failure, Navigating into Danger |
| **Onboard OT/ICS** | Engine, Cargo, Ballast Systems | Loss of Power/Control, Capsizing, Cargo Theft, Environmental Damage |
| **Onboard IT** | Admin & Crew Networks | Ransomware, Data Theft, Initial Entry Point for Deeper Attacks |
| **Shoreside Systems** | Terminal Operating System (TOS) | Port Shutdown, Supply Chain Paralysis, Systematic Cargo Theft |
| **Shoreside Systems** | Corporate & Port Networks | Financial Fraud, Corporate Espionage, Global Operations Disruption |
| **Communications**| SATCOM, VHF, Wi-Fi | Denial of Service, Eavesdropping, Man-in-the-Middle, Malware Vector |