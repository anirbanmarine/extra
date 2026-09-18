---
Title: Numericals Answers Previous Years
type: docs
sidebar:
  open: true

---
## 2025

#### **Q.1 (a) Tapered Beam SF and BM Curves**
**Given:**
* Length of beam, \(L = 10 \) m
* Area at free end (\(x=0\)), \(A_0 = 6\) m²
* Area at fixed end (\(x=10\)), \(A_{10} = 16\) m²
* Density, \(\rho = 0.8\) kg/m³ *(Note: This is unusually low for a solid material and is likely a typo in the exam paper for \(800 \text{ kg/m}^3\) or \(0.8 \text{ t/m}^3\). The methodology below uses the given \(0.8 \text{ kg/m}^3\), but you can simply multiply the final forces by 1000 if \(800 \text{ kg/m}^3\) was intended).*

**Step 1: Equation for Area and Weight**
Since the taper is uniform, the cross-sectional area \(A(x)\) at distance \(x\) from the free end is:
\[A(x) = 6 + \left(\frac{16 - 6}{10}\right)x = 6 + x \text{ m}^2\]
Weight per unit length \(w(x) = \rho \cdot A(x) \cdot g = 0.8 \times 9.81 \times (6 + x) = 7.848(6 + x) \text{ N/m}\)

**Step 2: Shear Force (SF) Curve**
The shear force \(V(x)\) is the integral of the load from the free end:
\[V(x) = \int_{0}^{x} 7.848(6 + x) dx = 7.848 \left[ 6x + \frac{x^2}{2} \right]\]
* At \(x = 0\) (free end), \(V = 0\)
* At \(x = 10\) m (fixed end), \(V = 7.848 \times (60 + 50) = \mathbf{863.28 \text{ N}}\)
*(The SF curve is a parabolic shape starting at 0 and increasing to 863.28 N).*

**Step 3: Bending Moment (BM) Curve**
The bending moment \(M(x)\) is the integral of the shear force:
\[M(x) = \int_{0}^{x} 7.848 \left( 6x + \frac{x^2}{2} \right) dx = 7.848 \left[ 3x^2 + \frac{x^3}{6} \right]\]
* At \(x = 0\), \(M = 0\)
* At \(x = 10\) m, \(M = 7.848 \times \left( 300 + \frac{1000}{6} \right) = \mathbf{3662.4 \text{ Nm}}\)
*(The BM curve is a cubic shape starting at 0 and increasing to 3662.4 Nm at the fixed support).*

---

#### **Q.1 (b) Bilged Compartment Draft and GM**
**Given:**
* Box vessel: \(L = 140\) m, \(B = 20\) m, Initial draft \(T = 6\) m
* Midship compartment: \(l = 18\) m, width = \(16\) m
* Double hull (port, starboard, bottom) = \(2\) m each. Side tanks joined to DB in 'J' form.
* Permeability of cargo, \(\mu = 0.70\), \(KG = 5.1\) m

**Step 1: Lost Buoyancy Method for New Draft**
* Intact Waterplane (WP) Area = \((140 - 18) \times 20 = 122 \times 20 = 2440 \text{ m}^2\)
* Total flooded area at midship = \(18 \times 20 = 360 \text{ m}^2\)
* Cargo area = \(18 \times 16 = 288 \text{ m}^2\)
* Buoyant cargo area = \(288 \times 0.70 = 201.6 \text{ m}^2\)
* Lost buoyancy area = Total flooded area - Buoyant cargo area = \(360 - 201.6 = 158.4 \text{ m}^2\)
* Effective WP Area = Intact WP + Lost buoyancy area = \(2440 + 158.4 = 2598.4 \text{ m}^2\)

Original volume of displacement \(\nabla = 140 \times 20 \times 6 = 16800 \text{ m}^3\)
Effective displaced volume (excluding buoyant cargo) \(\nabla_{eff} = 16800 - (201.6 \times 6) = 15590.4 \text{ m}^3\)
**New Draft** = \(\nabla_{eff} / \text{Intact WP Area} = 15590.4 / 2440 = \mathbf{6.3895 \text{ m}}\)

**Step 2: Calculate New GM**
* **New KB:** For a box shape, \(KB = \text{New Draft} / 2 = 6.3895 / 2 = 3.1947 \text{ m}\)
* **New BM:** \(BM = I_{eff} / \nabla_{eff}\)
  * \(I_{intact} = \frac{1}{12} \times 122 \times 20^3 = 81333.33 \text{ m}^4\)
  * Effective width of flooded part = \(20 - (16 \times 0.7) = 8.8 \text{ m}\)
  * \(I_{flooded\_eff} = \frac{1}{12} \times 18 \times 8.8^3 = 1026.82 \text{ m}^4\)
  * Total \(I_{eff} = 81333.33 + 1026.82 = 82360.15 \text{ m}^4\)
  * \(BM = 82360.15 / 15590.4 = 5.2827 \text{ m}\)
* **New KM:** \(KM = KB + BM = 3.1947 + 5.2827 = 8.4774 \text{ m}\)
* **New GM:** \(GM = KM - KG = 8.4774 - 5.1 = \mathbf{3.377 \text{ m}}\)

---

#### **Q.2 (a) Simpson's First and Second Rules Derivation**
* **Simpson's First Rule (1-4-1):** Assumes the curve between 3 ordinates (2 intervals) is a second-degree polynomial \(y = a + bx + cx^2\). Integrating this equation from \(-h\) to \(+h\) yields the area formula: 
  \[\text{Area} = \frac{h}{3} (y_0 + 4y_1 + y_2)\]
  For \(n\) intervals (where \(n\) is even), it extends to: \(\frac{h}{3} (y_0 + 4y_1 + 2y_2 + 4y_3 + ... + y_n)\).
* **Simpson's Second Rule (1-3-3-1):** Assumes the curve between 4 ordinates (3 intervals) is a third-degree polynomial \(y = a + bx + cx^2 + dx^3\). Integrating this from \(-1.5h\) to \(+1.5h\) yields:
  \[\text{Area} = \frac{3h}{8} (y_0 + 3y_1 + 3y_2 + y_3)\]

#### **Q.2 (b) Moment of Inertia about y-axis**
Consider a vertical strip of width \(dx\) and height \(y\) at a distance \(x\) from the y-axis.
* Area of the strip, \(dA = y \cdot dx\)
* The Moment of Inertia (MI) of this strip about the y-axis is \(dI_y = x^2 \cdot dA\)
* Substituting \(dA\): \(dI_y = x^2 \cdot y \cdot dx\)
* Integrating over the entire curve: **\(I_y = \int y x^2 dx\)**

---

#### **Q.3 Interrelationship of Hull Girder Terms**
* **Bending Moment (M):** The internal algebraic sum of moments resisting external loads (weights and buoyancies).
* **Neutral Axis (NA):** The longitudinal axis within the ship's cross-section where the bending stress is zero. It passes through the centroid of the section.
* **Second Moment of Area (I):** Also called Moment of Inertia. It is the geometric property \(\int y^2 dA\) measuring the section's resistance to bending.
* **Section Modulus (Z):** Defined as \(Z = I / y_{max}\), where \(y_{max}\) is the distance from the NA to the outermost fiber (deck or keel).
* **Bending Stress (\(\sigma\)):** The stress induced by the bending moment, calculated using the Engineer's Bending Equation: \(\sigma = \frac{M}{Z} = \frac{M \cdot y}{I}\).
* **Hull Deflection:** The physical sagging or hogging deformation of the hull girder. It is mathematically linked to BM via the differential equation: \(EI \frac{d^2z}{dx^2} = M\), where \(E\) is Young's Modulus.
* **Interrelationship:** External loads create a **Bending Moment (M)**. The hull girder resists this via its **Second Moment of Area (I)** and **Section Modulus (Z)**, which dictates the maximum **Bending Stress (\(\sigma\))** at the deck/keel. If the stress exceeds the yield strength, permanent **Hull Deflection** or failure occurs.

---

#### **Q.4 Propeller Calculations**
**Given:** \(L=150\) m, \(B=24\) m, \(\Delta=25000\) t, \(T=9\) m, \(\rho=1.025\) t/m³, \(D=5.8\) m, Pitch Ratio=0.9, BAR=0.45, \(N=2\) rev/s, Apparent Slip (\(S_a\))=0.06, TP=3800 kW, \(\eta_P=0.64\).

**Step 1: Block Coefficient & Wake Fraction**
* \(\nabla = 25000 / 1.025 = 24390.24 \text{ m}^3\)
* \(C_b = \frac{24390.24}{150 \times 24 \times 9} = 0.7528\)
* Taylor Wake Fraction \(W_t = 0.5(0.7528) - 0.05 = \mathbf{0.3264}\)

**Step 2: Ship's Speed (a)**
* Pitch \(P = 0.9 \times 5.8 = 5.22\) m
* Speed of propeller \(V_p = P \times N = 5.22 \times 2 = 10.44\) m/s
* Apparent Slip \(S_a = \frac{V_p - V_s}{V_p} \implies V_s = V_p(1 - S_a) = 10.44(1 - 0.06) = 9.8136 \text{ m/s}\)
* **Ship Speed** = \(9.8136 \times \frac{3600}{1852} = \mathbf{19.07 \text{ knots}}\)

**Step 3: Real Slip Ratio (b)**
* Speed of advance \(V_a = V_s(1 - W_t) = 9.8136(1 - 0.3264) = 6.610 \text{ m/s}\)
* **Real Slip** = \(\frac{V_p - V_a}{V_p} = \frac{10.44 - 6.610}{10.44} = \mathbf{0.3668 \text{ (or 36.68\%)}}\)

**Step 4: Thrust per unit area (c)**
* Blade Area \(A_B = \text{BAR} \times \frac{\pi D^2}{4} = 0.45 \times \frac{\pi \times 5.8^2}{4} = 11.889 \text{ m}^2\)
* Thrust \(T = \frac{TP}{V_a} = \frac{3800}{6.610} = 574.88 \text{ kN}\)
* **Thrust per unit area** = \(\frac{574.88}{11.889} = \mathbf{48.35 \text{ kN/m}^2}\)

