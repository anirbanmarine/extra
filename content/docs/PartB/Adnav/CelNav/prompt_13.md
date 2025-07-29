---
title: Discuss with respect to celestial navigation the formulation of Nories Nautical
  Ex­ meridian tables
type: docs
sidebar:
  open: true
---

Excellent question. Discussing the formulation of Norie's Ex-Meridian tables takes us to the very heart of the practical genius behind celestial navigation. It's a classic example of how complex spherical trigonometry was simplified into a straightforward, tabular method for the working mariner.

Let's break down the discussion into several key parts:

1.  **The Navigational Problem:** What are Ex-Meridian Tables for?
2.  **The Theoretical Foundation:** The Spherical Trigonometry behind the sight.
3.  **The Simplification:** How the complex formula is made practical.
4.  **The Formulation of Norie's Tables:** How the tables are structured to solve the simplified formula.
5.  **The Second Correction:** An additional refinement for greater accuracy.

---

### 1. The Navigational Problem: The Need for Ex-Meridian Sights

The simplest and most reliable method for finding latitude at sea is the **Meridian Passage** or **"Noon Sight."** At the exact moment the sun (or any celestial body) crosses the observer's meridian, it reaches its maximum altitude. At this instant, the calculation for latitude is simple arithmetic:

**Latitude = Declination ± (90° - Maximum Altitude)**

The problem is that it's easy to miss the exact moment of meridian passage. Clouds might obscure the sun, the ship's motion could make a sextant reading impossible, or the navigator might be occupied with other duties.

An **Ex-Meridian** (or "near-meridian") observation is a sight taken a short time *before* or *after* meridian passage. The altitude observed will be slightly *less* than the maximum altitude at meridian passage. The purpose of Ex-Meridian tables is to calculate the small correction that must be **added** to this observed altitude to find what the altitude *would have been* at meridian passage.

### 2. The Theoretical Foundation: The PZX Triangle

All celestial navigation calculations are based on solving the PZX (Pole-Zenith-Celestial Body) spherical triangle.

*   **P:** The elevated celestial pole (North or South).
*   **Z:** The observer's zenith (the point directly overhead).
*   **X:** The position of the celestial body (e.g., the Sun).

The sides and angles of this triangle are:
*   **Side PZ:** Co-Latitude = 90° - Latitude
*   **Side PX:** Polar Distance = 90° ± Declination
*   **Side ZX:** Zenith Distance = 90° - Altitude
*   **Angle at P:** Hour Angle (`t` or LHA)

The relationship between these elements is given by the **Spherical Cosine Rule**:
`cos(ZX) = cos(PZ) * cos(PX) + sin(PZ) * sin(PX) * cos(t)`

Substituting the navigational terms:
`sin(Altitude) = sin(Latitude) * sin(Declination) + cos(Latitude) * cos(Declination) * cos(t)`

This is the fundamental formula.

### 3. The Simplification: From Cosine Rule to Practical Correction

Our goal is to find the difference between the observed altitude (`Alt_obs`) at a small hour angle `t`, and the meridian altitude (`Alt_m`) where `t = 0`.

Let the correction be `x`, such that `Alt_m = Alt_obs + x`.

From the cosine rule:
*   `sin(Alt_obs) = sin(Lat)sin(Dec) + cos(Lat)cos(Dec)cos(t)`
*   At meridian passage, `t=0` and `cos(t)=1`. Therefore:
    `sin(Alt_m) = sin(Lat)sin(Dec) + cos(Lat)cos(Dec)`

The difference is:
`sin(Alt_m) - sin(Alt_obs) = cos(Lat)cos(Dec) * (1 - cos(t))`

This is the key relationship. The correction we need is related to Latitude, Declination, and the Hour Angle (`t`). For the small angles involved in an ex-meridian sight, two mathematical approximations are crucial:

1.  **Small Angle Approximation for Sine:** For a small correction `x` (in radians), `sin(Alt_m) - sin(Alt_obs) ≈ x * cos(Alt_m)`.
2.  **Half-Angle Formula:** `(1 - cos(t)) = 2 * sin²(t/2)`. For a small angle `t` (in radians), this is approximately `t²/2`.

