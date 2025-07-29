---
title: Marine Magnetic Compass adjustment:types of transmitting magnetic compass bowls
  and repeaters.
type: docs
sidebar:
  open: true
---

Of course. This is an excellent topic that bridges traditional navigation with modern marine electronics. Here is a detailed breakdown of transmitting magnetic compass bowls and their associated repeaters, all within the context of marine magnetic compass adjustment.

---

### **Overview: The Role of the Transmitting Magnetic Compass (TMC)**

A standard magnetic compass is a standalone instrument. To know the heading, you must look directly at it. A **Transmitting Magnetic Compass (TMC)**, also known as a Transmitting Heading Device (THD), enhances this by converting the magnetic heading into an electronic signal.

This is crucial for several reasons:
*   **Reliability & Redundancy:** SOLAS (Safety of Life at Sea) regulations require a means to transmit the magnetic heading to the main steering position, emergency steering position, and other navigational equipment. The TMC serves as a vital, non-power-dependent (for the heading sensing part) backup to the gyrocompass.
*   **Integration:** The electronic signal (usually in NMEA 0183 or NMEA 2000 format) allows the magnetic heading to be displayed on repeaters around the vessel and used by other equipment like radar, ECDIS, and the autopilot.

**Crucial Point on Adjustment:** A TMC is, at its core, a magnetic compass. It is still subject to magnetic deviation caused by the ship's steel structure and electrical equipment. **Therefore, a TMC system must be physically adjusted (swung) just like a standard magnetic compass.** The sensors only transmit the heading that the compass card is showing; if that heading is wrong due to deviation, the transmitted heading will also be wrong.

---

### **Part 1: Types of Transmitting Magnetic Compass Bowls**

The "bowl" is the housing that contains the compass card, magnets, pivot, and liquid. The "transmitting" part is achieved by a sensor system that reads the orientation of the compass card without touching it. The primary difference between types of TMC bowls lies in the sensor technology used.

Here are the most common types:

#### 1. Fluxgate Sensor System (Most Common)

This is the industry standard for modern TMCs.

*   **Principle:** A fluxgate sensor is a highly sensitive magnetometer. In a TMC, a ring-shaped fluxgate sensor is mounted on top of or below the compass bowl, directly over the compass card's magnets.
    *   The sensor consists of two coils wrapped around a highly permeable magnetic core.
    *   An alternating current is passed through a primary "drive" coil, which drives the core into and out of magnetic saturation.
    *   When an external magnetic field (from the compass magnets) is present, it creates an asymmetry in the saturation of the core.
    *   This asymmetry induces a signal in the secondary "sense" coils at double the drive frequency. The strength and phase of this signal are directly proportional to the strength and direction of the magnetic field from the compass card.
*   **How it works:** The electronic processor measures the signal from the sense coils to precisely determine the orientation of the compass card's magnets and, therefore, the ship's magnetic heading.
*   **Advantages:**
    *   Very high accuracy and sensitivity.
    *   No moving parts in the sensor itself, leading to high reliability.
    *   Solid-state and robust.
*   **Examples:** Raytheon Anschütz Standard 22, Sperry Marine Jupiter, Yokogawa CMZ series.

