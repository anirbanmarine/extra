---
title: discuss with respect to positional errors in fixes Errors in fixes by vertical
  and horizontal sextant angles.
type: docs
sidebar:
  open: true
---

Excellent topic. A fix obtained by sextant angles is a classic and highly reliable method of coastal navigation. However, like any measurement technique, it is subject to errors that can affect the accuracy of the final position. Understanding these errors is crucial for a navigator to assess the quality of their fix.

Let's break down the discussion into the two types of angles and then discuss the combined effect on the fix.

---

### 1. Errors in a Fix by Vertical Sextant Angles (VSA)

A Vertical Sextant Angle (VSA) is used to determine the distance of a vessel from an object of known, charted height (e.g., a lighthouse, cliff, or tower).

#### **The Principle:**
The observer measures the angle between the top of the object and the sea-level horizon at its base. Using simple trigonometry, this angle, combined with the object's height, gives a distance. This distance produces a **Line of Position (LOP)** which is a **circle** with the object at its center and the calculated distance as its radius. A fix can be obtained from two or more such distance circles.

#### **Sources of Positional Error in VSA:**

**a) Instrumental Errors:**
These are errors inherent to the sextant itself.
*   **Index Error:** The most common error. If the sextant doesn't read 0° 0' when the mirrors are parallel, all readings will be offset. This should be checked and corrected for before every use.
*   **Other Errors:** Perpendicularity Error, Side Error, Collimation Error. These are less common if the sextant is well-maintained but can contribute to inaccuracies.

**b) Observational Errors:**
These are mistakes made by the person taking the sight.
*   **Incorrect Reading:** Simply misreading the vernier scale or micrometer.
*   **Not Holding the Sextant Vertically:** If the sextant is tilted, the measured angle will be a slant angle, which is larger than the true vertical angle. This will result in a **calculated distance that is shorter than the true distance**, placing your circular LOP too close to the object.
*   **Incorrect Identification of the Target:** Measuring to the light source of a lighthouse (the lantern) instead of the top of the structure as specified on the chart, or vice versa. This changes the "Height of Object" used in the calculation.

**c) Environmental & Data Errors (These are often the most significant):**
*   **Error in Charted Height:** The chart itself may have a small error in the listed height of the object. This is a systematic error that is difficult to detect.
*   **State of the Tide:** This is arguably the **most significant and frequently overlooked source of error in VSA**. The charted height of an object is almost always referenced to a specific vertical datum, typically **Mean High Water Springs (MHWS)**.
    *   If you take a sight at **low tide**, the sea level is lower, making the object's effective height *greater* than charted. Using the charted height in your calculation will result in a **calculated distance that is much longer than the true distance**.
    *   If you take a sight at a high tide that is higher than MHWS, the opposite occurs, and your calculated distance will be shorter.
    *   **Mitigation:** The height of the tide at the time of observation must be calculated and used to correct the charted height of the object before calculating the distance.
*   **Abnormal Refraction:** Standard tables for VSA calculations include a correction for average atmospheric refraction. However, in unusual conditions (e.g., a strong temperature inversion), light can bend more or less than standard, affecting the observed angle and thus the calculated distance.
*   **Height of Eye (Dip):** The observer's height of eye above the waterline must be known to correct for the "dip" of the horizon. An error in estimating the height of eye will lead to a small error in the final distance.

**Impact on the Fix:** An error in a VSA measurement shifts the entire circular LOP either inwards or outwards. If a fix is obtained from two VSAs on two different objects, an error in one will displace the intersection point of the two circles.

---

### 2. Errors in a Fix by Horizontal Sextant Angles (HSA)

A Horizontal Sextant Angle (HSA) measures the angle between two charted objects as seen from the vessel.

#### **The Principle:**
The locus of all points from which the angle between two fixed objects (A and B) is constant is a **circle of position** that passes through the observer and the two objects. A fix is typically obtained by observing two adjacent angles between three objects (e.g., angle A-B and angle B-C), creating two intersecting circles of position. This is the classic "three-point fix."

