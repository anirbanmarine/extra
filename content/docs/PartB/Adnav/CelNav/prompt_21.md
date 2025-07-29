---
title: Discuss with respect to positional errors in fixes errors in terrestrial observations,
type: docs
sidebar:
  open: true
---

Of course. This is a fundamental topic in navigation, surveying, and any field that relies on determining a position from physical measurements. Let's break down the relationship between errors in terrestrial observations and the resulting positional error in a fix.

### 1. The Core Principle: Error Propagation

The central concept is **error propagation**. A "fix" is a calculated position derived from one or more observations. Any error, no matter how small, in the initial observation does not simply disappear; it **propagates** through the geometric calculation and manifests as an error in the final position.

The goal of a good navigator or surveyor is not just to make accurate observations, but to understand how those errors will affect the final result and to choose an observation strategy that minimizes this propagation.

---

### 2. Types of Terrestrial Observations and Their Lines of Position (LOPs)

First, let's define the common types of terrestrial observations and the "Line of Position" (LOP) each one creates. An LOP is a line (or curve) on which the observer is known to be located.

| Observation Type | Instrument | Line of Position (LOP) |
| :--- | :--- | :--- |
| **Bearing** | Compass, Pelorus | A straight line extending from the observed object at the measured bearing. |
| **Distance (Range)** | Radar, Laser Rangefinder | A circle centered on the observed object with a radius equal to the measured distance. |
| **Horizontal Angle** | Sextant (used horizontally) | A circle that passes through the observer and the two observed objects. |

A fix is determined by the intersection of two or more LOPs. In a perfect world with no errors, two LOPs would intersect at a single point, and a third LOP would pass directly through that same point. In reality, this never happens.

---

### 3. Sources of Observational Error

The errors in the final fix originate from errors in these initial observations. These errors can be categorized as:

*   **Systematic Errors:** These are consistent, repeatable errors caused by instrument miscalibration or known environmental factors.
    *   **Examples:** Compass deviation (magnetic influence of the vessel/vehicle), index error on a sextant, a radar with a fixed range offset.
    *   **Impact:** They shift the entire LOP in a predictable direction. A constant 2° compass error will shift the entire bearing line by 2°. These can and **should be corrected for** before plotting. Uncorrected systematic errors lead to a fix that is biased, i.e., consistently wrong in a particular direction.

*   **Random Errors:** These are small, unpredictable fluctuations that remain after all systematic errors have been removed. They follow a statistical distribution (often a normal distribution or "bell curve").
    *   **Examples:** Difficulty in holding the instrument perfectly steady, slight misreading of a vernier scale or digital display, atmospheric shimmer affecting sightlines, limitations of human eyesight.
    *   **Impact:** Random errors are the primary reason LOPs don't meet at a perfect point. They create a **zone of uncertainty** around each LOP. An LOP is not an infinitely thin line, but rather a "fuzzy" band. The fix is not a point, but an **area of uncertainty**.

*   **Blunders (Gross Errors):** These are significant mistakes made by the observer.
    *   **Examples:** Misidentifying a landmark, transposing numbers when recording a bearing (e.g., writing 235° instead of 253°), reading the wrong scale on an instrument.
    *   **Impact:** A blunder will produce an LOP that is wildly inconsistent with others. This is a key reason for taking a third (or more) LOP—to act as a check. If two LOPs intersect in one place and a third is miles away, a blunder is the likely cause.

---

### 4. How Observational Errors Create Positional Error: The Geometry of the Fix

The way observational errors translate into positional error is critically dependent on the **geometry** of the fix—that is, the spatial relationship between the observer and the objects being observed.

#### The "Cocked Hat" and Area of Uncertainty

When three bearing LOPs are plotted, the random errors almost always cause them to form a small triangle, known as a **"cocked hat."** The observer's true position is assumed to be somewhere within this triangle.

*   **A small, well-formed (equilateral) cocked hat** indicates good observations with small random errors and strong geometry. This gives high confidence in the fix.
*   **A large cocked hat** indicates either a large random error in one or more of the observations or a potential uncorrected systematic error or blunder.
*   **A long, thin "sliver" of a cocked hat** is a classic sign of poor geometry, even if the observations themselves are accurate.

#### Key Geometric Factors Influencing Positional Error

**1. Angle of Cut (Angle of Intersection)**

This is the most critical geometric factor. It is the angle at which the LOPs intersect.

*   **Ideal Cut:** The ideal angle of cut is **90°**. At this angle, the error band around each LOP creates a small, roughly square-shaped area of uncertainty at the intersection. The error in the observation is propagated minimally into the final position.
*   **Poor Cut:** As the angle of cut becomes more acute (less than 30°) or obtuse (more than 150°), the area of uncertainty becomes a long, elongated parallelogram or ellipse. A small uncertainty in the bearing or range can now cause a very large uncertainty in the position along the axis of the ellipse. This is known as **geometric weakness**.

> **Example:** Imagine two bearing LOPs intersecting at 15°. A tiny wobble of 1° in either bearing will cause the intersection point to slide a long way along the LOPs. If they intersect at 90°, that same 1° wobble moves the intersection point by a much smaller amount.

**2. Distance to Observed Objects**

The effect of an angular error (like a bearing error) is magnified by distance. The linear, or cross-track, error of a bearing line is calculated as:

`Linear Error ≈ Distance × tan(Angular Error)`

*   **Impact:** A 1° error in a bearing to a landmark 1 nautical mile away creates a positional uncertainty of about 100 feet. That same 1° error for a landmark 10 nautical miles away creates an uncertainty of about 1000 feet.
*   **Best Practice:** Whenever possible, use closer objects for observations, as they are less sensitive to small angular errors.

**3. Number of Observations (Redundancy)**

Using more than the minimum number of LOPs (two) is highly beneficial.

*   **Error Detection:** As mentioned, a third LOP is a powerful tool for detecting blunders.
*   **Increased Confidence:** If three or more LOPs create a small, tight area of uncertainty, it increases the confidence in the fix.
*   **Statistical Improvement:** In advanced surveying, multiple redundant observations are used in a "least-squares adjustment." This statistical method finds the single most probable position that best fits all the observations simultaneously, providing a statistically rigorous estimate of the positional error (often represented as an **error ellipse**).

### Summary: Practical Implications

To minimize positional error in a fix derived from terrestrial observations, an observer must:

1.  **Minimize Observational Error:**
    *   Calibrate instruments to remove **systematic errors**.
    *   Use careful technique and take multiple readings to reduce **random errors**.
    *   Maintain situational awareness and cross-check work to avoid **blunders**.

2.  **Optimize Fix Geometry:**
    *   **Select objects that provide angles of cut as close to 90° as possible.** For three objects, the ideal is to have them separated by 120°. Avoid objects that are lined up or nearly lined up.
    *   **Prefer closer objects over distant ones**, especially for bearing observations.
    *   **Use a mix of LOP types if possible** (e.g., one range and one bearing), as their intersection (circle and line) often provides a strong 90° cut.
    *   **Always take at least three LOPs** to provide redundancy and a check on the quality of the fix.

In essence, a high-quality fix is the product of both **accurate observations** and **strong geometry**. Excellent observations with poor geometry can still result in a poor-quality fix with large positional uncertainty.