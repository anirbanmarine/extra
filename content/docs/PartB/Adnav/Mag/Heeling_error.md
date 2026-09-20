---
title: "Heeling Error"
type: docs
---

**Heeling Error (H/E)** is a deviation that occurs when a vessel rolls, heels, or lists. When the ship is upright, its vertical magnetic forces act perpendicularly to the compass card and exert no horizontal turning force on the compass needle. However, when the ship heels, these vertical magnetic fields tilt relative to the compass plane, developing a horizontal component that deflects the compass card.

Heeling error is caused by a combination of:
1. **Permanent vertical magnetism** (Force \(R\)).
2. **Induced vertical magnetism** in various soft iron structures.

---

### 1. Induced Magnetic Rods Involved in Heeling Error

The induced components of heeling error arise from four primary soft iron representations:

#### **A. \(k\)-rod (Vertical Soft Iron Directly Below the Compass)**
* **Nature & Location:** Represents vertical soft iron located below the compass position, such as deck pillars, bulkheads, and stanchions.
* **Induction:** Induced by the Earth's vertical magnetic field (\(Z\)). In the Northern Hemisphere, \(Z\) induces a **Blue pole at the top** (near deck level) and a Red pole at the bottom.
* **Effect when Heeled:** When the ship heels, the top Blue pole shifts toward the **high side** of the ship (or low side in the Southern Hemisphere). This attracts the North (Red) end of the compass needle toward the high side.
* **Characteristics:** 
  * Varies directly with the angle of heel (\(i\)) and Earth's vertical field (\(Z\)).
  * Varies inversely with Earth's horizontal directive force (\(H\)).
  * Varies as \(\cos(\text{compass course})\) (maximum on North/South, nil on East/West).
  * Can be expressed as varying directly with \(\frac{Z}{H} = \tan(\text{dip})\).

#### **B. \(e\)-rod (Continuous Horizontal Athwartship Soft Iron)**
* **Nature & Location:** Represents continuous athwartship soft iron, such as deck beams and frames running side-to-side.
* **Induction:** When the vessel is **upright**, these beams lie horizontally and are induced solely by \(H\), producing Coefficient \(D\). When the vessel **heels**, the beams develop a vertical component that becomes induced by Earth's vertical field \(Z\).
* **Effect when Heeled:** In the Northern Hemisphere, induction by \(Z\) creates a Blue pole at the upper end of the tilted beam and a Red pole at the lower end. This causes an additional deviation toward the **high side** on both Port and Starboard heels.
* **Characteristics:**
  * Varies directly with angle of heel (\(i\)), vertical field (\(Z\)), and \(\cos(\text{compass course})\).
  * Acts in the exact same direction as the \(k\)-rod (toward the high side in the N. Hemisphere); therefore, \(k\)-rod and \(e\)-rod effects are combined together as **total induced H/E** in calculations.

#### **C. \(c\)-rod (Vertical Soft Iron Forward or Abaft the Compass)**
* **Nature & Location:** Represents vertical soft iron situated forward or abaft the compass line (e.g., funnel, mast).
* **Induction & Effect:** When upright, it is induced by \(Z\) causing \(iB\). When heeled, the vertical rod tilts, developing a horizontal component that becomes induced by \(H\) when heading East or West.
* **Characteristics:**
  * Produces maximum heeling error on **East and West headings** and **nil on North and South headings**.
  * Varies as \(\sin^2(\text{compass course})\) and angle of heel (\(i\)).
  * **Correction:** Automatically corrected when the **Flinders Bar** is placed to correct \(iB\), because as the ship heels, the Flinders Bar tilts and develops an opposing induced pole.

#### **D. \(g\)-rod (Fore-and-Aft Horizontal Soft Iron Terminating Below Compass)**
* **Nature & Location:** Represents fore-and-aft horizontal soft iron that terminates directly beneath the compass.
* **Induction & Effect:** Induced by \(H\) when heading North/South. When the ship heels, its effective pole shifts to the high or low side.
* **Characteristics:**
  * Varies as \(\cos^2(\text{compass course})\) and angle of heel (\(i\)), producing the same direction of deviation on both North and South headings.
  * Independent of magnetic latitude.
  * **Note:** On modern steel vessels, fore-and-aft girders run continuously rather than terminating beneath the compass, so \(g\)-rod heeling error is usually absent.

