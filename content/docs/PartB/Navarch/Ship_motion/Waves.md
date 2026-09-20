---
title: "Ship Waves and Wave Theory"
type: docs
math: true
---

## Relative Motion and Period of Encounter

**Vectors:**
- Ship's speed vector: \(\vec{V}_s\)
- Wave speed vector (phase velocity/Celerity): \(\vec{V}_w\)
- Angle between them: \(\mu\)

**Key Concepts:**
- **Absolute period** of waves: \(T_w\) (true wave period)
- **Period of encounter**: \(T_e\) (apparent period relative to ship)
- \(T_e\) is the resultant of \(T_w\) and the ship's speed through waves

**Direction Convention:**
- Head seas (meeting waves): \(\mu = 180^\circ\)
- Following seas: \(\mu = 0^\circ\)

**Relationships:**
\[T_e \propto V_s \quad \text{(ship speed)}\]
\[T_e \propto \mu \quad \text{(encounter angle)}\]

**Wave Group Velocity:**
\[V_{group} = \frac{1}{2}V_w \quad \text{(waves travel at half phase speed)}\]
*Note: A group of waves travels at \(V_w/2\), while individual wave crests travel at \(V_w\)*

**Energy Distribution:**
Exactly half the energy of a wave is kinetic and half is potential.

**Maximum Wave Height:**
\[H_{w\text{-max}} \approx 1.6 \times \text{SWH} \quad \text{(over 10 minutes)}\]
*(Note: The document also mentions \(H_{w\text{-max}} = 2 \times \text{SWH}\)  in another section—verify which coefficient your course uses)*

---

## Sinusoidal and Trochoidal Wave Theory

### Water Depth Classification
- **Shallow water:** \(d < \frac{\lambda}{2}\)
- **Deep water:** \(d > \frac{\lambda}{2}\) (presume this if depth not given)

### Wave Relationships

**Deep Water Formulas:**
\[V_w = \sqrt{\frac{g\lambda}{2\pi}}\]
\[T_w = \sqrt{\frac{2\pi\lambda}{g}}\]
\[\lambda = \frac{2\pi V_w^2}{g}\]

**General Relationship:**
\[\lambda = \frac{gT_w^2}{2\pi} \quad \text{(standard deep water dispersion)}\]

**Empirical Relation:**
\[T_w = 0.285 \times V_{wind} \quad \text{(where wind speed is in knots)}\]

**Very Shallow Water:**
\[V_w = \sqrt{g \times h_w}\]

---

## Trochoidal Wave Theory

### Historical Background
- **1905:** Froude theorized that irregular wave systems are composites of many regular wave systems
- **1952:** Researchers such as Trucker applied Fourier analysis to regular wave theory based on trochoidal waveforms
- The Trochoidal wave theory is not a perfect replica of observed sea states but comes closest compared to other theories

### Definition
> **A Trochoid** is a curve traced by a fixed point inside a circle as the circle rolls along and under a straight line.

### Geometric Properties
\[\lambda = L_w = 2\pi R \quad \text{(where \(R\) = radius of rolling circle)})\]
\[h_w = 2r \quad \text{(wave height, where \(r\) = radius of small circle)} \]

### Physical Characteristics
- Waveform has **sharper crests than troughs**
- Theory assumes water has **zero viscosity** and is **frictionless**
- Only the waveform (phase) moves, not the water mass
- Water particles move in **closed circular orbits** (one revolution per wave period)
- At depths greater than \(\frac{\lambda}{2}\), there is no water particle movement (wave base)

**Amplitude Decay with Depth:**
\[r = r_0 \cdot e^{-\left(\frac{2\pi z}{\lambda}\right)}\]
*(where \(z\) = depth below surface)*

---

## Assumptions for Simple Wave Theory

1. Crests are straight, parallel, and equally spaced
2. Wave heights remain constant
3. Wave form advances perpendicular to crest lines with uniform velocity \(V_w\)
4. \(V_w\) is "Celerity" (phase velocity), not individual particle velocity
5. Water has zero compressibility and zero viscosity
6. Trochoidal waves occur in deep waters
7. Deep sea waves: half kinetic, half potential energy
8. Individual waves rise behind the "dead water zone," travel through the group at \(2 \times V_w\) (relative to group), then subside in the dead water zone ahead
9. Waves travel in groups

---

## Significant Wave Height (SWH)

**Definition:**
When wave heights \(h_w\) are arranged in descending order, the mean of the **highest one-third** of the waves is called **SWH**.

**Requirements:**
- At least 20 observations needed for reliable assessment
- Waves not fully developed are excluded

**Importance:**
- Vital for master's decisions in heavy weather (particularly quartering/following seas)
- MSC 1228 specifically mentions importance of SWH observation

---

## Summary of Key Formulas

| Parameter | Formula | Notes |
|-----------|---------|-------|
| **Deep water wave speed** | \(V_w = \sqrt{\frac{g\lambda}{2\pi}}\) | |
| **Wave period** | \(T_w = \sqrt{\frac{2\pi\lambda}{g}}\) | |
| **Wavelength** | \(\lambda = \frac{2\pi V_w^2}{g}\) | |
| **Group velocity** | \(V_{grp} = \frac{V_w}{2}\) | |
| **Shallow water speed** | \(V_w = \sqrt{gh}\) | \(h\) = water depth |
| **Wave height** | \(H_{max} \approx 1.6\text{-}2.0 \times \text{SWH}\) | See note above |
| **Particle decay** | \(r = r_0 e^{-2\pi z/\lambda}\) | |

---