**Step 5: Torque delivered (d)**
* \(\eta_P = \frac{TP}{2 \pi N Q} \implies Q = \frac{3800}{2 \pi \times 2 \times 0.64} = \mathbf{472.49 \text{ kNm}}\)

---

#### **Q.5 (a) Ship Resistance from Model Test**
**Given:** Model \(L_m=6\) m, \(S_m=7\) m², \(V_m=3\) kts (\(1.543\) m/s), \(R_{tm}=35\) N. Ship \(L_s=120\) m. \(n=1.825\), SCF=1.15.
* Scale ratio \(\lambda = 120 / 6 = 20\).
* Ship speed \(V_s = V_m \sqrt{\lambda} = 3 \times \sqrt{20} = 13.416 \text{ knots} = 6.90 \text{ m/s}\).

Using the **ITTC 1957 Model-Ship Correlation Line**:
1. **Model Frictional Resistance:**
   \(Re_m = \frac{1.543 \times 6}{1.19 \times 10^{-6}} = 7.76 \times 10^6\)
   \(C_{fm} = \frac{0.075}{(\log_{10} Re_m - 2)^2} = 0.003138\)
   \(R_{fm} = \frac{1}{2} \rho S_m V_m^2 C_{fm} = 0.5 \times 1000 \times 7 \times 1.543^2 \times 0.003138 = 26.0 \text{ N}\)
2. **Residual Resistance:**
   \(R_{rm} = R_{tm} - R_{fm} = 35 - 26.0 = 9.0 \text{ N}\)
3. **Ship Residual Resistance:**
   \(R_{rs} = R_{rm} \times \left(\frac{\rho_s}{\rho_m}\right) \times \lambda^2 \times \lambda = 9.0 \times \left(\frac{1025}{1000}\right) \times 400 \times 20 = 73,800 \text{ N}\)
4. **Ship Frictional Resistance:**
   \(Re_s = \frac{6.90 \times 120}{1.19 \times 10^{-6}} = 6.95 \times 10^8\)
   \(C_{fs} = \frac{0.075}{(\log_{10} Re_s - 2)^2} = 0.00160\)
   \(R_{fs} = 0.5 \times 1025 \times (7 \times 400) \times 6.90^2 \times 0.00160 = 166,500 \text{ N}\)
5. **Total Ship Resistance:**
   Applying Ship Correlation Factor (SCF): \(R_{ts} = \text{SCF} \times (R_{fs} + R_{rs})\)
   \(R_{ts} = 1.15 \times (166500 + 73800) = \mathbf{276,345 \text{ N} \approx 276.3 \text{ kN}}\)

#### **Q.5 (b) Frictional Resistance Dependencies**
1. **Length of Ship:** Directly increases the wetted surface area. It also affects the Reynolds number, altering the frictional coefficient \(C_f\).
2. **Ship's Speed:** Frictional resistance is proportional to \(V^n\) (where \(n \approx 1.825\) according to Froude, or roughly \(V^2\) in turbulent flow).
3. **Wetted Surface Area:** Directly proportional; a larger surface area yields higher total frictional drag.
4. **Hull Roughness:** Increases the thickness of the viscous sublayer and disrupts the boundary layer, significantly increasing the frictional resistance coefficient over time due to corrosion, biofouling, and paint degradation.

---
## 2024

### **Q.1 (a) Area and Centroid of a Bounded Figure**
**Given:**
Radii at \(15^\circ\) intervals: \(r_0=0.2\), \(r_1=2.8\), \(r_2=5.4\), \(r_3=8.0\), \(r_4=10.7\), \(r_5=13.3\), \(r_6=15.9\) cm.
Common interval \(h = 15^\circ = \frac{\pi}{12}\) radians.

**Step 1: Calculate the Area**
Using Simpson's First Rule for polar coordinates: \(A = \frac{1}{2} \int r^2 d\theta \approx \frac{1}{2} \times \frac{h}{3} \sum (S \cdot r^2)\)
| \(\theta\) | \(r\) | \(r^2\) | Simpson's Multiplier (S) | Product |
| :--- | :--- | :--- | :--- | :--- |
| \(0^\circ\) | 0.2 | 0.04 | 1 | 0.04 |
| \(15^\circ\) | 2.8 | 7.84 | 4 | 31.36 |
| \(30^\circ\) | 5.4 | 29.16 | 2 | 58.32 |
| \(45^\circ\) | 8.0 | 64.00 | 4 | 256.00 |
| \(60^\circ\) | 10.7 | 114.49 | 2 | 228.98 |
| \(75^\circ\) | 13.3 | 176.89 | 4 | 707.56 |
| \(90^\circ\) | 15.9 | 252.81 | 1 | 252.81 |
**Sum** | | | | **1535.07**

\[A = \frac{1}{2} \times \frac{\pi/12}{3} \times 1535.07 = \frac{\pi}{72} \times 1535.07 = \mathbf{66.89 \text{ cm}^2}\]

**Step 2: Calculate the Centroid Position**
Distance from the initial bounding radius (\(\theta=0^\circ\)): \(\bar{y} = \frac{\frac{1}{3} \int r^3 \sin\theta d\theta}{A}\)
Distance from the final bounding radius (\(\theta=90^\circ\)): \(\bar{x} = \frac{\frac{1}{3} \int r^3 \cos\theta d\theta}{A}\)

Using Simpson's rule for \(\int r^3 \sin\theta d\theta\):
* Sum of products = \(0 + 4(5.68) + 2(78.73) + 4(362.04) + 2(1060.92) + 4(2272.47) + 4019.68 = 16859.74\)
* Integral \(= \frac{\pi}{36} \times 16859.74 = 1471.26\)
* \(\bar{y} = \frac{1}{3} \times \frac{1471.26}{66.89} = \mathbf{7.33 \text{ cm}}\)

Using Simpson's rule for \(\int r^3 \cos\theta d\theta\):
* Sum of products = \(0.008 + 4(21.20) + 2(136.37) + 4(362.04) + 2(612.52) + 4(608.88) + 0 = 5466.27\)
* Integral \(= \frac{\pi}{36} \times 5466.27 = 477.39\)
* \(\bar{x} = \frac{1}{3} \times \frac{477.39}{66.89} = \mathbf{2.38 \text{ cm}}\)

---

### **Q.1 (b) Mono-hull vs. Multi-hull Ships**
* **Comparison & Speed/Power Ratio:** Mono-hulls have a single V-shaped or U-shaped hull, offering high cargo capacity but suffering from high wave-making resistance at high Froude numbers. Multi-hulls (catamarans, trimarans) consist of narrow demihulls. This narrowness drastically reduces wave-making resistance at high speeds, giving multi-hulls a vastly superior **speed/power ratio** for fast cruising.
* **Examples:** Mono-hull (Container ships, VLCCs, conventional ferries). Multi-hull (High-speed crew boats, naval corvettes, luxury catamaran ferries).
* **Why Multi-hulls are smaller:** Scaling up a multi-hull requires an exponentially wider beam to maintain stability, leading to immense torsional and transverse bending stresses on the cross-deck structure connecting the hulls. Furthermore, large multi-hulls exceed the dimensions of standard locks, drydocks, and port infrastructure, making them structurally and economically unviable for bulk cargo transport compared to mono-hulls.

---

### **Q.2 (a) Propeller Cavitation Terms**
1. **Tip Cavitation:** Occurs at the blade tips due to the high pressure differential between the face and back. Water flows around the tip, creating a low-pressure vortex core that vaporizes the water.
2. **Sheet Cavitation:** Forms a continuous, stable sheet of vapor on the suction face (back) of the blade near the leading edge where the local pressure drops below the vapor pressure.
3. **Spot (Bubble) Cavitation:** Occurs as isolated, unstable vapor bubbles on the blade surface, often triggered by local surface roughness, pitting, or specific pressure pockets rather than a continuous low-pressure zone.

### **Q.2 (b) Rolling Decrement**
* **Decrement:** The progressive reduction in the maximum angle of roll in each successive cycle when a ship rolls in still water after an initial disturbance.
* **Graph:** An exponentially decaying sine wave (X-axis: Number of oscillations, Y-axis: Roll angle).
* **Causes of Amplitude Reduction:**
  1. **Frictional resistance** of the hull (skin friction).
  2. **Eddy-making resistance** (form drag due to hull shape).
  3. **Wave-making resistance** (energy radiated away as generated waves).
  4. **Lift forces on appendages** (e.g., bilge keels, rudders, stabilizing fins).

---

### **Q.3 Box Vessel Flooding Calculation**
**Given:** \(L=280\) m, \(B=22\) m, \(T=7\) m, \(GM=3.0\) m. 5 transverse compartments (Length = \(56\) m each). Centerline longitudinal bulkhead (Width = \(11\) m each). Forwardmost port compartment flooded.

**Step 1: Initial Particulars**
* \(\nabla = 280 \times 22 \times 7 = 43120 \text{ m}^3\)
* \(KB = 3.5\) m. \(I_{initial} = \frac{1}{12} \times 280 \times 22^3 = 248389.33 \text{ m}^4\)
* \(BM = 248389.33 / 43120 = 5.76\) m \(\implies KM = 3.5 + 5.76 = 9.26\) m
* \(KG = KM - GM = 9.26 - 3.0 = 6.26\) m

**Step 2: Lost Buoyancy Method (Bodily Sinkage)**
* Lost volume = \(56 \times 11 \times 7 = 4312 \text{ m}^3\)
* Intact WP Area = \((280 \times 22) - (56 \times 11) = 6160 - 616 = 5544 \text{ m}^2\)
* Sinkage = \(4312 / 5544 = 0.778\) m \(\implies\) **New Draft (\(T_1\)) = 7.778 m**
* New \(KB_1 = 7.778 / 2 = 3.889\) m

**Step 3: New Transverse Stability (List)**
* \(I_{lost} = [\frac{1}{12} \times 56 \times 11^3] + [616 \times (-5.5)^2] = 6209.33 + 18634 = 24843.33 \text{ m}^4\)
* \(I_{eff} = 248389.33 - 24843.33 = 223546 \text{ m}^4\)
* \(BM_1 = 223546 / 43120 = 5.184\) m \(\implies KM_1 = 3.889 + 5.184 = 9.073\) m
* **New \(GM_1\)** = \(9.073 - 6.26 = \mathbf{2.813 \text{ m}}\)
* List Moment = \(4312 \text{ t} \times 5.5 \text{ m (port)} = 23716 \text{ t-m}\)
* \(\tan\theta = 23716 / (43120 \times 2.813) = 0.1955 \implies\) **Rise at side (11m) = 2.15 m**

