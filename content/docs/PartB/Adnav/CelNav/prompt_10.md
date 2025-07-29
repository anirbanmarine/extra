---
title: Discuss with respect to celestial navigation Rates of change of hour angle
  of celestial bodies
type: docs
sidebar:
  open: true
---

Of course. This is an excellent and fundamental topic in celestial navigation. The rate of change of a celestial body's hour angle is the very foundation upon which we determine longitude at sea.

Let's break down the discussion into key parts:

1.  **Fundamental Concepts: GHA, LHA, and Time**
2.  **The Baseline Rate: Stars (Sidereal Rate)**
3.  **The Standard Rate: The Mean Sun (Solar Rate)**
4.  **The Variable Rate: The Apparent Sun**
5.  **The Slowest Rate: The Moon**
6.  **The "Almost-Star" Rate: The Planets**
7.  **Practical Implications for the Navigator**

---

### 1. Fundamental Concepts: GHA, LHA, and Time

*   **Greenwich Hour Angle (GHA):** The angular distance of a celestial body measured westward from the Greenwich Meridian (0° Longitude). It is a universal reference for the body's position relative to the Earth.
*   **Local Hour Angle (LHA):** The angular distance of a celestial body measured westward from the *observer's* own meridian.
*   **The Key Relationship:** The link between the two is your longitude.
    *   **LHA = GHA - Longitude** (if in West longitude)
    *   **LHA = GHA + Longitude** (if in East longitude)

In celestial navigation, we measure the altitude of a body to find our distance *from* its Geographic Position (GP). We use a chronometer (an accurate clock) to find the GHA at the exact moment of our sight. By calculating what the LHA *should* be for our assumed position, we can determine our line of position.

Therefore, the **rate at which GHA changes is directly proportional to the passage of time.** An error in time is an error in GHA, which translates directly into an error in our calculated longitude.

---

### 2. The Baseline Rate: Stars (Sidereal Rate)

The stars are so distant that their individual movements ("proper motion") are negligible for navigational purposes. They can be considered fixed points on the celestial sphere. Their apparent motion is caused purely by the Earth's rotation.

*   **The Reference:** The Earth completes one full 360° rotation relative to the stars in one **sidereal day**, which is approximately **23 hours, 56 minutes, and 4.09 seconds**.
*   **The Rate:** This gives a rate of change of GHA for any star (and the reference point, the First Point of Aries) of:
    *   360° / 23.934 hours ≈ **15.041° per hour**
    *   This is slightly faster than 15° per hour. It's why the stars rise about 4 minutes earlier each day.

In the Nautical Almanac, the GHA for stars is found by first looking up the GHA of the First Point of Aries (GHAγ) and then adding the star's Sidereal Hour Angle (SHA), which is a fixed value for a given epoch. The rate of change of GHA for a star is therefore the rate of change of GHAγ.

---

### 3. The Standard Rate: The Mean Sun

Our entire system of timekeeping (UTC, time zones) is based on the concept of a **Mean Sun**. This is a theoretical sun that moves along the celestial equator at a perfectly constant rate throughout the year.

*   **The Reference:** The Mean Sun completes its 360° circuit in exactly **24 hours**.
*   **The Rate:** This defines the standard rate we most often think of:
    *   360° / 24 hours = **15° per hour**
    *   15' (minutes of arc) per minute of time
    *   15" (seconds of arc) per second of time

This clean, constant rate is the bedrock of the "longitude by chronometer" method. **A time error of 1 minute results in a GHA error of 15 minutes of arc, which corresponds to a 15 nautical mile error in longitude at the equator.**

---

### 4. The Variable Rate: The Apparent Sun

The **Apparent Sun** (the real one we see and take sights of) does **not** move at a constant rate. Its rate of change of GHA varies slightly throughout the year.

*   **Reason 1 (Elliptical Orbit):** Due to Kepler's Second Law, the Earth moves faster in its orbit when it is closer to the Sun (perihelion, around January) and slower when it is farther away (aphelion, around July). This changes the Sun's apparent eastward motion against the background stars.
*   **Reason 2 (Axial Tilt):** The Sun's path (the ecliptic) is tilted 23.5° to the celestial equator. Even if the Sun moved at a constant speed along the ecliptic, its component of motion parallel to the celestial equator would be slower at the solstices and faster at the equinoxes.

*   **The Rate:** The Apparent Sun's GHA changes at a rate that is *on average* 15° per hour, but can be slightly more or less.
*   **The Correction:** The difference between the GHA of the Apparent Sun and the GHA of the Mean Sun is called the **Equation of Time (EoT)**. The Nautical Almanac tabulates the GHA of the Apparent Sun directly, so the navigator doesn't need to apply the EoT, but the underlying principle is why the GHA increments for the Sun are not perfectly uniform.

---

### 5. The Slowest Rate: The Moon

The Moon is the most challenging body because it has a very fast orbital motion of its own, in the same direction as the Earth's rotation (eastward).

*   **The Reference:** The Moon orbits the Earth in about 27.3 days. This means it moves eastward against the background stars by about 360°/27.3 ≈ 13.2° per day.
*   **The Effect:** This eastward motion "fights against" the westward apparent motion caused by Earth's rotation. Therefore, the Moon's GHA changes at a *slower* rate than any other body.
*   **The Rate:**
    *   It starts with the star rate (~15.04°/hr westward).
    *   It subtracts its own eastward motion (~0.55°/hr).
    *   The net rate of change of the Moon's GHA is approximately **14.5° per hour**.

This significant difference is why **the Nautical Almanac has a separate GHA increment table specifically for the Moon.** Using the table for the Sun or stars would introduce a large, immediate error.

---

### 6. The "Almost-Star" Rate: The Planets

Planets also have their own orbital motion. However, being much farther away than the Moon, their apparent daily motion against the background stars is much smaller.

*   **The Rate:** Their rate of change of GHA is very close to the sidereal rate of 15.04° per hour. The small difference is caused by their own orbital motion as seen from a moving Earth.
*   **The Correction:** For this reason, the Nautical Almanac groups the **Sun, Planets, and Aries** into the same GHA increment table. To account for the small deviation from the mean rate, a correction known as the **"v correction"** is applied.
    *   'v' is the hourly difference between the body's actual motion and the tabulated mean motion.
    *   You find the 'v' value at the bottom of the daily page for the planet and apply the corresponding correction from the increment tables. It is usually a small value (a few tenths of a minute of arc).

---

### 7. Practical Implications for the Navigator

*   **Time is Longitude:** The rate of change of GHA is the direct link between time and longitude. Accurate timekeeping is paramount.
*   **Use the Right Tools:** A navigator must understand these different rates to use the **Nautical Almanac** correctly. Using the wrong increment table (e.g., using the Sun/Planets table for a Moon sight) will result in a completely incorrect Line of Position (LOP).
*   **Criticality of Timing:** Because the GHA of every body changes at roughly 15' of arc per minute, a sight must be timed to the nearest second if possible. A 4-second time error is a 1' longitude error. For the faster-moving Moon, timing is even more critical.
*   **The "v" and "d" Corrections:** The 'v' correction (for GHA) and 'd' correction (for declination) exist precisely because the Sun, Moon, and Planets do not have constant rates of change relative to the celestial coordinate system. They are the fine-tuning that makes celestial navigation accurate.
*   **Running Fixes:** When advancing an LOP over time, the navigator must account for the body's movement. This means advancing the body's GHA by its rate of change for the time elapsed, in addition to accounting for the vessel's own movement.