---

### 2. Correcting Heeling Error Using the Vertical Force Instrument (VFI)

Because physically heeling a ship at a quay or sea to adjust magnets is cumbersome and time-consuming, the **Vertical Force Instrument (VFI)** is used to eliminate the ship's vertical magnetic field while the ship remains **completely upright**.

#### **Description & Principle of the VFI**
* **Construction:** The VFI consists of a magnetic needle mounted on a horizontal knife-edge pivot slightly above its center of gravity. In the absence of a vertical magnetic field, the needle lies horizontal. In a vertical field (\(Z\)), the needle tilts (Red end dips down in the Northern Hemisphere).
* **Graduated Arm & Rider Weight:** A sliding aluminum rider weight (\(w\)) moves along a graduated scale (\(d\)) on the needle to balance the dipping magnetic moment.
* **Equilibrium Condition:**
  \[2 m \cdot l \cdot Z = w \cdot d \implies M \cdot Z = w \cdot d\]
  *(where \(M\) is the magnetic moment of the needle, \(Z\) is the vertical field, \(w\) is rider weight, and \(d\) is scale distance)*.
* Since \(M\) and \(w\) are constant for a given instrument:
  \[d \propto Z\]
  The scale reading \(d\) is directly proportional to the vertical magnetic field strength.

---

#### **Step-by-Step Procedure for H/E Correction using VFI**

1. **Shore Calibration (Measuring Earth's \(Z_{\text{ashore}}\)):**
   * Place the VFI ashore in a location free from local magnetic interference, elevated at least 1 meter above the ground, aligned in the magnetic meridian.
   * Slide the rider weight along the high end until the needle is perfectly horizontal. Note the reading **\(n\) divisions**.

2. **Calculating the Ship's Setting (\(n_1\)):**
   * When upright on board, the horizontal athwartship \(e\)-rod receives no induction from \(Z\). However, when the ship heels later at sea, \(e\)-rod induction will appear.
   * To allow for the \(e\)-rod contribution without heeling the ship, the shore reading \(n\) is multiplied by the **Ship's Multiplier (\(\lambda_2\))**:
     \[n_1 = n \times \lambda_2\]
   * Reset the VFI rider weight to **\(n_1\) divisions** on the scale.

3. **Pre-Conditions On Board:**
   * **Flinders Bar and Soft Iron Spheres MUST be in position first**. The Flinders Bar eliminates \(c\)-rod H/E, and the soft iron spheres partly oppose/compensate the \(k\)-rod and \(e\)-rod fields. Correcting H/E before placing spheres would result in over-compensation.

4. **Ship Positioning:**
   * Head the ship on an **East or West magnetic heading**. This places any \(g\)-rod in a neutral position relative to Earth's \(H\), ensuring it does not influence the VFI reading.

5. **Instrument Setup at Compass Position:**
   * Unship the compass bowl from the binnacle.
   * Place the VFI in the exact gimbal/card position normally occupied by the compass needle system, with its needle aligned in the magnetic meridian (Red end pointing North).
   * If any uncorrected vertical field from the ship (\(R + k\text{-rod}\)) is present, the VFI needle will tilt away from the horizontal.

6. **Adjustment:**
   * Insert vertical permanent magnets into the **Heeling Error Bucket** directly below the compass position inside the binnacle (or raise/lower the bucket).
   * Adjust until the VFI needle becomes **perfectly horizontal**.
   * When leveled, the ship's vertical magnetic field at the compass position has been completely nullified.

> **Note on Latitude Changes:** Because vertical permanent magnets correct both permanent (\(R\)) and induced (\(k, e\)) fields together, the correction holds strictly for the latitude in which it was made. As the vessel changes latitude, \(Z\) changes, causing induced heeling error to change while the permanent magnet field remains constant, requiring re-adjustment across major latitude changes.

---

🧭 Would you like to work through a numerical calculation for setting the VFI rider weight (\(n_1 = n \times \lambda_2\)) or solving a multi-latitude heeling error adjustment problem?