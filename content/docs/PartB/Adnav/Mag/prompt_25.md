---
title: Marine Magnetic Compass adjustment:sextantal and octantal deviations;
type: docs
sidebar:
  open: true
---

Excellent question. This dives into the more theoretical and nuanced aspects of magnetic compass adjustment. While most mariners focus on correcting Coefficients B, C, and D, understanding sextantal and octantal deviations provides a complete picture of the physics involved.

Let's break it down, starting with the familiar concepts and building up to the more complex ones.

### The Big Picture: Fourier Analysis of Deviation

When a ship is "swung" to determine its magnetic deviation, the deviation value changes as the ship's head changes. This curve of deviation versus ship's head is not random; it can be accurately described by a mathematical formula called a Fourier series.

The standard simplified formula for deviation ($\delta$) on a given compass course ($\zeta'$) is:

**$\delta = A + B \sin(\zeta') + C \cos(\zeta') + D \sin(2\zeta') + E \cos(2\zeta')$**

*   **A, B, C, D, E** are the **Coefficients of Deviation**.
*   **A, B, C** describe **Semicircular Deviation** (repeats every 360°).
*   **D, E** describe **Quadrantal Deviation** (repeats every 180°).

The goal of compass adjustment is to physically compensate for B, C, and D to make them as close to zero as possible. A and E are generally not corrected physically but are noted as residual deviations.

### Where Sextantal and Octantal Fit In

The formula above is a simplification. The full Fourier series has more terms:

**$\delta = A + (B\sin\zeta' + C\cos\zeta') + (D\sin2\zeta' + E\cos2\zeta') + (F\sin3\zeta' + G\cos3\zeta') + (H\sin4\zeta' + K\cos4\zeta') + ...$**

*   **The `3ζ'` terms (F and G)** describe **Sextantal Deviation**.
*   **The `4ζ'` terms (H and K)** describe **Octantal Deviation**.

---

### 1. Sextantal Deviation (Coefficient F & G)

This is the next level of complexity after quadrantal deviation.

*   **Period:** The `sin(3ζ')` term means the deviation pattern repeats every **120 degrees** (360° / 3).
*   **Appearance:** It has **six** points of maximum deviation (three positive and three negative) as the ship turns through 360°. This "six-pointed" nature is where the name "sextantal" comes from.

