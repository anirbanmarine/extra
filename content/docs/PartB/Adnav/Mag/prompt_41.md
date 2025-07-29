---
title: Marine Magnetic Compass adjustment:Effects of magnets on a compass needle under
  varying conditions;
type: docs
sidebar:
  open: true
---

Of course. This is a fundamental topic in marine navigation. Here is a detailed breakdown of how a ship's magnetism affects its compass and how adjustments are made under varying conditions.

---

### **The Fundamental Problem: The Ship is a Magnet**

A marine magnetic compass is a simple instrument: a magnetized needle that wants to align itself with the Earth's magnetic field, pointing to Magnetic North.

The problem is that a steel ship is, itself, a massive and complex magnet. This shipboard magnetism creates its own magnetic field that pulls the compass needle away from Magnetic North. The angular difference between where the compass *should* point (Magnetic North) and where it *actually* points is called **Deviation**.

The goal of compass adjustment is to counteract the ship's magnetic field using a combination of small magnets and soft iron correctors placed within the compass binnacle, creating a "magnetically clean" environment for the compass itself.

The ship's magnetism is broken down into two main categories:

1.  **Permanent Magnetism (Hard Iron)**
2.  **Induced Magnetism (Soft Iron)**

Let's examine the effects of each under varying conditions.

---

### **1. Permanent Magnetism (Hard Iron)**

This is magnetism that is "locked into" the ship's steel structure during its construction (e.g., from hammering, welding, and riveting in the Earth's magnetic field) or from major events like a lightning strike. It is a fixed magnetic field *relative to the ship*.

#### **Effect on the Compass Needle**

Imagine a permanent bar magnet is fixed to the ship's deck.
*   When the ship is pointing North, this magnet might pull the compass needle to the East.
*   When the ship turns and points South, that same magnet is now on the opposite side of the compass and will pull the needle to the West.

This type of error, which changes as the ship turns, is called **Semicircular Deviation** because it goes through a full cycle in 180 degrees of turning (and repeats in the next 180 degrees).

#### **Varying Conditions & The Correctors**

**Condition: Change in Ship's Heading**

Permanent magnetism is analyzed in three components (P, Q, and R), but for adjustment, we focus on the horizontal components that affect the flat compass card.

*   **Fore-and-Aft Component (Coefficient B):** Caused by permanent magnetism aligned with the ship's centerline. It causes maximum deviation on East and West headings.
    *   **Corrector:** Small, permanent **fore-and-aft magnets** placed in the binnacle. They are adjusted while the ship is on an East or West heading to create an equal and opposite field, canceling out the error.

*   **Athwartships Component (Coefficient C):** Caused by permanent magnetism acting across the ship (port-to-starboard). It causes maximum deviation on North and South headings.
    *   **Corrector:** Small, permanent **athwartships magnets** placed in the binnacle. They are adjusted while the ship is on a North or South heading.

**Condition: Change in Ship's Latitude**

The strength of the Earth's magnetic field has a vertical component that changes with latitude (mostly vertical at the poles, horizontal at the equator). This can change the ship's permanent magnetism over time, but the primary corrector for vertical permanent magnetism is the Heeling Magnet.

**Condition: Heeling (When the Ship Rolls or Lists)**

Permanent vertical magnetism (e.g., in the funnel or masts) has no effect when the ship is upright. However, when the ship heels over, this vertical field gains a horizontal component that can pull the compass needle.

*   **Corrector:** The **Heeling Magnet**. This is a vertical magnet placed in a central tube directly beneath the compass pivot. It is adjusted to counteract the ship's permanent vertical field, preventing errors when the ship rolls.

---

### **2. Induced Magnetism (Soft Iron)**

Soft iron is material (like the ship's deck plates) that becomes a temporary magnet when it is placed in a magnetic field (in this case, the Earth's field). Its magnetism is *induced*, and its strength and polarity depend entirely on its orientation within the Earth's field. **This means its effect on the compass changes with both the ship's heading and its geographic location (latitude).**

#### **Effect on the Compass Needle**

**A. Symmetrical Soft Iron (Quadrantal Deviation)**

