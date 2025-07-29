---
title: Discuss with respect to celestial navigation the formulation of Nories Nautical
  A-B-C tables
type: docs
sidebar:
  open: true
---

Excellent question. Discussing the formulation of Norie's A-B-C tables gets to the very heart of how navigators solved the celestial navigation problem before the advent of electronic calculators and voluminous sight reduction tables like HO 229.

Let's break down the discussion into several key parts:
1.  **The Fundamental Problem:** What celestial navigation problem do the tables solve?
2.  **The Mathematical Foundation:** The specific formulas used to create the tables.
3.  **The "Divide and Conquer" Formulation:** How the tables break the formula into manageable parts (A, B, and C).
4.  **The Role and Context:** Why they were so valuable and how they compare to other methods.

---

### 1. The Fundamental Problem: Solving the P-Z-X Triangle

At its core, celestial navigation is about resolving the "Navigational Triangle" (or P-Z-X triangle). This is a spherical triangle on the Earth's surface with vertices at:

*   **P:** The elevated celestial pole (North or South).
*   **Z:** The observer's Zenith (the point directly above the observer).
*   **X:** The geographic position of the celestial body (the point on Earth where the body is directly overhead).

The goal of "sight reduction" is to use known information to calculate two key values:
1.  **Calculated Altitude (Hc):** The altitude at which the celestial body *should* appear from our assumed position.
2.  **Azimuth (Zn):** The true bearing of the celestial body from our assumed position.

By comparing our Calculated Altitude (Hc) with our Sextant Altitude (Ho), we get an intercept (towards or away from the body's azimuth) which allows us to draw a Line of Position (LOP).

The known values we start with are:
*   **Latitude (L)** of the observer.
*   **Declination (d)** of the celestial body (from the Nautical Almanac).
*   **Local Hour Angle (LHA)** of the celestial body (calculated from GMT and longitude).

Norie's tables are a tool designed specifically to solve for Hc and Zn using these three inputs.

### 2. The Mathematical Foundation: The Haversine Formula

Directly solving the PZX triangle using spherical trigonometry is cumbersome. The key formula that Norie's tables are based on is the **Haversine Formula**, which is mathematically stable and well-suited for calculations involving logarithms and tables.

The formula to find the Zenith Distance (ZD), from which Hc is derived (Hc = 90° - ZD), is:

**`hav(ZD) = hav(L ~ d) + [ hav(LHA) * cos(L) * cos(d) ]`**

Where:
*   `hav(θ)` is the haversine of an angle θ, defined as `(1 - cos(θ)) / 2`.
*   **`L ~ d`** is the difference between Latitude and Declination if they are of the same name (both N or both S), or their sum if they are of contrary names (one N, one S).
*   **`LHA`** is the Local Hour Angle.
*   **`L`** is Latitude.
*   **`d`** is Declination.

Notice the formula has two main parts joined by addition. This is the key to the "divide and conquer" strategy.

### 3. The "Divide and Conquer" Formulation of the A-B-C Tables

Norie's genius was to pre-compute the difficult parts of this formula and present them in a way that reduces the entire process to simple addition and table lookups. The tables are formulated to solve the two parts of the Haversine formula separately.

#### **Solving for Calculated Altitude (Hc)**

The tables break the calculation into finding the value of the two terms in the Haversine formula.

**Term 1: `hav(LHA) * cos(L) * cos(d)`**

This term involves multiplication, which is difficult to do by hand. The historical solution for multiplication is **logarithms**, where `log(a * b) = log(a) + log(b)`. Norie's tables cleverly use this principle.

*   **Norie's Table A (Log Haversine):** This table is formulated as a lookup for the **logarithm of the haversine of the LHA**.
    *   **Input:** Local Hour Angle (LHA).
    *   **Output (Value A):** `log(hav(LHA))`
    *   *Formulation:* The table creator calculated `hav(t)` for every possible angle `t`, then took the logarithm of that value.

*   **Norie's Table B (Log Cosine):** This table is formulated to solve for the `cos(L) * cos(d)` part.
    *   **Input:** Latitude (L) and Declination (d).
    *   **Output (Value B):** `log(cos(L)) + log(cos(d))`
    *   *Formulation:* The table is a pre-computed addition of the log-cosines of the two input angles.

By finding A and B from the tables and adding them (`A + B`), the navigator is actually performing the calculation:
`log(hav(LHA)) + log(cos(L)) + log(cos(d))`, which equals `log [ hav(LHA) * cos(L) * cos(d) ]`.

The navigator then takes this sum and uses a "log-haversine to natural-haversine" conversion table (often part of Table C or a separate section) to find the anti-log, which is the natural number value of Term 1.

**Term 2: `hav(L ~ d)`**

This is a simple haversine lookup.

*   The navigator calculates `L ~ d`.
*   They then use a **Natural Haversine table** (usually included with the A-B-C tables) to look up `hav(L ~ d)`.

**Final Step for Hc:**
The navigator adds the two natural values they found:
`Natural Value of Term 1` + `Natural Value of Term 2` = `Natural hav(ZD)`

Finally, they re-enter the Natural Haversine table with this final value to find the angle ZD (Zenith Distance). The Calculated Altitude is then simply `Hc = 90° - ZD`.

#### **Solving for Azimuth (Zn)**

The Azimuth is calculated separately using a different set of A-B-C tables, often just called the "ABC Azimuth Tables." These are formulated from a different spherical trig identity:

**`tan(Azimuth) = sin(LHA) / [ cos(L) * tan(d) - sin(L) * cos(LHA) ]`**

This formula is messy. Norie's tables simplify it by breaking it into three parts, A, B, and C.

*   **A = `tan(L) / tan(LHA)`**
*   **B = `tan(d) / sin(LHA)`**
*   **C = `A ± B`** (The sign depends on the relationship between L and d).

The Azimuth is then found by: **`tan(Azimuth) = 1 / (C * cos(L))`**

*   **Formulation of the Azimuth Tables:** The tables are designed for the navigator to enter with LHA, L, and d to look up the values for A and B directly. The navigator then performs the simple addition or subtraction to find C, and a final lookup gives the Azimuth. The rules for naming the azimuth (e.g., N or S, E or W) are based on the observer's latitude and the body's LHA.

### 4. Role, Context, and Comparison

*   **Why were they created?** To provide a faster, more streamlined, and less error-prone method than performing a full calculation from scratch using a complete book of logarithms. They were a specialized tool for a specific job.

*   **Norie's vs. Sight Reduction Tables (HO 229):**
    *   **Norie's:** Requires more steps of calculation (addition, subtraction, interpolation). However, a single, compact volume covers all latitudes and all celestial bodies. This makes it highly portable and versatile.
    *   **HO 229:** A massive, multi-volume set where the entire problem is pre-computed. The navigator simply enters with L, d, and LHA and pulls out Hc and Zn directly with minimal interpolation. It's much faster and simpler to use but requires carrying a huge library of books to cover different latitude bands.

*   **Modern Relevance:** While obsolete for primary navigation due to GPS and electronic calculators, Norie's tables are still held in high regard. They are an essential backup on any ocean-going vessel, and learning to use them provides a deep understanding of the mathematics behind celestial navigation. They represent a brilliant bridge between raw theory and practical, at-sea application.

In summary, the **formulation of Norie's A-B-C tables is a masterclass in practical computation**. They deconstruct the complex Haversine and Azimuth formulas into small, additive steps, using pre-computed logarithms and haversines to eliminate the need for difficult multiplication and division, thereby allowing the navigator to solve the PZX triangle with only simple arithmetic and table lookups.