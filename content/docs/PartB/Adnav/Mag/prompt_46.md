---
title: variation, dip, total force, horizontal force, vertical force, local attraction;
  geographical variation and its effect on deviation; effects of permanent and induced
  magnetism; Components P, Q and R; the rods a, b, c, d, e, f, g, h and k. Sub-permanent
  magnetism and its effects at sea;
type: docs
sidebar:
  open: true
---

Of course. This is an excellent list of terms that form the foundation of marine compass theory. They explain why a ship's magnetic compass rarely points to True North and how navigators account for these errors.

Let's break down each concept in a logical order.

---

### **Part 1: The Earth's Magnetic Field**

This is the baseline. Before we can understand the errors, we must understand what the compass is trying to measure.

*   **Total Force:** The Earth's magnetic field is a vector, meaning it has both strength and direction. The **Total Force** is the full strength and direction of the magnetic field at any point on Earth.
*   **Horizontal Force (H):** This is the component of the Total Force that acts parallel to the Earth's surface. **This is the force that directs the magnetic compass needle.** The stronger the Horizontal Force, the more "directive force" the compass has. H is strongest near the magnetic equator and weakest near the magnetic poles.
*   **Vertical Force (Z):** This is the component of the Total Force that acts perpendicular to the Earth's surface, pointing down (in the Northern Hemisphere) or up (in the Southern Hemisphere). This force is responsible for **magnetic dip** and is a primary cause of **induced magnetism** in a ship's vertical steel.
*   **Dip (or Magnetic Inclination):** The angle between the Total Force and the Horizontal Force. It is the angle a freely suspended magnetic needle would make with the horizontal.
    *   At the magnetic equator, Dip is 0°.
    *   At the magnetic poles, Dip is 90°.