Imagine horizontal soft iron beams running across the ship on the port and starboard sides of the compass.
*   When the ship is on a North/South heading, these beams are aligned East-West. The Earth's field induces magnetism in them that pulls equally on both sides of the needle, causing no deviation.
*   When the ship is on an East/West heading, the beams are aligned North-South. They become magnetized and shield or intensify the field, but again, the effect is symmetrical and causes no deviation.
*   When the ship is on an **intercardinal heading (NE, SE, SW, NW)**, the induction is asymmetrical and pulls the needle off its proper heading.

This error is called **Quadrantal Deviation** because it is maximum at the four intercardinal points and zero at the cardinal points (N, E, S, W). It is represented by **Coefficient D**.

*   **Corrector:** The two **Quadrantal Spheres** (soft iron spheres) mounted on the sides of the binnacle. When the ship is on an intercardinal heading (e.g., NE), the spheres have magnetism induced in them that is equal and opposite to the effect of the ship's horizontal soft iron, thus canceling the deviation. They are moved closer to or further from the compass to adjust the effect.

**B. Vertical Soft Iron (Variable with Latitude)**

This is one of the most complex effects. It is caused by magnetism induced in vertical soft iron structures (masts, funnels, bulkheads) by the vertical component of the Earth's magnetic field.

*   **At the Magnetic Equator:** The Earth's field is horizontal, so no magnetism is induced in vertical soft iron. This effect is zero.
*   **In the Northern Hemisphere:** The Earth's field dips downwards. This induces a North pole at the bottom of a vertical mast and a South pole at the top. The "South pole at the top" acts like the North-seeking end of a permanent magnet and affects the compass.
*   **In the Southern Hemisphere:** The field points upwards, reversing the polarity. The "North pole at the top" now affects the compass.

This induced field creates a semicircular deviation that is indistinguishable from the permanent **Coefficient B** (Fore-and-Aft) magnetism. The key difference is that its strength depends on latitude.

*   **Corrector:** The **Flinders Bar**. This is a vertical bar of soft iron placed in a case on the binnacle, usually on the forward or aft side.
    *   **How it works:** It counteracts the magnetism induced in the ship's *vertical* soft iron. Because the Flinders Bar is also vertical soft iron, the magnetism induced in it changes with latitude in the *exact same way* as the unwanted magnetism in the ship.
    *   Therefore, it provides automatic correction for this latitude-dependent error, whereas the permanent magnets for Coefficient B do not. The adjuster's job is to figure out how much of the "fore-and-aft" error is permanent (corrected by magnets) and how much is induced (corrected by the Flinders Bar).

### **Summary Table of Effects and Correctors**

| Type of Magnetism | Name of Deviation | Caused By (Example) | Max Deviation On Heading | Corrector |
| :--- | :--- | :--- | :--- | :--- |
| **Permanent (Hard Iron)** | Semicircular (Coeff. B) | Fore-and-aft permanent magnetism | East / West | Fore-and-Aft Magnets |
| **Permanent (Hard Iron)** | Semicircular (Coeff. C) | Athwartships permanent magnetism | North / South | Athwartships Magnets |
| **Permanent (Hard Iron)** | Heeling Error | Vertical permanent magnetism (when ship rolls) | Varies with roll | Heeling Magnet |
| **Induced (Soft Iron)** | Quadrantal (Coeff. D) | Symmetrical horizontal soft iron | NE, SE, SW, NW | Quadrantal Spheres |
| **Induced (Soft Iron)** | Semicircular (Part of B) | Vertical soft iron (changes with latitude) | East / West | Flinders Bar |

---

### **Conclusion: The Art of Adjustment**

The process of "swinging the ship" involves slowly turning the vessel in a full circle and recording the deviation on various headings. A skilled compass adjuster uses this data to calculate the coefficients (B, C, D, etc.) and then introduces the physical correctors—the magnets, spheres, and Flinders Bar—to counteract each effect.

The final result is a compass with the minimum possible deviation. Any small, remaining deviation is recorded on a **deviation card** that the navigator uses to make final corrections to their course. The process must be repeated periodically, especially after major structural work, carrying magnetic cargo (like iron ore), or after a long period on one heading.