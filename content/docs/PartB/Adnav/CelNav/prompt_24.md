---
title: discuss with respect to positional errors in fixes Errors in astronomical observations,
  position line and in fixes,
type: docs
sidebar:
  open: true
---

Of course. This is a fundamental topic in celestial navigation. Let's break down the sources and propagation of errors, from the initial observation to the final fix.

### Introduction: The Goal and the Reality

The goal of celestial navigation is to determine a ship's or aircraft's position on the Earth's surface. This is done by obtaining a **fix**, which is the intersection of two or more **Lines of Position (LOPs)**.

*   A **Line of Position (LOP)** is a line on which the observer is located. In celestial navigation, an LOP is derived from observing the altitude of a celestial body (Sun, Moon, planet, or star).
*   A **Fix** is the point where these LOPs intersect, theoretically representing the observer's exact position.

However, every step of this process is subject to error. Understanding these errors is as important as knowing the procedures themselves, as it allows the navigator to assess the quality and reliability of their calculated position.

The chain of error propagation is as follows:
**Errors in Observation → Errors in the Position Line → Errors in the Fix**

---

### 1. Errors in Astronomical Observations

This is the foundational source of all subsequent errors. An observation consists of measuring the **altitude (angle)** of a celestial body above the horizon at a precise **time**. Errors can be categorized as systematic or random.

#### A. Systematic Errors (Can be corrected for)

These are predictable errors that, if ignored, will consistently bias the result in one direction. Good practice and calculations can eliminate most of them.

1.  **Instrumental Error (Index Error):** No sextant is perfect. The index mirror and horizon mirror may not be perfectly parallel when the sextant is set to zero. This correctable error is called **Index Error** and must be measured and applied to every sight.
2.  **Chronometer Error:** The ship's chronometer (timepiece) may be running fast or slow. A timing error of just 4 seconds results in a 1' (one minute of arc) error in longitude. The daily rate of error of the chronometer must be known and applied to find the correct Greenwich Mean Time (GMT).
3.  **Refraction:** The Earth's atmosphere bends light from celestial bodies, making them appear higher than they actually are. This error is greatest at low altitudes and is corrected for using tables in the Nautical Almanac.
4.  **Dip (Height of Eye):** The observer's eye is above sea level, causing the visible horizon to be lower than the celestial horizon. This makes the observed altitude appear greater than it is. The correction for **Dip** depends on the observer's height of eye and is always subtracted.
5.  **Parallax:** For bodies within our solar system (Sun, Moon, planets), observations are made from the Earth's surface, not its center. Parallax correction adjusts the sight to a hypothetical observation from the center of the Earth. It's negligible for stars.
6.  **Semi-Diameter:** When observing the Sun or Moon, the navigator observes either the upper or lower edge (limb). The semi-diameter correction adjusts this reading to the center of the body.

#### B. Random Errors (Cannot be fully corrected for)

These are unpredictable and unavoidable errors that cause scatter in the data. The navigator's skill aims to minimize them.

1.  **Personal Error:** The observer's inability to perfectly align the celestial body with the horizon at the exact moment of observation. This can be due to reaction time, judging the "rocking" of the sextant, or a tendency to read the scale slightly high or low.
2.  **Atmospheric Conditions:** Haze, clouds, or abnormal atmospheric shimmer ("boiling" horizon) can make the horizon indistinct and the celestial body's image blurry, leading to inaccurate readings.
3.  **Vessel Motion:** The rolling and pitching of the vessel makes it extremely difficult to get a stable sight and read the sextant accurately.
4.  **Reading the Instrument:** Minor errors in reading the sextant's micrometer drum.

**Impact:** A cumulative error of **1 minute of arc (1')** in the final corrected altitude will result in a **1 nautical mile** error in the resulting Line of Position.

---

### 2. Errors in the Position Line (LOP)

An error in the observed altitude directly translates into an error in the LOP.

The process of plotting an LOP involves comparing the corrected **Observed Altitude (Ho)** with a **Computed Altitude (Hc)** for an Assumed Position (AP).

*   If Ho > Hc, the true position is on a line that is shifted *towards* the celestial body from the AP.
*   If Ho < Hc, the true position is on a line that is shifted *away* from the celestial body from the AP.

**The key takeaway is:**
**An error in the altitude (Ho) directly shifts the entire LOP along the azimuth (bearing) line to the celestial body.**

Because of the random errors mentioned above, a celestial LOP is not a perfect, infinitely thin line. It is more accurately described as a **"band of uncertainty."** The width of this band is determined by the likely magnitude of the random errors in the observation. A skilled navigator might trust their LOPs to within 0.5 NM, while a less experienced one in rough seas might have an uncertainty of 2 NM or more.

