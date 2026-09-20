---
title: Pole Star Tables
type: docs
---

### 1. \(PZX\) Spherical Triangle Setup

In the celestial sphere, consider the \(PZX\) triangle for Polaris:
* \(P\): Elevated Pole
* \(Z\): Observer's Zenith
* \(X\): Position of Polaris
* \(PZ = c = 90^\circ - L\) (co-latitude, where \(L\) is Latitude)
* \(ZX = z = 90^\circ - a\) (zenith distance, where \(a\) is True Altitude)
* \(PX = p\) (polar distance of Polaris, where \(p \approx 1^\circ\))
* \(\angle ZPX = h\) (Local Hour Angle of Polaris, \(\text{LHA}_\star\))

Let the zenith distance be \(z = c + k\), where \(k\) represents the correction to be applied to the altitude. Substituting \(z = 90^\circ - a\) and \(c = 90^\circ - L\):
\[90^\circ - a = (90^\circ - L) + k \implies L = a + k\]

---

### 2. Fundamental Spherical Trigonometry Relation

Applying the **Cosine Formula** to triangle \(PZX\):
\[\cos z = \cos p \cos c + \sin p \sin c \cos h\]

Substituting \(z = c + k\) into the left-hand side:
\[\cos(c + k) = \cos c \cos k - \sin c \sin k\]

Equating the two expressions for \(\cos z\):
\[\cos c \cos k - \sin c \sin k = \cos p \cos c + \sin p \sin c \cos h\]

Dividing both sides by \(\sin c\):
\[\cot c \cos k - \sin k = \cos p \cot c + \sin p \cos h\]

Rearranging terms:
\[\sin k = \cot c (\cos k - \cos p) - \sin p \cos h\]

---

### 3. Small Angle Expansion

Since \(p\) and \(k\) are small angles, express \(\sin\) and \(\cos\) as series expansions in radians:
\[\sin k \approx k, \quad \cos k \approx 1 - \frac{k^2}{2}\]
\[\sin p \approx p, \quad \cos p \approx 1 - \frac{p^2}{2}\]

#### **First Approximation**
Neglecting higher-order terms (\(\cos k \approx 1\) and \(\cos p \approx 1\)):
\[-k \approx p \cos h \implies k \approx -p \cos h\]

#### **Second Approximation**
Substituting the second-order terms back into the rearranged equation:
\[\cot c \left(1 - \frac{k^2}{2}\right) - k = \cot c \left(1 - \frac{p^2}{2}\right) + p \cos h\]

\[\cot c - \frac{1}{2} k^2 \cot c - k = \cot c - \frac{1}{2} p^2 \cot c + p \cos h\]

\[-k = \frac{1}{2} k^2 \cot c - \frac{1}{2} p^2 \cot c + p \cos h\]

\[k = -p \cos h + \frac{1}{2} \cot c (p^2 - k^2)\]

Substitute \(k \approx -p \cos h \implies k^2 \approx p^2 \cos^2 h\):
\[p^2 - k^2 = p^2 - p^2 \cos^2 h = p^2 (1 - \cos^2 h) = p^2 \sin^2 h\]

Since \(c = 90^\circ - L \implies \cot c = \tan L\):
\[k = -p \cos h + \frac{1}{2} p^2 \sin^2 h \tan L \quad \text{(in radians)}\]

Expressing \(p\) and \(k\) in minutes of arc (\(p', k'\)) using \(p' \sin 1' = \sin p\):
\[k = -p' \cos h + \frac{1}{2} p' \sin p \sin^2 h \tan L\]

---

### 4. Derivation of Table Correction Factors \(a_0, a_1, a_2\)

To avoid negative quantities in Nautical Almanac lookups, the correction \(k\) is decomposed into three positive values (\(a_0, a_1, a_2\)):

1. **\(a_0\) (Function of \(\text{LHA}_\gamma\))**:
   Computed using the main term \(-p' \cos h\) and the second term evaluated at a reference baseline latitude of \(50^\circ\text{N}\), using adopted mean values of SHA (\(327^\circ 39'\)) and declination (\(89^\circ 09.5'\)), plus an added constant of \(+58.8'\) to ensure \(a_0 > 0\):
   \[a_0 = -p' \cos h + \frac{1}{2} p' \sin p \sin^2 h \tan 50^\circ + 58.8'\]

2. **\(a_1\) (Function of \(\text{LHA}_\gamma\) and Latitude \(L\))**:
   Corrects for the difference between the observer's actual latitude \(L\) and the \(50^\circ\text{N}\) reference latitude, plus an added constant of \(+0.6'\):
   \[a_1 = \frac{1}{2} p' \sin p \sin^2 h (\tan L - \tan 50^\circ) + 0.6'\]

3. **\(a_2\) (Function of \(\text{LHA}_\gamma\) and Date / Declination)**:
   Adjusts for small seasonal/annual variations of Polaris's actual SHA and declination from the mean values, plus an added constant of \(+0.6'\):
   \[a_2 = (\text{variation correction}) + 0.6'\]

---

### 5. Final Latitude Formula

The total offset constant added across all three factors is:
\[\text{Sum of constants} = 58.8' + 0.6' + 0.6' = 60.0' = 1^\circ\]

Subtracting \(1^\circ\) to compensate for the added constants gives the final formula:
\[\text{Latitude } (L) = \text{True Altitude} - 1^\circ + a_0 + a_1 + a_2\]

---