Combining these, we get:
`x * cos(Alt_m) ≈ cos(Lat)cos(Dec) * (t²/2)`

Solving for the correction `x`:
`x ≈ (t²/2) * [cos(Lat) * cos(Dec) / cos(Alt_m)]`

Since `Alt_m` is related to `Lat` and `Dec` (`Alt_m = 90 - (Lat ~ Dec)`), this can be rewritten as:
`x ≈ (t²/2) * [cos(Lat) * cos(Dec) / sin(Lat ~ Dec)]`
*(Note: `Lat ~ Dec` means `Lat - Dec` if they are the same name, and `Lat + Dec` if contrary name).*

This is the formula that Norie's tables are designed to solve. **The correction is proportional to the square of the time from meridian passage (`t²`)**.

### 4. The Formulation of Norie's Nautical Ex-Meridian Tables

Instead of forcing the mariner to calculate `t²` and `cos(Lat)`, `cos(Dec)`, etc., Norie's brilliance was to break the formula down into pre-computed parts. The tables are typically structured in two main parts.

**Let's rewrite the correction `x` in a form suitable for tables:**

`Correction (x) = [A] * [B]`

Where:
*   `[A]` is a factor depending only on the **Hour Angle (`t`)**.
*   `[B]` is a factor depending on the **Latitude and Declination**.

#### **Table I: The Time Factor (The "A" Value)**

*   **Argument (Input):** Hour Angle (`t`), expressed in minutes and seconds of time from meridian passage.
*   **Formulation:** This table calculates a value proportional to `t²`. The constant of proportionality is chosen to make the final units come out as minutes of arc (`'`) for the correction. The table essentially pre-computes `(t²/2)` scaled by a constant. Because the correction varies as the square of the time, doubling the time from noon quadruples the correction.

#### **Table II: The Latitude & Declination Factor (The "B" Value or Multiplier)**

*   **Arguments (Inputs):** Observer's DR Latitude and the Sun's Declination.
*   **Formulation:** This table pre-computes the term `cos(Lat) * cos(Dec) / sin(Lat ~ Dec)`. The user enters the table with their approximate latitude and the body's declination to find a single multiplier.

**The Practical Process:**
1.  Navigator determines the hour angle (`t`) in minutes of time from local noon.
2.  Enter **Table I** with `t` to find a value (let's call it the "At" factor).
3.  Enter **Table II** with DR Latitude and Declination to find a multiplier.
4.  **Correction = (Value from Table I) × (Multiplier from Table II)**.
5.  This correction is then **added** to the observed altitude (`Ho`) to get the computed Meridian Altitude.
6.  Latitude is then found using the standard Meridian Passage formula.

### 5. The Second Correction

The `t²` approximation works very well for hour angles up to about 15-20 minutes. For larger hour angles, or in high latitudes where the sun's altitude changes more slowly, the approximation begins to fail.

Norie's tables therefore include a **Second Correction**.

*   **Formulation:** This correction accounts for the next term in the Taylor series expansion of the cosine function. It is proportional to `t⁴` and also depends on the altitude itself. In practice, it's calculated using a simpler formulation: **Second Correction = C × (First Correction)²**, where `C` is a factor found in a small table, usually entered with the tangent of the meridian altitude.
*   **Application:** The second correction is almost always **subtracted** if the first correction is large. It is a small refinement to the much larger first correction.

### Summary of Formulation

In essence, the formulation of Norie's Ex-Meridian tables is a masterful piece of practical science. It:
1.  Starts with the exact **Spherical Cosine Rule**.
2.  Uses mathematical approximations (`t²`) valid for the specific conditions of a near-meridian sight.
3.  **Deconstructs the resulting formula** `x ≈ (t²/2) * [cos(Lat)cos(Dec) / sin(Lat~Dec)]` into two independent parts.
4.  **Tabulates these parts separately** (a time-dependent part and a latitude/declination-dependent part).
5.  Allows the navigator to solve a complex trigonometric problem by looking up two numbers in tables and performing a single multiplication, making the process fast, simple, and robust in a pre-electronic era.