**Step 4: Longitudinal Stability (Trim)**
* New LCF position: \((6160 \times 140 - 616 \times 252) / 5544 = 127.56\) m from AP.
* Distance from LCF to FP = \(127.56\) m. Distance from LCF to AP = \(152.44\) m.
* \(I_{L, eff} = 40254933 - [\frac{1}{12} \times 11 \times 56^3 + 616 \times 112^2] = 32367296 \text{ m}^4\)
* \(MCTC = (43120 \times (32367296 / 43120)) / (100 \times 280) = 1156.24 \text{ t-m/cm}\)
* Trim Moment = \(4312 \times 112 = 482944 \text{ t-m}\)
* **Total Trim** = \(482944 / 1156.24 = 417.7 \text{ cm} = \mathbf{4.177 \text{ m (by the head)}}\)

**Step 5: Final Drafts**
* **Draft at FP** = \(7.778 + 4.177 \times (127.56 / 280) = \mathbf{9.68 \text{ m}}\)
* **Draft at AP** = \(7.778 - 4.177 \times (152.44 / 280) = \mathbf{5.50 \text{ m}}\)
* **Draft at FS** = \(9.68 + 2.15 \text{ (list rise)} = \mathbf{11.83 \text{ m}}\)
* **Draft at AS** = \(5.50 + 2.15 \text{ (list rise)} = \mathbf{7.65 \text{ m}}\)

---

### **Q.4 (a) Collision Bulkhead Thrust and COP**
**Given:** Triangle apex down, depth \(h=15\) m, top breadth \(b=18\) m. Sounding = \(17\) m (water is \(2\) m above the top edge).
* Area \(A = 0.5 \times 18 \times 15 = 135 \text{ m}^2\)
* Depth of centroid from top edge = \(15 / 3 = 5\) m.
* Depth of centroid from free surface (\(\bar{h}\)) = \(2 + 5 = 7\) m.
* **Thrust (\(F\))** = \(\rho g A \bar{h} = 1.025 \times 9.81 \times 135 \times 7 = \mathbf{9502 \text{ kN (or 9.5 MN)}}\)

**Center of Pressure (COP):**
* \(I_{centroid} = \frac{b h^3}{36} = \frac{18 \times 15^3}{36} = 1687.5 \text{ m}^4\)
* Depth of COP from free surface = \(\bar{h} + \frac{I_{centroid}}{A \bar{h}} = 7 + \frac{1687.5}{135 \times 7} = 7 + 1.786 = 8.786 \text{ m}\)
* Depth of COP from top edge = \(8.786 - 2 = 6.786 \text{ m}\)
* **Distance of COP from bottom** = \(15 - 6.786 = \mathbf{8.214 \text{ m}}\)

### **Q.4 (b) Oil Tanker Hull Strengths vs. Dry Cargo**
* **Stresses:** Tankers feature a continuous, uninterrupted strength deck (no large hatch openings) and a deep double bottom. This provides a massive section modulus, offering superior resistance to global hogging and sagging bending moments compared to dry cargo ships.
* **Stability:** The double bottom allows for very low KG (ballast tanks), yielding high initial GM. The centerline longitudinal bulkhead and wing tank arrangements provide excellent transverse stability and damage stability.
* **ILLC Considerations:** Because of their inherent structural continuity and double-hull damage stability (mandated by MARPOL), tankers are often assigned Type 'B' freeboards, which can be slightly reduced compared to Type 'A' if strict damage stability criteria are met, maximizing cargo deadweight.

---

### **Q.5 (a) Submarine Hull Construction**
* **Outer Hull:** Constructed from lightweight, hydrodynamically optimized materials (e.g., low-carbon steel or fiberglass). Its stress/strain curve shows a lower yield strength, as it is designed purely to minimize drag and house sonar/sensors, not to withstand deep-sea pressure.
* **Inner (Pressure) Hull:** Constructed from high-tensile steel (e.g., HY-80/HY-100). The stress/strain curve exhibits a very high yield point, high ultimate tensile strength, and high ductility. It is circular/cylindrical to distribute external hydrostatic pressure evenly as membrane stresses.
* **Negative Tank:** A specialized tank used to precisely control the submarine's buoyancy. By flooding it, the submarine overcomes positive buoyancy to dive or maintain a specific depth, compensating for weight changes (e.g., torpedo firing, fuel consumption).

### **Q.5 (b) Angle of Loll Derivation & Practical Application**
**Derivation:**
Wall-sided formula: \(GZ = \sin\theta \left( GM + \frac{1}{2} BM \tan^2\theta \right)\)
At the angle of loll, the ship is in unstable equilibrium, so \(GZ = 0\) for \(\theta \neq 0\).
Since \(\sin\theta \neq 0\), the term in the bracket must be zero:
\(GM + \frac{1}{2} BM \tan^2\theta = 0 \implies \tan^2\theta = \frac{-2 GM}{BM}\)
**\(\tan\theta = \sqrt{\frac{-2 GM}{BM}}\)** *(Note: GM is negative, making the root positive).*

**Practical Use for Timber Carrier:**
A 7-degree loll indicates a **negative GM**, likely caused by waterlogged timber deck cargo raising the VCG.
* **Action:** The Master must **NOT** attempt to correct the list by shifting weights or ballasting the high side, as this will cause the ship to capsize.
* **Correction:** The Master must lower the Center of Gravity (G). This is done by **jettisoning timber cargo from the high side** or pressing up/slack tanks low down on the low side to lower G without creating a free-surface moment.

---

### **Q.6 Safe Return to Port (SRtP) Regulations**
The SRtP regulations (SOLAS II-1/2-1) mandate that large passenger ships (typically Ro-Ro and cruise ships >120m) must be designed to survive a casualty (fire or flooding) and safely return to port under their own power, avoiding the need for immediate, dangerous at-sea evacuation.
* **Robustness & Redundancy:** Requires separation of essential systems (propulsion, steering, power) into multiple safe zones. If one zone is compromised, the ship retains enough power and steering to navigate to a safe haven.
* **Fire Safety:** Mandates strict fire zoning (A-60 boundaries) and the ability to isolate the fire while maintaining a "safe area" for passengers.
* **Damage Stability:** Ensures the ship remains afloat and stable with a limited heel angle (usually \(\le 10^\circ\)) even after multiple compartment flooding, allowing for safe internal movement and preventing capsizing.
* **Impact on Design:** Drives the integration of cross-flooding arrangements, multiple engine rooms, enhanced fire detection/suppression, and careful arrangement of muster stations to keep passengers safe during the transit back to port.

---
## 2023
### **Q.1 (a) Importance of Bonjean Curves**
**Definition & Diagram:** 
Bonjean curves are a set of curves plotted for each transverse section (station) of a ship. The X-axis represents the cross-sectional area of the immersed portion, and the Y-axis represents the draft. 
*(Sketch: A ship profile with vertical lines at each station. On each vertical line, a curve is plotted showing Area vs. Draft.)*

**Importance and Applications:**
1. **Longitudinal Strength in Waves:** They are the primary tool for calculating the buoyancy distribution along the ship's length when the vessel is in a wave. By superimposing the wave profile on the Bonjean curves, the exact immersed area at each station can be read, allowing for the calculation of Shear Forces and Bending Moments.
2. **Damage Stability & Floodable Length:** They are used to quickly determine the buoyancy lost and the new waterline when a compartment is bilged, aiding in the calculation of floodable length curves.
3. **Trim and Stability Calculations:** They allow for rapid estimation of displacement and Longitudinal Center of Buoyancy (LCB) for any arbitrary waterline (even when the ship is trimmed), which is crucial for loading and ballasting operations.

---

### **Q.1 (b) Screw Propeller Sketch**
*(Sketch Description: A 3D or 2D profile of a propeller blade attached to a central hub.)*
* **Hub:** The central cylindrical boss that connects the blades to the propeller shaft.
* **Blade Tip:** The outermost extremity of the blade, tracing the maximum propeller diameter circle.
* **Blade Root:** The inner edge of the blade where it merges into the hub.
* **Propeller Diameter:** The total diameter of the circle traced by the blade tips (\(2 \times\) Radius).
* **Pressure Face:** The face of the blade that pushes against the water to generate thrust (typically the aft-facing surface when moving ahead).
* **Suction Back:** The face of the blade that experiences low pressure, drawing water in (typically the forward-facing surface). This is the face most susceptible to cavitation.

---

### **Q.2 (a) Natural Frequency of Vertical Vibration**
**Given:** \(L = 150\) m, \(B = 18\) m, \(T = 8.5\) m, \(C_b = 0.70\), \(I = 195,000 \text{ m}^4\), Schlick Constant (\(C\)) = \(28,000\).

**Step 1: Calculate Displacement (\(\Delta\))**
\[\nabla = L \times B \times T \times C_b = 150 \times 18 \times 8.5 \times 0.70 = 16,065 \text{ m}^3\]
\[\Delta = \nabla \times \rho = 16,065 \times 1.025 = 16,466.6 \text{ tonnes}\]

**Step 2: Calculate Natural Period (\(T_V\)) and Frequency (\(f\))**
Using Schlick's formula for the 2-node vertical vibration period:
\[T_V = C \sqrt{\frac{\Delta \cdot L^3}{E \cdot I}}\]
*(Note: Assuming standard SI units where \(E \approx 2.06 \times 10^{11} \text{ N/m}^2\) for steel, and the constant \(C\) incorporates unit conversions).*
\[E \cdot I = 2.06 \times 10^{11} \times 195,000 = 4.017 \times 10^{16} \text{ N}\cdot\text{m}^2\]
\[T_V = 28000 \times \sqrt{\frac{16466.6 \times 150^3}{4.017 \times 10^{16}}} = 28000 \times \sqrt{\frac{5.557 \times 10^{12}}{4.017 \times 10^{16}}} = 28000 \times 0.01175 = \mathbf{3.29 \text{ seconds}}\]
**Natural Frequency (\(f\))** = \(1 / T_V = 1 / 3.29 = \mathbf{0.304 \text{ Hz}}\)

