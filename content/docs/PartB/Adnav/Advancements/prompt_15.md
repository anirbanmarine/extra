---
title: Discuss the special navigation systems the basic principle and use of Dynamic
  Positioning Systems;
type: docs
sidebar:
  open: true
---

Of course. Let's break down the concepts of special navigation systems, with a detailed focus on the principles and uses of Dynamic Positioning (DP) Systems.

---

### Part 1: Special Navigation Systems - An Overview

Standard navigation systems, like the GPS in your car or a ship's standard chart plotter, are primarily concerned with getting a vessel from Point A to Point B. **Special navigation systems**, on the other hand, are designed for tasks that require extremely high precision, operation in unique environments (like underwater), or automated control where human operation is impractical or unsafe.

These systems often integrate multiple sensors and are used for specific, mission-critical operations rather than general transit. Examples include:

*   **Inertial Navigation Systems (INS):** These use accelerometers and gyroscopes to track position and orientation from a known starting point. They are crucial for submarines and subsea vehicles where GPS signals cannot penetrate.
*   **Acoustic Navigation Systems (USBL, LBL):** These use sound pulses to determine the position of underwater vehicles or equipment relative to a surface vessel.
*   **Terrain-Referenced Navigation (TRN):** Used by advanced aircraft and cruise missiles, this system matches a real-time terrain profile (from radar or sonar) against a stored digital map to determine its precise location.
*   **Dynamic Positioning (DP) Systems:** A sophisticated system to automatically maintain a vessel's position and heading, which we will now discuss in detail.

---

### Part 2: Dynamic Positioning (DP) Systems

A Dynamic Positioning (DP) system is a computer-controlled system that automatically maintains a vessel's position and heading by using its own thrusters and propellers. It is essentially a "robotic" system for station-keeping, eliminating the need for anchors, which are often impractical or impossible in deep water or near subsea infrastructure.

#### The Basic Principle: A Three-Part Control Loop

The core principle of a DP system can be understood as a continuous loop of three essential functions: **Measure, Calculate, and Act**. Think of it as the system constantly asking and answering three questions: "Where am I?", "Where should I be?", and "How do I correct the difference?"

Here’s a breakdown of the three core components:

**1. MEASURE: The "Senses" of the System (Position Reference Systems & Sensors)**

The DP system must first know its exact position, its heading, and the environmental forces acting upon it. It does this by taking data from a suite of sensors. **Redundancy is critical**; a DP system will always use multiple reference systems simultaneously to cross-check data and reject faulty readings.

*   **Position Reference Systems:**
    *   **Global Navigation Satellite System (GNSS):** This is more than standard GPS. DP systems use **Differential GPS (DGNSS)** or **Real-Time Kinematic (RTK) GPS**, which use a fixed ground station or satellite corrections to achieve sub-meter or even centimeter-level accuracy.
    *   **Acoustic Systems (USBL/LBL):** An acoustic transponder (a pinger) is placed on the seabed or on a subsea vehicle (like an ROV). The vessel has a transceiver that sends a sound pulse and measures the time and angle of the return signal to calculate its position relative to the transponder.
    *   **Laser-Based Systems:** A laser on the vessel targets a reflective prism installed on a nearby fixed structure (like an offshore platform or another vessel). It measures the range and bearing to the target with very high accuracy.
    *   **Mechanical Taut Wire:** A classic system where a wire is lowered to the seabed with a depressor weight. A sensor on the vessel measures the angle and length of the wire to determine the vessel's movement relative to the fixed point on the seabed.

*   **Environmental and Vessel Sensors:**
    *   **Gyrocompasses:** To measure the vessel's heading (the direction it is pointing).
    *   **Motion Reference Units (MRU) / Vertical Reference Sensors (VRS):** To measure the vessel's roll, pitch, and heave (its up-and-down motion). This data allows the system to distinguish between the vessel being pushed off station and it simply rocking in the waves.
    *   **Anemometers (Wind Sensors):** To measure wind speed and direction.

**2. CALCULATE: The "Brain" of the System (The DP Controller)**

This is the central computer that processes all the incoming data.

*   **Data Analysis:** It takes in all the data from the position reference systems and sensors, filters out noise, and calculates a single, reliable estimate of the vessel's current position and heading.
*   **Mathematical Model:** The controller uses a sophisticated mathematical model of the vessel. This model "knows" how the vessel will react to forces like wind, waves, and current, and how much thrust is produced by each thruster.
*   **Force Calculation:** It compares the vessel's actual position to its desired setpoint. It then calculates the environmental forces (wind, waves, current) pushing the vessel off station. Based on this, it determines the precise amount of counteracting force (in tonnes) and turning moment required to stay perfectly in place.
*   **Thrust Allocation Logic:** The controller then decides the most efficient way to generate the required forces using the available thrusters. It calculates the optimal direction and power level for each individual thruster.

**3. ACT: The "Muscles" of the System (Thrusters and Propulsion)**

The DP controller sends commands to the vessel's propulsion system, which provides the physical force to hold the position.

*   **Thrusters:** DP vessels are equipped with specialized thrusters that can provide force in any direction (360 degrees).
    *   **Azimuth Thrusters:** Propellers that can be rotated 360 degrees to direct thrust precisely where it's needed. These are the workhorses of most DP vessels.
    *   **Tunnel Thrusters:** Thrusters mounted in tunnels running through the bow and stern, used for side-to-side (athwartship) movement.
*   **Main Propellers and Rudders:** These can also be integrated into the DP system to provide forward and backward (surge) thrust.

This **Measure -> Calculate -> Act** loop runs continuously, often several times per second, making constant, minute adjustments to the thrusters to keep the vessel exactly on its target position and heading, typically within a circle of just a few meters, even in harsh weather.

#### Use and Applications of DP Systems

Dynamic Positioning is an enabling technology for a vast range of maritime operations where anchoring is not feasible.

*   **Offshore Oil & Gas:**
    *   **Drillships & Semi-submersibles:** For deep-water drilling where anchors cannot reach the seabed.
    *   **Floating Production, Storage, and Offloading (FPSO) Units:** Large vessels that process and store oil from subsea wells.
    *   **Platform Supply Vessels (PSV):** Delivering supplies, mud, and equipment to offshore platforms, holding a steady position alongside the rig.
*   **Offshore Renewables:**
    *   **Wind Turbine Installation Vessels:** Precisely positioning heavy components like towers and blades.
    *   **Cable-Laying Vessels:** Laying power cables from offshore wind farms to shore with extreme accuracy.
*   **Subsea Construction & Maintenance:**
    *   **ROV (Remotely Operated Vehicle) Support Vessels:** Acting as a stable platform for launching and controlling underwater robots for inspection and repair.
    *   **Diving Support Vessels (DSV):** Providing a safe, stationary base for commercial diving operations.
*   **Other Applications:**
    *   **Dredging Vessels:** Maintaining position while performing precision dredging operations.
    *   **Cruise Ships & Mega Yachts:** Holding position in environmentally sensitive areas where anchoring would damage coral reefs, or for smooth passenger embarkation.
    *   **Research Vessels:** Staying perfectly still over a specific point for scientific sampling or seabed mapping.
    *   **Shuttle Tankers:** Loading oil from FPSOs in open seas.

In summary, Dynamic Positioning is a highly advanced special navigation and control system that integrates sensors, computers, and propulsion to achieve a feat of precision station-keeping that is fundamental to the modern offshore industry.