---
title: Terrestrial and ship's magnetism :the rods a, b, c, d, e, f, g, h and k.
type: docs
sidebar:
  open: true
---

Excellent question. This gets to the very heart of how a magnetic compass is corrected on a steel ship.

You've listed the standard coefficients used in the mathematical analysis of compass deviation. It's a common point of confusion, so let's clarify: **the letters a, b, c, d, e, etc., are not names for physical rods themselves.**

Instead, they are **coefficients** in a mathematical equation that describes the different magnetic forces acting on the compass. The physical correctors—some of which are rods of soft iron or permanent magnets—are placed in the ship's binnacle to counteract the forces represented by these coefficients.

Let's break down each coefficient, the magnetic force it represents, and the physical corrector used to fix it.

---

### The Big Picture: The Deviation Equation

A ship's magnetic field causes the compass to deviate from Magnetic North. This deviation (`δ`) changes as the ship turns. The relationship is described by this approximate formula:

**Deviation (δ) ≈ A + B sin(ζ) + C cos(ζ) + D sin(2ζ) + E cos(2ζ)**

Where `ζ` (zeta) is the ship's magnetic heading. The letters A, B, C, D, and E are the coefficients you're asking about. The process of "swinging the ship" (turning it in a full circle and taking readings) is done to calculate the values of these coefficients.

---

### The Coefficients and Their Corresponding Correctors

Here is a detailed breakdown of each coefficient and the "rods" or other correctors associated with them.

#### Semicircular Deviation (Coefficients B, C, and k)
This deviation is caused by the ship's **permanent magnetism** and magnetism induced in **vertical soft iron**. It's called "semicircular" because it has one cycle over 360° of turning (i.e., it's positive on one semicircle of headings and negative on the other).

*   **Coefficient C**
    *   **Represents:** The force from permanent magnetism acting in the ship's **athwartships** (port-starboard) direction.
    *   **Correction:** **Fore-and-aft permanent magnets.** These are small, powerful bar magnets placed in the binnacle in a fore-and-aft orientation to create an equal and opposite field.

*   **Coefficient B**
    *   **Represents:** The force from permanent magnetism acting in the ship's **fore-and-aft** direction.
    *   **Correction:** **Athwartships permanent magnets.** These are bar magnets placed in the binnacle in an athwartships (port-starboard) orientation.

*   **Coefficient k (The Flinders Bar)**
    *   **This is the most famous "rod".** The coefficient `k` is a component of the semicircular deviation that is caused by magnetism **induced in vertical soft iron** (like masts, funnels, and the ship's bow and stern).
    *   **The Problem:** The strength of this induced magnetism changes with the Earth's magnetic dip, meaning it changes as the ship travels to different latitudes. The permanent magnets for `B` cannot account for this change.
    *   **Correction:** The **Flinders Bar**. This is a vertical rod of soft iron placed in the binnacle (usually in a canister on the forward or after side). Because it is also vertical soft iron, it gains and loses induced magnetism at the same rate as the ship's vertical iron, automatically correcting for this error in any latitude.

#### Quadrantal Deviation (Coefficients D and E)
This deviation is caused by magnetism **induced in the ship's horizontal soft iron** (like deck beams). It's called "quadrantal" because it has two cycles over 360° of turning, reaching maximums in the four intercardinal quadrants (NE, SE, SW, NW).

*   **Coefficient D**
    *   **Represents:** The force from magnetism induced in symmetrical horizontal soft iron.
    *   **Correction:** **Quadrantal Correctors.** These are two spheres of soft iron placed on brackets on the port and starboard sides of the binnacle. They are often called "Kelvin's balls." They correct the deviation by having magnetism induced in them that is equal and opposite to the effect of the ship's horizontal iron.

*   **Coefficient E**
    *   **Represents:** The force from magnetism induced in *asymmetrical* horizontal soft iron.
    *   **Correction:** This is usually very small and is corrected by slightly **skewing the quadrantal correctors** forward or aft. For most ships, this is ignored.

#### Constant and Higher-Order Deviation (A, f, g, h)

*   **Coefficient A**
    *   **Represents:** Constant deviation. This can be caused by a misalignment of the compass lubber line with the ship's centerline, or by an asymmetrical arrangement of the quadrantal correctors.
    *   **Correction:** If significant, the compass bowl is physically rotated slightly to remove the constant error.

*   **Coefficients f, g, h, j**
    *   **Represents:** Higher-order deviations (Sextantal, Octantal). They are caused by more complex interactions of induced and permanent magnetism.
    *   **Correction:** These are almost always negligible and are not corrected for in practice. They are simply part of the remaining "residual" deviation that is recorded on the deviation card.

---

### Summary Table

| Coefficient | Name of Deviation | Main Cause | Physical Corrector ("The Rods") |
| :--- | :--- | :--- | :--- |
| **A** | Constant | Misalignment of compass or correctors | Physically rotating the compass bowl |
| **B** | Semicircular | Permanent fore-and-aft magnetism | **Athwartships Magnets** |
| **C** | Semicircular | Permanent athwartships magnetism | **Fore-and-Aft Magnets** |
| **D** | Quadrantal | Symmetrical horizontal soft iron | **Quadrantal Correctors** (soft iron spheres) |
| **E** | Quadrantal | Asymmetrical horizontal soft iron | Skewing the Quadrantal Correctors |
| **k** | Semicircular (Heeling) | **Vertical soft iron** (masts, funnels) | **The Flinders Bar** (a vertical soft iron rod) |
| **f, g, h** | Higher Order | Complex magnetic interactions | None (usually ignored) |

So, when you hear about "the rods a, b, c...", what is really being discussed are the **coefficients** that quantify the magnetic problems, and the **physical correctors** (magnets, spheres, and the Flinders Bar) that are used to solve them. The most literal "rods" in this system are the **Flinders Bar (for coefficient k)** and the **permanent magnet bars (for coefficients B and C)**.