### **Q.2 (b) Effect on Curve of Static Stability**
1. **Grain Cargo Shift:** 
   * **Effect:** Shifting grain to one side creates a permanent heeling moment. The GZ curve is effectively shifted to the right by the angle of list (\(\theta_{list}\)). 
   * **Dynamical Stability:** The area under the GZ curve (which represents dynamical stability) is significantly reduced because the maximum righting lever is reached at a smaller angle relative to the new vertical, and the range of stability is curtailed.
2. **Formation of Ice:**
   * **Effect:** Ice accumulation adds weight high up on the ship (especially on masts, rigging, and exposed decks), raising the Vertical Center of Gravity (KG). This reduces the initial GM. The entire GZ curve is lowered, resulting in a reduced maximum GZ and a shorter range of stability.
   * **Dynamical Stability:** The total area under the curve (dynamical stability) is reduced, making the ship more vulnerable to capsizing in heavy seas.

---

### **Q.3 (a) Derivation of Natural Period of Roll (\(T_R\))**
**Derivation:**
For small angles of heel (\(\theta\)), the righting moment is \(RM = \Delta \cdot g \cdot GM \cdot \sin\theta \approx \Delta \cdot g \cdot GM \cdot \theta\).
The equation of motion for undamped rolling is:
\[I_{mass} \cdot \ddot{\theta} + \Delta \cdot g \cdot GM \cdot \theta = 0\]
Where \(I_{mass}\) is the mass moment of inertia, given by \(I_{mass} = \frac{\Delta}{g} k_{xx}^2\) (\(k_{xx}\) is the radius of gyration).
Substituting \(I_{mass}\):
\[\frac{\Delta}{g} k_{xx}^2 \ddot{\theta} + \Delta \cdot g \cdot GM \cdot \theta = 0 \implies \ddot{\theta} + \left( \frac{g^2 \cdot GM}{k_{xx}^2} \right) \theta = 0\]
This is the standard Simple Harmonic Motion equation (\(\ddot{\theta} + \omega_n^2 \theta = 0\)), where natural circular frequency \(\omega_n = \sqrt{\frac{g^2 \cdot GM}{k_{xx}^2}} = \frac{g \sqrt{GM}}{k_{xx}}\).
**Natural Period (\(T_R\))** = \(\frac{2\pi}{\omega_n} = \mathbf{\frac{2\pi \cdot k_{xx}}{g \sqrt{GM}}}\)

**Radius of Gyration (\(k_{xx}\)):** It is the theoretical distance from the axis of rotation (longitudinal axis) at which the entire mass of the ship could be concentrated to produce the same mass moment of inertia as the actual distributed mass.

### **Q.3 (b) Six Degrees of Freedom & Period Estimations**
**Degrees of Freedom:**
1. **Surge (X):** Linear motion along the longitudinal axis. *(No restoring force)*
2. **Sway (Y):** Linear motion along the transverse axis. *(No restoring force)*
3. **Heave (Z):** Linear motion along the vertical axis. *(Restoring force: Buoyancy)*
4. **Roll (\(\phi\)):** Angular motion about the longitudinal axis. *(Restoring force: Transverse Metacentric Height, GM)*
5. **Pitch (\(\theta\)):** Angular motion about the transverse axis. *(Restoring force: Longitudinal Metacentric Height, GM_L)*
6. **Yaw (\(\psi\)):** Angular motion about the vertical axis. *(No restoring force)*

**Estimations for the Tanker:**
* **Heaving Period (\(T_H\)):** \(T_H = 2\pi \sqrt{\frac{T}{g \cdot C_w}} = 2\pi \sqrt{\frac{13}{9.81 \times 0.85}} = \mathbf{7.83 \text{ seconds}}\)
* **Pitching Period (\(T_P\)):** \(T_P = 2\pi \sqrt{\frac{k_{yy}^2}{g \cdot GM_L}}\). Assuming \(k_{yy} \approx 0.25 L = 55\) m. 
  \(GM_L \approx BM_L = \frac{L^2 \cdot C_{wL}}{12 \cdot T \cdot C_b} = \frac{220^2 \times 0.85}{12 \times 13 \times 0.8} = 329.4 \text{ m}\).
  \(T_P = 2\pi \sqrt{\frac{55^2}{9.81 \times 329.4}} = \mathbf{6.07 \text{ seconds}}\)

---

### **Q.4 Procedure for Calculating Metacentric Height (Flooded Condition)**
**Given:** \(\Delta = 30,000\) t, \(T = 10\) m, \(TPC = 30\), Compartment \(12 \times 8\) m, \(\mu = 0.3\).

**Step 1: Calculate Lost Buoyancy Volume**
Since the compartment is on the centerline and permeability is 0.3, the lost buoyant volume is:
\[V_{lost} = l \times b \times T \times (1 - \mu) = 12 \times 8 \times 10 \times (1 - 0.3) = 672 \text{ m}^3\]

**Step 2: Calculate Bodily Sinkage and New Draft**
Intact Waterplane Area (\(A_{wp}\)) = \(TPC \times 100 / 1.025 = 30 \times 100 / 1.025 = 2926.8 \text{ m}^2\).
\[\text{Sinkage} = \frac{V_{lost}}{A_{wp}} = \frac{672}{2926.8} = 0.229 \text{ m}\]
**New Draft** = \(10 + 0.229 = \mathbf{10.229 \text{ m}}\)

**Step 3: Calculate New KB**
Assuming a wall-sided or box-shaped midship section, the new \(KB\) is approximately:
\[KB_{new} = KB_{old} + \frac{\text{Sinkage}}{2}\]

**Step 4: Calculate New BM**
\[BM_{new} = \frac{I_{new}}{\nabla_{new}}\]
* \(I_{new} = I_{old} - I_{lost} = I_{old} - \left(\frac{1}{12} \times 12 \times 8^3\right) = I_{old} - 512 \text{ m}^4\)
* \(\nabla_{new} = \nabla_{old} + (l \times b \times T \times \mu) = \frac{30000}{1.025} + (12 \times 8 \times 10 \times 0.3) = 29268.3 + 288 = 29556.3 \text{ m}^3\)

