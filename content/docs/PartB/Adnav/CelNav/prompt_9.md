---
title: Discuss with respect to celestial navigation Rates of change of altitude of
  celestial bodies
type: docs
sidebar:
  open: true
---

Of course. Let's have a detailed discussion on the rates of change of altitude of celestial bodies, a crucial and practical concept in celestial navigation.

This discussion will cover:
1.  **What it is:** The fundamental concept.
2.  **Why it's Important:** Its practical implications for the navigator.
3.  **The Governing Factors:** What makes the rate fast or slow.
4.  **Practical Scenarios & Applications:** How a navigator uses this knowledge.
5.  **The Effect of Observer's Motion:** An additional layer of complexity.

---

### 1. What is the "Rate of Change of Altitude"?

In celestial navigation, the **altitude (H)** of a celestial body is its angular height above the horizon, measured with a sextant. The **rate of change of altitude (dH/dt)** is simply how fast that angle is changing over time.

Imagine you are looking at the Sun through a sextant. In the morning, you see its lower limb climbing steadily away from the horizon. Around noon, it seems to "hang" in the sky, barely moving up or down. In the afternoon, it starts to descend, moving faster and faster towards the horizon. The speed of this apparent vertical movement is its rate of change of altitude.

This rate is primarily caused by the **rotation of the Earth**, which makes the celestial sphere appear to rotate around the observer at a rate of 15° per hour.

### 2. Why is this Important in Celestial Navigation?

Understanding the rate of change is not just academic; it is fundamental to the art and science of taking a good sight.

*   **Timing the Perfect Sight:** It tells you the best time to take a sight for a specific purpose (e.g., finding latitude vs. finding longitude).
*   **Assessing Sight Quality:** If you take a series of sights over a minute or two, the observed change in altitude should match the expected rate. If it doesn't, it could indicate an unsteady hand, a poorly defined horizon, or inconsistent sextant usage.
*   **Planning Sight Sessions:** A navigator can pre-calculate the best times to observe different bodies to get Lines of Position (LOPs) that cross at a good angle, leading to a more accurate fix.
*   **The "Noon Sight" (LAN):** The most famous application is finding latitude at Local Apparent Noon (LAN). At the exact moment the Sun reaches its highest point in the sky (its meridian passage), its altitude is momentarily stationary. The rate of change is zero. This gives the navigator a "window" to take a very careful and accurate measurement of the maximum altitude, which is then used to calculate latitude with high precision.

### 3. The Governing Factors

The rate of change of a body's altitude is not constant. It is governed by a precise mathematical relationship based on the geometry of the "Navigational Triangle" (the triangle formed by the Pole, the Zenith, and the celestial body).

The practical formula for a stationary observer is:

**`dH/dt = 15°/hr * cos(L) * sin(Zn)`**

Where:
*   **`dH/dt`** is the rate of change of altitude (in degrees per hour).
*   **`15°/hr`** is the base rate of Earth's rotation.
*   **`L`** is the observer's Latitude.
*   **`Zn`** is the body's Azimuth (its true bearing or direction from the observer).

Let's break down the influence of each factor:

#### a) Effect of Azimuth (Zn)

This is the most significant factor for a navigator at a given location.

*   **Fastest Rate:** The rate is at its **maximum** when the body is on the **Prime Vertical**, i.e., when it is due East (Azimuth = 90°) or due West (Azimuth = 270°). At these points, `sin(Zn)` is 1 or -1, and the body is "cutting" across the horizon at the steepest angle.
*   **Slowest Rate (Zero):** The rate is **zero** when the body is on the **observer's meridian**, i.e., when it is due North (Azimuth = 0°/360°) or due South (Azimuth = 180°). At this point, `sin(Zn)` is 0. This is the moment of maximum (or minimum) altitude, where the body appears to hang motionless in its vertical travel before reversing direction.

#### b) Effect of Latitude (L)

*   **Fastest at the Equator:** At the Equator (L = 0°), `cos(L)` is 1. All rates of change are at their maximum possible values for any given azimuth.
*   **Slowest at the Poles:** At the Poles (L = 90°), `cos(L)` is 0. The rate of change of altitude is always zero. This makes intuitive sense: at the poles, stars don't rise or set but travel in circles parallel to the horizon (circumpolar). Their altitude never changes.

### 4. Practical Scenarios & Applications

A good navigator uses this knowledge to their advantage.

#### Scenario 1: Sights for Longitude (Time Sights)

*   **Goal:** To get a Line of Position (LOP) that is as close to North-South as possible. This LOP is very sensitive to time but less sensitive to altitude errors, making it ideal for determining longitude.
*   **Method:** Take a sight of a body when its azimuth is close to **90° (East) or 270° (West)**.
*   **Consequence:** The rate of change will be at its **fastest**.
    *   **Pro:** An error in your sextant reading (altitude) will have a minimal effect on the longitude calculated from the sight. The resulting LOP will be very reliable.
    *   **Con:** Because the altitude is changing so rapidly, your timing must be perfect. An error of a few seconds can significantly change the altitude, so a chronometer with a known, small error is essential.

#### Scenario 2: Sights for Latitude (Meridian Passage)

*   **Goal:** To get an LOP that is perfectly East-West, providing a precise line of latitude.
*   **Method:** Take a sight of a body when it is on your meridian (Azimuth = **0° or 180°**). For the Sun, this is the classic "Noon Sight."
*   **Consequence:** The rate of change will be **zero**.
    *   **Pro:** The body "hangs" in the sky, allowing you to take multiple, careful readings to get the most accurate possible altitude without worrying about precise timing.
    *   **Con:** The resulting LOP is useless for determining longitude. An error in altitude translates directly to an error in latitude, but the position in the East-West direction is completely undefined from this single sight.

#### The Ideal Fix

The best fix is obtained from LOPs that cross at a large angle, ideally close to 90°. A navigator achieves this by:
*   Taking a sight of a body in the East (fast rate of change) to get a good N-S LOP.
*   Waiting an hour or two and taking a sight of another body in the South (slow rate of change) to get a good E-W LOP.
*   The intersection of these two LOPs gives a reliable position.

### 5. The Effect of Observer's Motion

The formula above assumes a stationary observer. If the vessel is moving, its own motion will also cause the body's altitude to change. This is critical for the concept of a **Running Fix**, where sights are taken at different times.

The change in altitude due to the observer's motion can be calculated as:

**`Change in H (nm) = Speed (kts) * Time (hrs) * cos(C - Zn)`**

Where:
*   **`Speed`** is the vessel's speed over ground.
*   **`Time`** is the interval between sights.
*   **`C`** is the vessel's course.
*   **`Zn`** is the body's azimuth.

**Interpretation:**
*   If you are moving directly **towards** the body's ground position (your course `C` is the same as the azimuth `Zn`), your motion causes the altitude to **increase**.
*   If you are moving directly **away** from the body's ground position (`C = Zn + 180°`), your motion causes the altitude to **decrease**.
*   If you are moving at a right angle to the azimuth, your motion has no effect on the altitude.

This effect is why we must "advance" or "retire" an earlier LOP to account for the vessel's travel between sights.

---

### Conclusion

The rate of change of altitude is far more than an abstract curiosity. It is a powerful, practical tool that lies at the heart of proficient celestial navigation. By understanding how and why the altitude of a celestial body changes, a navigator can plan their sights strategically, judge the quality of their observations, and ultimately produce the most accurate and reliable fix possible from the information the heavens provide.