#### **Sources of Positional Error in HSA:**

**a) Instrumental and Observational Errors:**
These are similar to VSA:
*   Index Error must be applied.
*   The sextant must be held horizontally.
*   Misidentification of objects or misreading the scale will cause errors.
*   **Lack of Simultaneity:** If the vessel is moving, the angles A-B and B-C must be taken as close to simultaneously as possible. If there is a delay, the vessel will have moved between sights, distorting the geometry and creating a false fix.

**b) The Critical Role of Geometry ("Strength of Cut"):**
This is the most important concept for understanding HSA errors. The accuracy of the fix depends entirely on the angle at which the two circles of position intersect.

*   **Strong Fix:** The two circles of position intersect at a large angle (ideally close to 90°). In this case, a small error in one of the measured sextant angles will only cause a small displacement of the final fix.
    *   **Best Geometry:** Occurs when the middle object is closer to the vessel than the other two, or when the vessel is inside the triangle formed by the three objects.

*   **Weak Fix ("Revolver" or "Station Pointer" Error):** The two circles intersect at a very shallow, acute angle. Here, a tiny error in a measured sextant angle causes the corresponding circle to shift significantly, resulting in a **large error in the position along the common tangent of the two circles**. The resulting fix is unreliable.

*   **Indeterminate Fix (On the Danger Circle):** This is the worst-case scenario. If the observer and the three selected objects all lie on the circumference of the same circle, the two circles of position (from angle A-B and B-C) are actually the *same circle*. They are coincident, not intersecting. You cannot obtain a fix. This is known as being "on the circle."
    *   **How to Avoid:** Never choose three objects that appear to lie on the arc of a circle passing through your position. A simple check is that if the three objects are roughly in a straight line, the geometry is likely to be weak or indeterminate.

**Impact on the Fix:** The positional error is magnified by poor geometry. A navigator could take two perfect sextant readings but, due to a weak cut, end up with a very poor and unreliable fix.

---

### 3. The Combined Result: The "Cocked Hat"

When three or more LOPs are plotted (e.g., from two HSAs and one VSA, or three compass bearings), they will rarely intersect at a single point due to the combination of all the errors discussed above. Instead, they will form a small triangle (or polygon) called a **"cocked hat."**

*   **Size:** The size of the cocked hat is a direct indicator of the confidence in the fix. A small, tight cocked hat suggests small errors and a reliable position. A large cocked hat indicates a significant error in at least one of the observations or a very weak geometric cut.
*   **Interpretation:** The vessel's true position is assumed to be somewhere inside the cocked hat. For safety, a navigator will always assume the position within the cocked hat that is **closest to danger** (e.g., closest to a shoal, rocks, or the shore).
*   **Shape:** The shape can give clues. A long, thin cocked hat often points towards a weak cut from two of the LOPs.

### Summary and Conclusion

| Feature | Fix by Vertical Sextant Angle (VSA) | Fix by Horizontal Sextant Angle (HSA) |
| :--- | :--- | :--- |
| **LOP Type** | Circle of Distance around an object. | Circle of Position through two objects. |
| **Key Principle** | Distance from a known height. | Angle between two known positions. |
| **Most Critical Error** | **State of the Tide.** Failing to correct for it leads to large distance errors. | **Poor Geometry ("Strength of Cut").** Leads to magnification of small observational errors. |
| **Primary Mitigation** | Correct for height of tide. Hold sextant vertical. | Choose objects carefully for a strong cut. Avoid being "on the circle." |

In conclusion, while the sextant is a precision instrument, a reliable fix depends far more on the **navigator's understanding of the principles and potential errors.** For VSA, environmental corrections (especially tide) are paramount. For HSA, a diligent selection of objects to ensure strong geometric intersection is the key to accuracy. A good navigator will not only take the sights but will also critically assess the geometry and potential error sources to determine the confidence they can place in their final plotted position.