**Step 5: Calculate New GM**
\[KM_{new} = KB_{new} + BM_{new}\]
Since the KG of the ship does not change in the lost buoyancy method (the water entering the compartment is considered external to the ship's mass):
**New GM** = \(KM_{new} - KG_{old}\)

---

### **Q.5 (a) Angle of Loll and GM at Loll**
**Diagram & Explanation:** 
*(Sketch: A GZ curve starting from the origin. Because GM is negative, the initial slope is negative. The curve dips below the X-axis, reaches a minimum, and then crosses the X-axis again at an angle \(\theta_{loll}\). This crossing point is the angle of loll, where the ship rests in stable equilibrium.)*

**Calculation using Wall-Sided Formula:**
The wall-sided formula is: \(GZ = \sin\theta \left( GM + \frac{1}{2} BM \tan^2\theta \right)\)
At the angle of loll, the ship is in equilibrium, so \(GZ = 0\) (and \(\sin\theta \neq 0\)).
\[GM + \frac{1}{2} BM \tan^2\theta = 0 \implies \tan\theta_{loll} = \sqrt{\frac{-2 GM}{BM}}\]
**GM at the Angle of Loll:**
The metacentric height at the angle of loll (\(GM_{loll}\)) is positive and can be found by differentiating the GZ formula with respect to \(\theta\) and evaluating it at \(\theta_{loll}\). It is mathematically proven that:
**\(GM_{loll} = 2 \times |GM_{initial}|\)** (where \(GM_{initial}\) is the negative initial GM).

### **Q.5 (b) Grounding Calculation (Bilging on a Sand Bank)**
**Given:** \(\Delta = 10,000\) t, \(T = 6\) m, \(KG = 5.5\) m, Sounding = \(4\) m, \(KM = 6.0\) m, \(TPC = 22\).

**Step 1: Calculate Weight on Ground (\(P\))**
The ship has settled on the bottom, losing buoyancy equal to the weight of the water displaced by the difference in draft.
\[P = (T_{initial} - \text{Sounding}) \times TPC = (6 - 4) \times 22 = \mathbf{44 \text{ tonnes}}\]

**Step 2: Calculate Virtual Loss of GM**
The upward force \(P\) at the keel acts like a weight added at the keel, creating a virtual rise in KG (or virtual loss of GM).
\[\text{Virtual Loss of GM} = \frac{P \times KM}{\Delta} = \frac{44 \times 6.0}{10,000} = \mathbf{0.0264 \text{ m}}\]

**Step 3: Calculate New GM**
Original \(GM = KM - KG = 6.0 - 5.5 = 0.5 \text{ m}\).
**New GM** = Original \(GM\) - Virtual Loss = \(0.5 - 0.0264 = \mathbf{0.4736 \text{ m}}\)

---

### **Q.6 (a) Submarine Surfacing and Submerging**
**Submerging:** 
To dive, the submarine opens the main ballast tank (MBT) vents. Air escapes from the top of the tanks, and seawater floods in through the bottom flood ports, replacing the buoyant air. This reduces the ship's overall buoyancy. Hydroplanes are angled to generate downward dynamic lift to assist the dive and control the bow's pitch.

**Surfacing:** 
To surface, high-pressure air is blown into the MBTs, forcing the seawater out through the bottom flood ports. This restores positive buoyancy. 
**Use of Hydroplanes in Early Surfacing:** As buoyancy increases, the submarine might become unstable or the bow could dive due to hydrodynamic forces. Hydroplanes are angled to generate upward dynamic lift, helping the submarine break the surface cleanly, maintain a positive angle of attack, and prevent the bow from plunging back into the water before the MBTs are fully blown.

### **Q.6 (b) Alternative Intact Stability Criteria for Timber Carriers**
**IS Code 2008 Criteria:**
1. **Initial GM:** \(\ge 0.15\) m (or as per specific timber deck cargo calculations).
2. **Area under GZ curve:** \(\ge 0.08\) m.rad up to an angle of \(40^\circ\).
3. **Maximum GZ:** \(\ge 0.25\) m.
4. **Range of Stability:** \(\ge 25^\circ\).

**Reasons for Changed Criteria:**
Timber deck cargo provides additional buoyancy when submerged, which can increase the range of stability. However, it also adds significant weight high up (reducing GM), is susceptible to water absorption (increasing weight over time), and can shift if not properly secured. The criteria are specifically tailored to ensure the vessel has enough residual stability to counteract these adverse effects and the risk of cargo shift.

**Prerequisites:**
To be eligible for this alternative criteria, the ship must:
1. Comply with the International Convention on Load Lines (ICLL) regarding Timber Load Lines.
2. Have the timber cargo stowed upright and securely lashed.
3. The cargo must not extend forward of the superstructure or aft of the aft superstructure (if fitted).

---
## 2022

### **Q.1 (a) Hydrostatic Calculations using Simpson's Rules**
**Given:**
* LBP = 128 m, Breadth (B) = 18.30 m, Draft (T) = 8.25 m
* Midship Area (\(A_m\)) = 150.22 m²
* Station ordinates (in terms of \(A_m\)): 0, 0.5, 1, 2, 3, 4, 5(Amidships), 6, 7, 8, 9, 9.5, 10
* Values: 0.04, 0.16, 0.36, 0.73, 0.91, 1.0, 1.0, 1.0, 0.98, 0.86, 0.48, 0.21, 0.00

**Step 1: Calculate Volume and Displacement**
Because the intervals are not uniform (0.5 at the ends, 1.0 in the middle), we divide the calculation into segments. The common interval \(h\) for the main body is \(LBP/10 = 12.8\) m.
* **Forward Half (Stations 5 to 10):**
  * Stations 5 to 9 (4 intervals of \(h\)): Sum of products = \(1(1.0) + 4(1.0) + 2(0.98) + 4(0.86) + 1(0.48) = 10.88\)
  * Stations 9 to 10 (2 intervals of \(0.5h\)): Sum of products = \(1(0.48) + 4(0.21) + 1(0.00) = 1.32\)
  * Forward Volume = \(A_m \times \frac{h}{3} \times [10.88 + 1.32 \times 0.5] = 150.22 \times \frac{12.8}{3} \times 11.54 = 7396.4 \text{ m}^3\)
* **Aft Half (Stations 0 to 5):**
  * Stations 1 to 5 (4 intervals of \(h\)): Sum of products = \(1(0.36) + 4(0.73) + 2(0.91) + 4(1.0) + 1(1.0) = 10.10\)
  * Stations 0 to 1 (2 intervals of \(0.5h\)): Sum of products = \(1(0.04) + 4(0.16) + 1(0.36) = 1.04\)
  * Aft Volume = \(A_m \times \frac{h}{3} \times [10.10 + 1.04 \times 0.5] = 150.22 \times \frac{12.8}{3} \times 10.62 = 6806.7 \text{ m}^3\)
* **Total Volume (\(\nabla\))** = \(7396.4 + 6806.7 = \mathbf{14203.1 \text{ m}^3}\)
* **Displacement (\(\Delta\))** = \(14203.1 \times 1.025 = \mathbf{14558.2 \text{ tonnes}}\)** *(Note: Minor variations may occur based on exact integration methods used in the examiner's key, which lists 14858 t).*

**Step 2: Calculate Coefficients**
* **Block Coefficient (\(C_b\))** = \(\frac{\nabla}{L \times B \times T} = \frac{14203.1}{128 \times 18.3 \times 8.25} = \mathbf{0.736}\)
* **Midship Coefficient (\(C_m\))** = \(\frac{A_m}{B \times T} = \frac{150.22}{18.3 \times 8.25} = \mathbf{0.995}\)
* **Prismatic Coefficient (\(C_p\))** = \(\frac{C_b}{C_m} = \frac{0.736}{0.995} = \mathbf{0.740}\)

**Step 3: Calculate LCB and Centroid**
By taking moments of the volume functions about Amidships (Station 5) using the same Simpson's multipliers and intervals:
* Forward Moment Sum = 25.08 \(\rightarrow\) Forward Moment = \(16075.3 \text{ m}^4\)
* Aft Moment Sum = 22.16 \(\rightarrow\) Aft Moment = \(14203.2 \text{ m}^4\)
* Net Moment = \(16075.3 - 14203.2 = 1872.1 \text{ m}^4\)
* **LCB from Amidships** = \(\frac{1872.1}{14203.1} \times \frac{LBP}{2} = \mathbf{8.43 \text{ m Forward}}\) (or approx. 72.4 m from AP).

---

### **Q.1 (b) Hydrodynamic Interactions**
1. **Ship and River Bank (Bank Effect):**
   * **Causes:** As a ship moves in a narrow channel, the restricted waterway between the ship and the bank causes water velocity to increase. According to Bernoulli's theorem, this increases dynamic pressure and drops static pressure, creating a suction force that pulls the bow toward the bank and pushes the stern away, causing a sudden sheer.
   * **Remedies:** Reduce speed, maintain a safe distance from the bank, and apply proactive helm toward the bank to counteract the bow suction.
2. **Ship and Sea Bottom (Squat Effect):**
   * **Causes:** In shallow water, the flow of water under the hull is restricted, increasing velocity and decreasing pressure. This causes the ship to sink deeper (squat) and often change trim.
   * **Remedies:** Reduce speed (squat is proportional to the square of the speed), calculate under-keel clearance dynamically, and be aware of trim changes.

---

### **Q.2 (a) Ship Wave Pattern and Interference**
* **Wave Pattern:** A moving ship generates two primary wave systems: *Transverse waves* (moving at the ship's speed) and *Divergent waves* (angling outward at roughly 19.5° to the ship's path, forming the Kelvin wake).
* **Interference:** The bow and stern each generate their own wave systems. When these systems overlap, they interfere. If a bow crest meets a stern crest, they amplify each other (Hump). If a bow trough meets a stern crest, they cancel out (Hollow).
* **Humps and Hollows:** These occur in the wave-making resistance curve against \(V/\sqrt{L}\) due to this interference. Humps (high resistance) occur when the systems are in phase; hollows (low resistance) occur when they are out of phase.
* **Approximate Values:** The first major hump occurs at \(V/\sqrt{L} \approx 0.3\), and the first hollow occurs around \(V/\sqrt{L} \approx 0.4\) to \(0.5\).

### **Q.2 (b) Container Ship Speed Estimation**
**Given:** \(L = 122\) m. First trough of bow wave coincides with stern trough. Wave system distance = \(0.9L\).
* Wavelength (\(\lambda\)) = \(0.9 \times 122 = 109.8\) m.
* Using the wave speed formula \(V = 1.314 \sqrt{\lambda}\):
  \(V = 1.314 \times \sqrt{109.8} = 13.77 \text{ m/s} = \mathbf{26.7 \text{ knots}}\).
*(Note: The provided answer key states 20.271 knots, which implies a different interpretation of the wave interference formula or a specific empirical coefficient was expected, but the standard hydrodynamic derivation yields ~26.7 knots).*

---

### **Q.3 Curve of Static Stability**
**Given:** Cross curves (KN) are provided for VCG = 8.0 m. Actual KG = 10.0 m.
**Correction Formula:** \(GZ_{actual} = KN - KG_{actual} \sin\theta\)
*(Assuming the table provides KN values. If the table provides GZ at KG=8.0, the correction is \(GZ_{actual} = GZ_{table} + (8.0 - 10.0)\sin\theta\))*.
Using the standard KN correction:
* 0°: \(0 - 10(0) = \mathbf{0 \text{ m}}\)
* 15°: \(3.17 - 10(0.2588) = \mathbf{0.58 \text{ m}}\)** *(Derived KN from table context)*
* 30°: \(6.22 - 10(0.5) = \mathbf{1.22 \text{ m}}\)
* 45°: \(8.26 - 10(0.707) = \mathbf{1.19 \text{ m}}\)
* 60°: \(9.14 - 10(0.866) = \mathbf{0.48 \text{ m}}\)
* 75°: \(8.97 - 10(0.966) = \mathbf{-0.69 \text{ m}}\)
* 90°: \(8.30 - 10(1.0) = \mathbf{-1.70 \text{ m}}\)

**Results from the plotted curve:**
1. **Maximum GZ:** \(\approx \mathbf{1.22 \text{ m}}\)** *(Occurs around 30°-35°)*.
2. **Range of Stability:** From 0° to approx \(\mathbf{70^\circ}\) (where GZ crosses zero).
3. **Angle of Max GZ:** \(\approx \mathbf{32^\circ}\).
4. **Deck Edge Immersion:** Determined by the geometry of the midship section (typically where the freeboard deck angle is reached, often around 15°-20° for this hull form).

---

### **Q.4 (a) Virtual Gravity and Virtual Upright**
* **Virtual Gravity:** On a trochoidal wave, water particles move in circular orbits, creating a centrifugal force. The vector sum of the true downward gravity and this centrifugal force creates an effective "virtual gravity" that is always perpendicular to the wave surface.
* **Virtual Upright:** The ship's plumb bob will hang perpendicular to the wave surface. This direction is the "virtual upright." The ship will heel relative to this virtual upright, not the true vertical.
* **r and R:** 'R' is the radius of the wave profile (epicycle), and 'r' is the radius of the water particle's orbit at a given depth. \(r < R\) below the surface. At the crest, centrifugal force opposes gravity (reducing virtual gravity); at the trough, it adds to gravity.
* **Dangerous Conditions:** For small vessels like fishing boats, if the wave length is close to the ship's length, the rapid change in virtual gravity and transverse GM at the wave crest can cause a sudden loss of stability, leading to a sudden, catastrophic capsize (often associated with parametric rolling or pure loss of stability).

### **Q.4 (b) Parametric Rolling**
* **Reasons:** Ships with fine bows and full sterns experience massive fluctuations in waterplane area (and thus transverse GM) as waves pass along the hull. GM is lowest when a wave crest is at midships and highest when a trough is at midships.
* **Relationship:** If this periodic change in GM occurs at a frequency that matches the ship's natural roll frequency, it pumps energy into the roll. This happens when the **Encounter Period (\(T_E\)) is exactly half the Natural Rolling Period (\(T_R\))**, i.e., **\(T_R = 2 \times T_E\)**.

---

### **Q.5 (a) Submarine Systems**
1. **Trimming Tanks:** Located at the extreme forward and aft ends. They are used to transfer water to adjust the longitudinal center of gravity, ensuring the submarine remains level (neutral trim) during maneuvering and speed changes.
2. **Hull Buoyancy after Torpedo Ejection:** Firing a torpedo removes significant weight, making the sub positively buoyant. To compensate, water is immediately flooded into the torpedo room or a dedicated compensation tank to replace the lost weight.
3. **Depth Compensation Tank:** As a submarine dives, hydrostatic pressure compresses the hull, reducing its volume and buoyancy. This tank automatically or manually admits seawater to compensate for the "hull squeeze," maintaining neutral buoyancy at depth.

### **Q.5 (b) Planing Hull Boats**
* **Hydrodynamic Lift:** A hard chine hull generates lift dynamically. As the boat moves forward, the flat bottom pushes water downward. By Newton's third law, the water pushes the hull upward. The hard chine prevents water from spilling up the sides, concentrating the lift force under the flat bottom.
* **Poor Seakeeping:** Because the hull is flat, it does not slice through waves. Instead, it "slams" onto the water surface, causing severe vertical accelerations, structural shock, and a very rough, uncomfortable ride for passengers in any chop.

---

### **Q.6 (a) Derivation of Attwood's Formula**
1. Consider a ship heeled to a large angle \(\theta\). The emerged wedge (volume \(v\)) on the lowered side and the immersed wedge on the raised side must have equal volumes to maintain the same displacement.
2. The center of buoyancy shifts from \(B\) to \(B_1\) because the volume of the emerged wedge has effectively been "moved" to the immersed wedge.
3. Let \(y\) be the transverse distance of a small volume element \(v\) from the centerline axis. When moved from the emerged to the immersed wedge, its transverse shift is \(2y\).
4. The total transverse moment of the shifted buoyancy is \(\int v \cdot (2y)\).
5. The transverse shift of the center of buoyancy (\(BB_1 \cos\theta\)) is this total moment divided by the total displaced volume (\(\nabla\)).
6. From the geometry of the heeled ship, the righting lever \(GZ = (BB_1 \cos\theta) - BG \sin\theta\).
7. Substituting the moment, we get **Attwood's Formula**:
   \[GZ = \frac{\int v \cdot 2y}{\nabla} - BG \sin\theta\]

### **Q.6 (b) Limitations of the Wall-Sided Formula**
* **Limitations:** The formula \(GZ = \sin\theta (GM + \frac{1}{2} BM \tan^2\theta)\) strictly assumes that the ship's sides are perfectly vertical (wall-sided) at the waterline.
* **Relevance to "Wall" Sides:** At large angles of heel, the deck edge will inevitably immerse, or the bilge will emerge. The waterplane is no longer bounded by vertical sides, completely invalidating the geometric assumptions of the formula.
* **Why use other formulas:** For small angles (\(<10^\circ\)), the waterplane shape barely changes, and the metacenter \(M\) is fixed, making \(GZ = GM \sin\theta\) perfectly acceptable. At large angles, \(M\) moves significantly, and the waterplane shape changes drastically. Therefore, we must use cross curves of stability (derived from the actual 3D hull form at each angle) or Attwood's formula to accurately capture the true righting lever.

---
## 2021

### **Q.1 Bilged Compartment Draft and GM (Lost Buoyancy Method)**
**Given:**
* Box vessel: \(L = 140\) m, \(B = 20\) m, Initial draft \(T = 6\) m
* Midship compartment: \(l = 18\) m, width = \(16\) m (hold) + \(2\) m (port side tank) + \(2\) m (starboard side tank) = \(20\) m total width.
* Double bottom height = \(2\) m. Side tanks joined to DB in 'J' form.
* Permeability of cargo, \(\mu = 0.70\), \(KG = 5.1\) m.

**Step 1: Calculate Lost Buoyancy and New Draft**
* Intact Waterplane (WP) Area = \((140 - 18) \times 20 = 122 \times 20 = 2440 \text{ m}^2\)
* Total flooded volume of the compartment = \(18 \times 20 \times 6 = 2160 \text{ m}^3\)
* Buoyant volume of the cargo inside the hold = \(18 \times 16 \times 6 \times 0.70 = 1209.6 \text{ m}^3\)
* **Lost Buoyancy Volume** = Total flooded volume - Buoyant cargo volume = \(2160 - 1209.6 = 950.4 \text{ m}^3\)
* **Sinkage** = Lost Buoyancy / Intact WP Area = \(950.4 / 2440 = 0.3895 \text{ m}\)
* **New Draft** = \(6 + 0.3895 = \mathbf{6.3895 \text{ m}}\)

**Step 2: Calculate New GM**
* **New KB:** For a box shape, \(KB = \text{New Draft} / 2 = 6.3895 / 2 = 3.1948 \text{ m}\)
* **New BM:** \(BM = I_{eff} / \nabla_{eff}\)
  * Intact WP Moment of Inertia (\(I_{intact}\)) = \(\frac{1}{12} \times 122 \times 20^3 = 81333.33 \text{ m}^4\)
  * Inside the bilged compartment, the effective waterplane width is only the buoyant part of the cargo: \(16 \times 0.70 = 11.2 \text{ m}\).
  * Effective \(I\) inside compartment = \(\frac{1}{12} \times 18 \times 11.2^3 = 2115.17 \text{ m}^4\)
  * Total \(I_{eff} = 81333.33 + 2115.17 = 83448.5 \text{ m}^4\)
  * Effective displaced volume \(\nabla_{eff} = \text{Intact WP} \times \text{New Draft} = 2440 \times 6.3895 = 15590.38 \text{ m}^3\)
  * \(BM = 83448.5 / 15590.38 = 5.348 \text{ m}\)
* **New KM:** \(KM = KB + BM = 3.1948 + 5.348 = 8.5428 \text{ m}\)
* **New GM:** \(GM = KM - KG = 8.5428 - 5.1 = \mathbf{3.443 \text{ m}}\)

---

### **Q.2 Hydrostatic Calculations using Simpson's Rules**
**Given:** \(L = 91.46\) m, \(B = 14.63\) m, \(T = 3.66\) m, \(A_m = 51.40 \text{ m}^2\).
Common interval for main body \(2h = L/10 = 9.146\) m. Half-intervals at ends \(h = 4.573\) m.

**Step 1: Volume and Displacement**
Using Simpson's First Rule for the main body (Stations 0 to 10) and adding the half-intervals:
* Main Body Sum of Products = \(1(0.025) + 4(0.203) + 2(0.456) + 4(0.714) + 2(0.911) + 4(1.000) + 2(0.910) + 4(0.648) + 2(0.375) + 4(0.161) + 1(0.072) = 16.305\)
* Volume of main body = \(\frac{9.146}{3} \times 51.40 \times 16.305 = 2555.0 \text{ m}^3\)
* Forward Half (Stn 9 to 10) Sum = \(1(0.161) + 4(0.072) + 1(0.000) = 0.449 \implies V_{fwd} = \frac{4.573}{3} \times 51.40 \times 0.449 = 35.24 \text{ m}^3\)
* Aft Half (Stn 0 to 0.5) Sum = \(1(0.025) + 4(0.089) + 1(0.203) = 0.584 \implies V_{aft} = \frac{4.573}{3} \times 51.40 \times 0.584 = 45.77 \text{ m}^3\)
* **Total Volume (\(\nabla\))** = \(2555.0 + 35.24 + 45.77 = \mathbf{2636.01 \text{ m}^3}\)
* **Displacement (\(\Delta\))** = \(2636.01 \times 1.025 = \mathbf{2701.9 \text{ tonnes}}\)

**Step 2: Coefficients**
* **\(C_m\)** = \(A_m / (B \times T) = 51.40 / (14.63 \times 3.66) = \mathbf{0.960}\)
* **\(C_b\)** = \(\nabla / (L \times B \times T) = 2636.01 / (91.46 \times 14.63 \times 3.66) = \mathbf{0.538}\)
* **\(C_p\)** = \(C_b / C_m = 0.538 / 0.960 = \mathbf{0.560}\)

**Step 3: LCB and Centroid**
Taking moments about Amidships (Station 5) using lever arms in units of \((2h)\):
* Net Moment Sum = \(-1.453\) (Main) \(+ 1.940\) (Fwd Half) \(- 2.539\) (Aft Half) = \(-2.092\)
* Total Moment = \(\frac{9.146}{3} \times 51.40 \times (-2.092) \times 9.146 = -2993.5 \text{ m}^4\)
* **LCB from Amidships** = \(-2993.5 / 2636.01 = \mathbf{1.135 \text{ m Aft}}\)
* **Position of centroid from datum line (AP):** Distance from AP to Amidships = \(45.73\) m. LCB from AP = \(45.73 - 1.135 = \mathbf{44.595 \text{ m}}\). *(Note: Vertical centroid/KB cannot be calculated without the vertical center of each sectional area).*

---

### **Q.3 2005 ILLC Amendments for Type B Ships**
* **(a) Bow Height:** The 2005 amendments introduced stricter minimum bow height requirements to prevent green water on deck. For Type B ships (like bulk carriers), this ensures the forward hatch covers are not subjected to catastrophic dynamic wave impact loads, significantly reducing the risk of water ingress and subsequent loss of stability.
* **(b) Hatch Cover Design:** The amendments mandated higher design loads for hatch covers, requiring them to withstand increased sea pressures and dynamic loads. This forced an increase in scantlings, improved securing devices, and better weathertightness. Since water ingress through failed hatch covers is the primary cause of bulk carrier losses, this amendment directly enhances structural survivability in heavy weather.

---

### **Q.4 Wave Statistics and Stability**
**(a) SWH and H1/10 Calculation**
Total waves = \(6 + 30 + 17 + 9 + 3 = 65\) waves.
* **Significant Wave Height (SWH or \(H_{1/3}\)):** Average of the highest \(1/3\) (22 waves).
  * Top 22 waves: 3 of 1.8m, 9 of 1.5m, and 10 of 1.0m.
  * Sum = \((3 \times 1.8) + (9 \times 1.5) + (10 \times 1.0) = 5.4 + 13.5 + 10.0 = 28.9 \text{ m}\)
  * **SWH** = \(28.9 / 22 = \mathbf{1.31 \text{ m}}\)
* **One-Tenth Highest Wave (\(H_{1/10}\)):** Average of the highest \(1/10\) (7 waves).
  * Top 7 waves: 3 of 1.8m, and 4 of 1.5m.
  * Sum = \((3 \times 1.8) + (4 \times 1.5) = 5.4 + 6.0 = 11.4 \text{ m}\)
  * **\(H_{1/10}\)** = \(11.4 / 7 = \mathbf{1.63 \text{ m}}\)
* **Practical Significance:** SWH closely matches the visual estimate of an experienced observer and is the standard parameter used to define sea state for ship design, operational limits, and predicting extreme structural loads.

**(b) Hydrofoil Stability**
* **Surface-Piercing Foils:** V-shaped foils that pierce the water surface. When the craft heels, the immersed area of the lower foil increases (generating more lift), while the higher foil's area decreases. This differential lift creates a strong passive righting moment.
* **Submerged Foils:** Fully submerged foils rely on a dihedral angle for passive stability or an active electronic control system that adjusts the angle of attack to generate corrective lift forces when heel is detected.

**(c) Limitations of GM**
1. GM only defines *initial* stability (small angles \(<10^\circ\)) and does not indicate the maximum righting lever (GZ max) or the angle at which it occurs.
2. A ship with a large GM may have a short range of stability and low dynamical stability (small area under the GZ curve), making it prone to capsizing despite feeling "stiff".
3. GM fails to account for large-angle stability phenomena like deck edge immersion, freeboard loss, or the development of an angle of loll.

---

### **Q.5 Rudder Stock Design**
**Given:** \(A = 17 \text{ m}^2\), \(d = 1.1 \text{ m}\), \(v = 16 \text{ knots} = 8.23 \text{ m/s}\), \(\tau_{max} = 55 \text{ MN/m}^2\).
**Step 1: Rudder Force and Torque**
* \(F = 580 \times A \times v^2 = 580 \times 17 \times (8.23)^2 = 667,855 \text{ N}\)
* Torque \(T = F \times d = 667,855 \times 1.1 = 734,640 \text{ Nm}\)

**Step 2: Stock Diameter**
Using the torsion formula for a solid circular shaft: \(T = \frac{\pi}{16} \times \tau \times D^3\)
* \(D^3 = \frac{16 \times 734640}{\pi \times 55 \times 10^6} = 0.0680 \text{ m}^3\)
* **Diameter (\(D\))** = \(\sqrt[3]{0.0680} = \mathbf{0.408 \text{ m} \text{ (or 408 mm)}}\)

---

### **Q.6 Hull Failure and Drydocking**
**(a) Causes of Bulk Carrier Hull Failure (e.g., MV "Flare" / North Atlantic)**
1. **Bending Moment in Ballast:** In ballast, the ship experiences high still-water hogging. When combined with wave-induced sagging moments in heavy seas, it creates massive cyclic tensile and compressive stresses on the deck and bottom shell.
2. **Upkeep of Topside Tanks:** Corrosion in the topside (hopper) tanks reduces the section modulus of the hull girder, particularly at the deck and upper bilge strakes, creating localized weak points susceptible to cracking.
3. **Resonant Rolling:** Parametric or synchronous rolling in head or following seas can induce massive dynamic loads on the hull structure, rapidly propagating existing fatigue cracks.
4. **Brittle Fracture:** The freezing waters of the North Atlantic can drop the hull steel below its ductile-to-brittle transition temperature. Combined with high tensile stresses and existing corrosion/fatigue cracks, this leads to sudden, catastrophic brittle fracture of the hull girder without warning.

**(b) Virtual Loss of GM in Drydock**
**Diagram Description:** A midship cross-section resting on keel blocks. 
* **Vectors:** Gravity (\(W\)) acts downwards through \(G\). Buoyancy (\(B\)) acts upwards through \(B\). Upthrust (\(P\)) from the blocks acts upwards at the keel (\(K\)).
* **Derivation:** When the ship heels by a small angle \(\theta\), the upthrust \(P\) at the keel creates a listing moment. The horizontal shift of the keel is \(KM \sin\theta\). 
  * Listing Moment = \(P \times KM \sin\theta\)
  * The ship's natural Righting Moment = \(W \times GM \sin\theta\)
  * Effective Righting Moment = \(W \times GM \sin\theta - P \times KM \sin\theta = (W \times GM - P \times KM) \sin\theta\)
  * This must equal the new righting moment: \(W \times GM_{new} \sin\theta\)
  * Therefore, \(W \times GM_{new} = W \times GM - P \times KM\)
  * \(GM_{new} = GM - \frac{P \times KM}{W}\)
  * **Virtual Loss of GM** = \(\mathbf{\frac{P \times KM}{W}}\)** *(Notice that KG is completely eliminated from the final expression).*

---
## 2020

### **Q.1 Second-Generation Intact Stability Criteria**
**(a) Stability Failure Modes and Vulnerability Checks**
The IMO's second-generation intact stability criteria (SGISC) address five specific dynamic stability failure modes that were not adequately covered by the current weather criterion:
1. **Parametric Rolling:** Large roll angles induced by periodic variations in transverse stability (GM) in head or following seas.
2. **Pure Loss of Stability:** Sudden capsize due to a significant reduction in GM when a wave crest is at midships.
3. **Surf-Riding and Broaching-to:** Loss of control in following seas when the ship is caught by a wave and accelerated to wave speed, leading to a yaw and capsize.
4. **Dead Ship Condition:** Loss of stability and subsequent capsize of a vessel drifting in beam seas after a propulsion failure.
5. **Excessive Acceleration:** High vertical accelerations in head seas that can cause structural damage or injury to crew/passengers.

**Formalized Procedures:** For each mode, the criteria establish a formalized vulnerability check. **Level 1** checks are simple, criteria-based thresholds. If a vessel fails Level 1, it undergoes a more rigorous **Level 2** check, which uses advanced hydrodynamic simulations or simplified empirical formulas to assess the actual probability or severity of the failure mode in specific sea states.

**(b) Impact on Coastal Shipping**
Small coastal vessels often lack the detailed hydrodynamic data (like extensive model test results) required for the complex Level 2 assessments. The impact includes:
* **Compliance Burden:** Smaller operators may face high costs to generate the necessary data or perform numerical simulations.
* **Design Changes:** Vessels might need hull form modifications (e.g., adding bilge keels or changing bow flare) to pass the vulnerability checks.
* **Operational Restrictions:** If a vessel cannot meet the criteria, it may face strict weather windows or route restrictions, impacting its operational viability.

---

### **Q.2 Safe Return to Port (SRtP) and Industrial Personnel (IP) Code**
**(a) Evaluation of Safe Return to Port (SRtP)**
* **Applicability:** SRtP (SOLAS II-1/2-1) applies to passenger ships (especially Ro-Ro and cruise ships) of 120 m in length or more, built after 2010. It mandates that after a casualty (fire or flooding), the ship must retain essential systems to return to port without external assistance.
* **Effect on Costing & Operations:** It significantly increases initial capital expenditure due to the need for redundant systems (multiple engine rooms, separated power grids), enhanced fire zoning (A-60 boundaries), and dedicated "safe areas." Operationally, it requires rigorous crew training, complex emergency drills, and strict maintenance of redundant systems.
* **Passenger Capacity:** While dedicated safe areas and redundant machinery spaces consume valuable volume, the SRtP framework sometimes allows for a relaxation of strict evacuation time limits, potentially enabling higher passenger capacities on certain deck configurations compared to traditional SOLAS requirements.

**(b) Submissions to IMO SDC regarding >12 Industrial Personnel (IP)**
As a shipowner, my submissions to balance safety with operational feasibility would include:
1. **Safety Equipment (LSA & FFE):** While IPs are not crew, they are not traditional passengers either. I would propose that LSA and fire-fighting equipment meet cargo ship standards but scaled to the maximum number of IPs, rather than the full, costly passenger ship (SOLAS) standards.
2. **Training and Familiarization:** IPs often lack basic maritime safety training. I would submit that a mandatory, simplified "Basic Safety Induction" must be conducted before departure, covering muster stations, immersion suits, and basic fire awareness.
3. **Medical Facilities:** Offshore personnel are prone to industrial injuries. The code should mandate a dedicated medical room with telemedicine capabilities, rather than just standard passenger ship medical facilities.
4. **Chain of Command:** The code must explicitly state that the Master retains absolute authority over the vessel's safety and navigation, preventing conflicts between the offshore installation manager and the ship's Master during emergencies.

---

### **Q.3 Mid-Ship Section and Bending Stress**
*(Note: As Figure 1 of the mid-ship section is not provided in the text, the exact numerical values for Z cannot be calculated. Below is the exact step-by-step methodology and formulas required to solve this, followed by the bending stress calculation using the provided Bending Moments.)*

**Step-by-Step Procedure for Section Modulus (Z):**
1. **Tabulate Scantlings:** List all longitudinal structural members (deck, bottom, side shell, longitudinals) with their cross-sectional areas (\(a\)) and distances from a reference axis (usually the keel, \(y\)).
2. **Find Neutral Axis (NA):** Calculate the vertical center of the section. 
   \[KN = \frac{\sum (a \cdot y)}{\sum a}\]
3. **Calculate Moment of Inertia (\(I_{NA}\)):** For each member, calculate its own moment of inertia (\(i\)) and transfer it to the NA using the parallel axis theorem.
   \[I_{NA} = \sum \left( i + a \cdot (y - KN)^2 \right)\]
4. **Calculate Section Modulus (\(Z\)):** 
   \[Z_{deck} = \frac{I_{NA}}{y_{deck} - KN} \quad \text{and} \quad Z_{keel} = \frac{I_{NA}}{KN}\]

**Calculation of Total Bending Stress:**
* **Total Bending Moment (\(M_{total}\)):** Assuming the Still-Water Bending Moment (SWBM) and Wave Bending Moment (WBM) act in the same direction (e.g., both causing sagging):
  \[M_{total} = SWBM + WBM = 797 + 718 = \mathbf{1515 \text{ MNm}}\]
* **Bending Stress (\(\sigma\)):** Using the Engineer's Bending Equation (\(\sigma = M / Z\)):
  \[\sigma_{deck} = \frac{1515 \times 10^3}{Z_{deck}} \text{ kN/m}^2 \quad \text{and} \quad \sigma_{keel} = \frac{1515 \times 10^3}{Z_{keel}} \text{ kN/m}^2\]
*(Once \(Z_{deck}\) and \(Z_{keel}\) are calculated from the missing figure in \(m^3\), simply divide 1,515,000 by those values to get the stress in kN/m² or MPa).*

---

### **Q.4 Steel Coil Dunnage Calculation**
**Given:** Coil weight \(W = 20 \text{ T} = 196.2 \text{ kN}\), Dia = \(1 \text{ m}\), Width = \(1.6 \text{ m}\). Frame spacing (Span \(L\)) = \(750 \text{ mm}\).

**Step 1: Determine Load Category**
* Contact length = \(\frac{1}{12} \times \pi \times \text{Dia} = \frac{3.1416}{12} = 0.2618 \text{ m} = \mathbf{261.8 \text{ mm}}\)
* Check against Span (\(L = 750 \text{ mm}\)):
  * \(0.3 \times L = 225 \text{ mm}\)
  * \(0.7 \times L = 525 \text{ mm}\)
* Since \(225 \text{ mm} < 261.8 \text{ mm} < 525 \text{ mm}\), the load falls in the **intermediate category**. 
* Allowable load for the dunnage = \(1.5 \times P\) (where \(P\) is the allowable point load).

**Step 2: Select Dunnage Size and Type**
We need the allowable load (\(1.5 \times P\)) to support the coil. Let's test **100 mm \(\times\) 100 mm Hard Wood** (\(E = 10350 \text{ MPa}\), \(\sigma_{allow} = 55 \text{ MPa}\)).
* Allowable point load \(P\) for a simply supported beam with a midspan point load:
  \[M_{max} = \frac{P \cdot L}{4} \implies \sigma = \frac{M}{Z} = \frac{P \cdot L / 4}{b \cdot h^2 / 6} = \frac{1.5 \cdot P \cdot L}{b \cdot h^2}\]
  \[P = \frac{\sigma_{allow} \cdot b \cdot h^2}{1.5 \cdot L} = \frac{55 \times 100 \times 100^2}{1.5 \times 750} = \mathbf{48,888 \text{ N} \approx 48.89 \text{ kN} \text{ (or 4.98 T)}}\]
* Allowable load for this contact condition = \(1.5 \times 4.98 = \mathbf{7.47 \text{ Tonnes}}\).
* Number of dunnage pieces required per coil = \(\frac{20 \text{ T}}{7.47 \text{ T}} = 2.67 \implies \mathbf{3 \text{ pieces}}\).

**Step 3: Check Deflection**
* Limiting deflection = \(\frac{750 \text{ mm}}{375} = \mathbf{2 \text{ mm}}\).
* Actual deflection \(\delta = \frac{P \cdot L^3}{48 \cdot E \cdot I} = \frac{48888 \times 750^3}{48 \times 10350 \times (100 \times 100^3 / 12)} = \mathbf{0.0049 \text{ mm}}\).
* \(0.0049 \text{ mm} \ll 2 \text{ mm}\) (Safe).

**Answers:**
**(a) Type and Size:** Hard Wood dunnage, \(100 \text{ mm} \times 100 \text{ mm}\) cross-section.
**(b) Length of Dunnage:** Must be at least the width of the coil. Specify **\(1.6 \text{ m}\)** (or \(1.8 \text{ m}\) to allow for lashing/overhang).
**(c) Distribution:** Place **3 pieces** of \(100 \times 100 \times 1600 \text{ mm}\) Hard Wood dunnage transversely under the coil, spaced evenly along the \(1.6 \text{ m}\) length (approx. \(0.53 \text{ m}\) apart).
**(d) Variation across holds:** Dunnage requirements may vary if the tank top frame spacing differs between holds, or if the local deck strength (allowable load per \(m^2\)) is lower in certain holds, requiring more pieces of dunnage or larger scantlings to distribute the load.

---

### **Q.5 National Waterway Tanker Design**
**(a) Mid-Ship Section and Main Dimensions**
* **Payload (DWT):** \(2400 \text{ T}\)
* **Draft Restriction:** The most restrictive Least Available Depth (LAD) is \(2.5 \text{ m}\). Assuming an Under-Keel Clearance (UKC) of \(0.4 \text{ m}\), the maximum operational draft is \(2.1 \text{ m}\).
* **Main Dimensions:** 
  * Length (\(L\)) = \(110 \text{ m}\) (Max permitted)
  * Breadth (\(B\)) = \(12 \text{ m}\) (Max permitted)
  * Draft (\(T\)) = \(2.1 \text{ m}\)
  * Depth (\(D\)) = \(3.0 \text{ m}\) (Provides adequate freeboard and clearance for overhead bridges).
* **Block Coefficient (\(C_b\)):** \(\frac{2400}{110 \times 12 \times 2.1 \times 1.0 \text{ (fresh water)}} = 0.865\) (Typical for a river tanker).
* **Mid-Ship Section Description:** A double-bottom structure (to protect against grounding in shallow waterways), single deck with longitudinal framing, transverse side frames, and a centerline longitudinal bulkhead (or double side skins if pollution regulations mandate it). 
* **Factors Considered:** LAD constraints (dictating draft), topography/lock constraints (dictating beam), overhead bridges (dictating air draft/depth), payload requirement, and structural integrity for shallow water navigation.

**(b) Engine Power Evaluation**
* **Speed (\(V\)):** \(2 \text{ knots} = 1.029 \text{ m/s}\).
* **Wetted Surface Area (\(S\)):** Approx. \(L \times (B + 2T) \times 0.9 = 110 \times (12 + 4.2) \times 0.9 \approx 1600 \text{ m}^2\).
* **Frictional Resistance (\(R_f\)):** 
  * Reynolds number \(Re = \frac{1.029 \times 110}{1.19 \times 10^{-6}} \approx 9.5 \times 10^7\).
  * \(C_f = \frac{0.075}{(\log_{10} Re - 2)^2} \approx 0.00155\).
  * \(R_f = 0.5 \times 1000 \times 1600 \times 1.029^2 \times 0.00155 \approx 1315 \text{ N}\).
* **Total Resistance (\(R_t\)):** At this extremely low Froude number (\(Fn \approx 0.03\)), wave-making resistance is negligible. Assuming residual resistance is \(20\%\) of \(R_f\) and adding a \(15\%\) correlation allowance:
  * \(R_t \approx 1.15 \times 1.2 \times 1315 \approx 1815 \text{ N}\).
* **Effective Power (\(P_E\)):** \(R_t \times V = 1815 \times 1.029 \approx 1867 \text{ W} = \mathbf{1.87 \text{ kW}}\).
* **Shaft Power (\(P_S\)):** Assuming a low propulsive efficiency (\(\eta_D \approx 0.45\)) due to the low speed and small propeller:
  * \(P_S = \frac{1.87}{0.45} \approx \mathbf{4.15 \text{ kW}}\).
* **Conclusion:** A very small engine, such as a **5 kW to 10 kW** diesel or electric motor, is more than sufficient to propel this vessel at 2 knots.

---

### **Q.6 Change in GM for Connected Hulls**
**Given:** Single hull \(\Delta = 248 \text{ t}\), \(TPC = 0.5\), \(GM = 0.4 \text{ m}\). Distance between centerlines = \(7 \text{ m}\).

**Step 1: Understand the New Configuration**
When the two identical hulls are connected by a weightless platform:
* New Displacement \(\Delta_{new} = 2 \times 248 = 496 \text{ t}\).
* Since the platform is weightless, the vertical center of gravity remains unchanged: \(KG_{new} = KG\).
* The draft of each hull remains unchanged, so the vertical center of buoyancy remains unchanged: \(KB_{new} = KB\).

**Step 2: Calculate the New Transverse Moment of Inertia (\(I_{new}\))**
The new waterplane consists of the two individual waterplanes. The new centerline is exactly midway between the two hulls, so the distance from each hull's centerline to the new centerline is \(d = \frac{7}{2} = 3.5 \text{ m}\).
Using the parallel axis theorem:
\[I_{new} = 2 \times (I_{orig} + A_{wp} \cdot d^2)\]

**Step 3: Calculate the New BM**
\[BM_{new} = \frac{I_{new}}{\nabla_{new}} = \frac{2 \times (I_{orig} + A_{wp} \cdot d^2)}{2 \times \nabla} = \frac{I_{orig}}{\nabla} + \frac{A_{wp} \cdot d^2}{\nabla} = BM_{orig} + \frac{A_{wp} \cdot d^2}{\nabla}\]

**Step 4: Calculate the Change in GM**
Since \(KM = KB + BM\), and both \(KB\) and \(KG\) are unchanged:
\[\Delta GM = GM_{new} - GM_{orig} = KM_{new} - KM_{orig} = BM_{new} - BM_{orig} = \frac{A_{wp} \cdot d^2}{\nabla}\]

We know that \(A_{wp} = \frac{TPC \times 100}{\rho}\) and \(\nabla = \frac{\Delta}{\rho}\). Substituting these:
\[\Delta GM = \frac{\left(\frac{TPC \times 100}{\rho}\right) \cdot d^2}{\left(\frac{\Delta}{\rho}\right)} = \frac{TPC \times 100 \times d^2}{\Delta}\]

**Step 5: Final Calculation**
\[\Delta GM = \frac{0.5 \times 100 \times 3.5^2}{248} = \frac{50 \times 12.25}{248} = \frac{612.5}{248} = \mathbf{2.47 \text{ m}}\]

**Answer:** The GM increases by **2.47 meters**.