---
title: "errors of position line"
type: docs

---
In celestial navigation, position lines (PLs) derived from astronomical observations rely on precise measurements of altitude and time. Errors in reading the sextant (Index Error and Dip) or recording time (Chronometer Error) directly affect the **True Altitude (\(T_{\text{alt}}\))**, **True Zenith Distance (\(\text{TZD}\))**, or the **Geographical Position (\(\text{GP}\))** of the observed body, causing the calculated Position Line to shift.

---

### 1. Index Error (IE) — On the Arc vs. Off the Arc

Index Error occurs when the index mirror and horizon glass of a sextant are not parallel when the index arm is set exactly to \(0^\circ\). 

#### **On the Arc vs. Off the Arc**
* **On the Arc**: The sextant reads **above \(0^\circ\)** when zeroed. Because all altitude readings taken with this instrument will be **too high**, Index Error *on the arc* must be **subtracted** from the sextant altitude.
* **Off the Arc**: The sextant reads **below \(0^\circ\)** (on the arc of excess/micrometer drum) when zeroed. Because all altitude readings taken will be **too low**, Index Error *off the arc* must be **added** to the sextant altitude.

> **Mnemonic Rule:** *"If it's on the arc, it's off (subtract); if it's off the arc, it's on (add)."*

#### **Application in Numericals**
\[\text{Observed Altitude (Obs Alt)} = \text{Sextant Altitude }(S_A) \mp \text{IE}\]
* **Minus (\(-\))** for IE *on the arc*.
* **Plus (\(+\))** for IE *off the arc*.

#### **Effect of Misapplication / Omission on Position Lines**
* **Wrong Application (e.g., applying \(2'\) *on the arc* as \(2'\) *off the arc*)**:
  * Instead of subtracting \(2'\), you add \(2'\), causing the calculated True Altitude (\(T_{\text{alt}}\)) to be **too high by \(4'\)** (\(2 \times \text{IE}\)).
  * Since \(\text{TZD} = 90^\circ - T_{\text{alt}}\), the calculated True Zenith Distance becomes **too small by \(4'\)**.
  * Because TZD is the angular distance from the body's GP to the Position Line, a smaller TZD places the incorrect PL **too close (towards) to the GP** by \(4'\).
* **Rectification in Numericals**: To correct the position line, shift the PL **away from the GP** by \(2 \times \text{IE}\) (or subtract \(2 \times \text{IE}\) from a "towards" intercept).

---

### 2. Error of Chronometer (Time Error)

Chronometer error is the difference between the deck watch/chronometer time and Greenwich Mean Time (GMT/UTC). Since GHA increases as the Earth rotates, an error in GMT translates directly into a positional error in longitude.

#### **Rate of Rotation & Longitude Conversion**
The Earth rotates \(360^\circ\) in 24 hours (\(15^\circ\) per hour or \(15'\) of arc per minute of time):
\[\text{Arc Error} = \text{Time Error (in seconds)} \times \frac{15'}{60\text{s}} = \text{Time Error (in seconds)} \times 0.25' \text{ of long}\]
*(Note: For star observations, the rate of travel is approximately \(15.04'\) per minute of time).*

#### **Effect on Numericals**
* **Chronometer Fast**: Reading a fast chronometer means using a **later GMT**. The GHA extracted from the almanac will be **too large (shifted West)**, which shifts the calculated Position Line **Westwards**. To rectify, apply a \(\text{d'long}\) correction **Eastwards**.
* **Chronometer Slow**: Reading a slow chronometer means using an **earlier GMT**. The GHA extracted will be **too small (shifted East)**, shifting the calculated Position Line **Eastwards**. To rectify, apply a \(\text{d'long}\) correction **Westwards**.

#### **Relationship Between Longitude Error and Intercept Error**
The relationship between an error in longitude (\(\delta\,\text{d'long}\)) and the corresponding shift in intercept (\(\delta\,\text{Intercept}\)) is given by:
\[\delta\,\text{Intercept} = \delta\,\text{d'long} \times \sin(\text{Az}) \times \cos(\text{Lat})\]
\[\delta\,\text{d'long} = \frac{\delta\,\text{Intercept}}{\sin(\text{Az}) \cos(\text{Lat})}\]

---

### 3. Error of Dip (Height of Eye — HE)

Dip is the angular depression of the visible sea horizon below the true sensible horizon caused by the observer's height of eye above sea level.

#### **Finding Dip Given Height of Eye (HE)**
Dip is calculated using the standard formula:
\[\text{Dip (minutes of arc)} = 1.76 \sqrt{\text{HE in meters}} \quad \left(\text{or } \text{Dip}' = 0.97 \sqrt{\text{HE in feet}}\right)\]

#### **Application in Numericals**
Because elevating the eye depresses the visible horizon, sextant altitudes measured relative to the sea horizon are always **too large**. Therefore, Dip is **ALWAYS SUBTRACTED**:
\[\text{Apparent Altitude (App Alt)} = \text{Observed Altitude} - \text{Dip}\]

#### **Effect of Omitting Dip in Numericals**
* If Dip correction is **omitted**:
  * The True Altitude (\(T_{\text{alt}}\)) remains **too high** by the value of Dip.
  * The True Zenith Distance (\(\text{TZD}\)) becomes **too small** by the value of Dip.
  * The resulting Position Line is drawn **too close (towards) to the GP** by an amount equal to Dip.
* **Rectification in Numericals**: To rectify the omission of Dip, shift the Position Line **away from the GP** by the Dip value (or reduce a "towards" intercept by Dip).

---

Would you like to solve a numerical example combining Index Error, Chronometer Error, and Dip corrections to see their cumulative shift on a position line?
