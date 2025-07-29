---
title: Discuss with respect to celestial navigation Maximum and meridian altitudes
  of celestial bodies
type: docs
sidebar:
  open: true
---

Of course. This is a fantastic topic that gets to the heart of one of the most fundamental and reliable techniques in celestial navigation: finding latitude. Let's discuss Maximum and Meridian Altitudes in detail.

---

### Introduction: The Goal of the "Noon Sight"

In celestial navigation, the primary goal of observing a celestial body's altitude at or near its highest point in the sky is to determine the observer's **latitude**. This observation, traditionally done with the Sun at local noon, is famously called the "Noon Sight" or "Meridian Passage." The two concepts central to this process are **Meridian Altitude** and **Maximum Altitude**. While often used interchangeably in casual conversation, they are technically distinct.

### 1. Meridian Altitude

**Definition:**
Meridian Altitude is the altitude (the angle of a celestial body above the horizon) at the exact moment it crosses the observer's **celestial meridian**.

**Key Concepts:**
*   **Celestial Meridian:** This is an imaginary great circle on the celestial sphere that passes through the North and South celestial poles and the observer's zenith (the point directly overhead). Think of it as a projection of your line of longitude up into the sky.
*   **Time of Occurrence:** A body is at Meridian Altitude at the moment of **Local Apparent Noon (LAN)** for the Sun, or more generally, at the moment of **meridian passage** for any other body (Moon, planet, or star). At this instant, the body's bearing is exactly True North or True South.
*   **Significance:** This is the theoretical moment when the body is at its highest point in the sky *if the observer is stationary*. The geometry at this moment is the simplest possible for calculating latitude.

#### Calculating Latitude from Meridian Altitude

The beauty of the Meridian Altitude sight is its simple calculation. The relationship between your latitude (L), the body's declination (d), and its zenith distance (z) is direct.

1.  **Observe the Altitude:** Using a sextant, you measure the body's altitude as it crosses your meridian. This observed altitude (Hs) is corrected for various errors (index error, dip, refraction, etc.) to get the Corrected Altitude (Hc).
2.  **Calculate Zenith Distance (z):** The zenith is 90° directly overhead. Therefore, the angular distance from the zenith to the body is:
    $z = 90° - Hc$
3.  **Find Declination (d):** The declination of the body (its celestial latitude, or angular distance north or south of the celestial equator) is found in the Nautical Almanac for the date and time of the observation.
4.  **Determine Latitude (L):** The formula is a simple combination of declination and zenith distance.

The most reliable rule to apply is:
*   **Name the zenith distance (z):** Name it North if the body is bearing South at meridian passage; name it South if the body is bearing North.
*   **Combine:**
    *   If `L` and `d` have the same name (e.g., both North), **ADD** them: `Latitude = Declination + Zenith Distance`
    *   If `L` and `d` have different names (e.g., one North, one South), **SUBTRACT** the smaller from the larger: `Latitude = Larger - Smaller`. The resulting latitude takes the name of the larger value.