*   **Variation (or Magnetic Declination):** The horizontal angle between True North (the direction to the geographic North Pole) and Magnetic North (the direction indicated by the Horizontal Force of the Earth's magnetic field).
    *   Variation is a **geographical phenomenon**. It changes based on your location on Earth and also changes slowly over time.
    *   It is labeled as East or West. This value is found on nautical charts.
*   **Local Attraction (or Local Magnetic Anomaly):** A deviation from the Earth's normal magnetic field caused by large, localized magnetic influences *outside* the ship, such as underwater iron ore deposits, pipelines, bridges, or port structures. This is a rare, geographically-specific error.

---

### **Part 2: The Ship's Own Magnetism and its Errors**

A steel ship acts as a large, complex magnet that creates its own magnetic field, distorting the Earth's field at the compass position. This distortion is called **Deviation**.

*   **Geographical Variation and its Effect on Deviation:**
    *   **Variation** itself does *not* cause deviation. They are two separate errors. Variation is geographic; Deviation is ship-specific.
    *   However, the **geographical location** (latitude and longitude) dramatically affects the **magnitude of the deviation**. This is because the ship's induced magnetism (see below) is created by the Earth's field. As the ship travels to different latitudes, the Earth's H and Z forces change, which in turn changes the ship's induced magnetism and therefore its deviation.

#### **Types of Ship's Magnetism:**

1.  **Permanent Magnetism:**
    *   **Cause:** Acquired during the ship's construction. The hammering, riveting, and welding of steel plates in the Earth's magnetic field aligns the magnetic domains, turning the ship into a giant permanent magnet. Its magnetic signature is "hardened" into the hull.
    *   **Effect:** This magnetism is **fixed relative to the ship**. As the ship turns, these fixed magnetic fields are carried around with it, pushing and pulling the compass needle and causing **Semicircular Deviation** (an error that is maximum on two opposite headings, e.g., East and West).

2.  **Induced Magnetism:**
    *   **Cause:** Created in the ship's "soft iron" (steel that does not retain magnetism well) by the influence of the Earth's magnetic field. This magnetism is **temporary and changes depending on the ship's heading and location (latitude)**.
    *   **Effect:**
        *   **Vertical Soft Iron** (masts, funnels, bulkheads) becomes magnetized by the Earth's **Vertical Force (Z)**. This creates a force that acts like permanent magnetism and causes **Semicircular Deviation**.
        *   **Horizontal Soft Iron** (decks, beams) becomes magnetized by the Earth's **Horizontal Force (H)**. This causes **Quadrantal Deviation** (an error that is maximum on the four intercardinal headings: NE, SE, SW, NW).

3.  **Sub-permanent Magnetism:**
    *   **Description:** A "semi-permanent" form of magnetism that sits between permanent and induced. It's acquired after construction and can change over time.
    *   **Cause:** Long voyages on a single course, heavy pounding in rough seas, vibrations from the engine, major repairs, or loading/discharging magnetic cargoes (like iron ore). These events can slightly alter the ship's "permanent" magnetic signature.
    *   **Effects at Sea:** This is a major reason why a ship's deviation table is not permanently valid. After a long passage or a significant event, the sub-permanent magnetism may have changed, making the old deviation card inaccurate. This necessitates periodic checking of the compass error.

---

### **Part 3: Analyzing and Correcting Deviation**

To correct the compass, the complex magnetic forces of the ship are broken down into simpler components.

#### **Components P, Q, and R (Permanent Magnetism Forces)**

These are the three principal components of the ship's **permanent** magnetic force acting at the compass.

*   **Component P:** The force acting in the ship's **fore-and-aft** direction.
    *   `+P` is a force from a blue pole forward of the compass (or red pole aft).
    *   It causes semicircular deviation that is maximum on East and West headings.
*   **Component Q:** The force acting in the ship's **athwartships** (port-starboard) direction.
    *   `+Q` is a force from a blue pole on the starboard side of the compass (or red pole on the port side).
    *   It causes semicircular deviation that is maximum on North and South headings.
*   **Component R:** The force acting in the **vertical** direction at the compass. This force causes **Heeling Error** when the ship rolls, but has little effect when the ship is upright.

#### **The Rods a, b, c, d, e, f, g, h, and k (Induced Magnetism Model)**

This is a theoretical model developed by Archibald Smith to represent all the soft iron in the ship as nine notional rods. The interaction of these "rods" with the Earth's magnetic field (H and Z) explains all the induced magnetism effects.

*   **`a`, `b`, `c`:** Vertical rods (like masts, funnels). They are magnetized by the Earth's Vertical Force (Z) and cause **semicircular deviation**.
    *   `+c` is a vertical rod below the compass. Its effect is corrected by the **Flinders Bar**.
*   **`d`, `e`:** Horizontal rods. They are magnetized by the Earth's Horizontal Force (H) and cause **quadrantal deviation**.
    *   `+e` is a fore-and-aft rod. `+d` is an athwartships rod.
    *   Their combined effect is corrected by the **Quadrantal Correctors** (soft iron spheres).
*   **`f`, `g`, `h`, `k`:** Rods that are positioned diagonally, representing asymmetrical arrangements of iron. Their effects are generally smaller and contribute to heeling error.

---

### **Summary Table**

| Error Type | Caused By | Nature of Error | Corrected By |
| :--- | :--- | :--- | :--- |
| **Variation** | Earth's geography | Difference between True & Magnetic North | Applied from the nautical chart (calculation) |
| **Semicircular Deviation** | 1. Permanent Magnetism (P & Q) <br> 2. Induced Magnetism in Vertical Iron (rod `c`) | Maximum on two opposite headings | 1. Permanent Magnets (fore-and-aft and athwartships) <br> 2. Flinders Bar (vertical soft iron rod) |
| **Quadrantal Deviation**| Induced Magnetism in Horizontal Iron (rods `d` & `e`) | Maximum on intercardinal headings (NE, SE, SW, NW) | Quadrantal Correctors (soft iron spheres) |
| **Heeling Error** | Asymmetrical permanent (R) and induced (`g`, `k`) magnetism when ship rolls | Occurs only when the ship is heeled over | Heeling Magnet (vertical permanent magnet below the compass) |

This entire framework allows a compass adjuster to "swing the ship" (turn it through 360 degrees), measure the deviation on various headings, analyze the forces (P, Q, etc.) causing the error, and then place correctors (magnets, Flinders Bar, spheres) in the binnacle to counteract those forces, making the compass as reliable as possible.