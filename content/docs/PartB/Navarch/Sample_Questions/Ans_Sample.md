---
Title: Sample Question and Answers
type: docs
sidebar:
  open: true

---
***

## Part 1: Submarine Design, Metallurgy & Stability

### 1. Metallurgy of Submarine Hulls: Why the Inner Hull Must Be Stronger

A submarine has a **double-hull** or **partial double-hull** construction:

- **Inner hull (pressure hull)**: Withstands external hydrostatic pressure at depth. Must resist **elastic buckling** and **plastic collapse**.
- **Outer hull (light hull)**: Provides hydrodynamic shape, protects internal systems, and houses ballast tanks. It is **not pressure-tight** and experiences minimal stress.

#### Why the inner hull is stronger:
At depth \( h \), external pressure is:
\[
P = \rho g h
\]
where \( \rho \approx 1025 \, \text{kg/m}^3 \) (seawater), \( g = 9.81 \, \text{m/s}^2 \).

At 300 m depth:
\[
P \approx 1025 \times 9.81 \times 300 \approx 3.0 \, \text{MPa} \, (\approx 30 \, \text{bar})
\]

This pressure acts uniformly on the inner hull, creating **compressive hoop stress**:
\[
\sigma_{\theta} = \frac{P \cdot r}{t}
\]
where \( r \) = hull radius, \( t \) = hull thickness.

If \( \sigma_{\theta} \) exceeds yield strength or causes buckling, catastrophic implosion occurs. Hence, the inner hull uses **high-yield, low-alloy steels** with excellent toughness at low temperatures.

#### Materials Used:

| Hull Type | Typical Materials | Yield Strength (MPa) | Key Properties |
|-----------|------------------|----------------------|----------------|
| **Inner (Pressure) Hull** | HY-80, HY-100, HY-130 (US); TI-6Al-4V (titanium, Russian Alfa-class); NS110 (modern) | 550–900+ | High yield, fracture toughness, weldability, corrosion resistance |
| **Outer (Light) Hull** | Mild steel (A36), stainless cladding, composites | 250–350 | Formability, corrosion resistance, low cost |

**Stress-Strain Diagram Insight**:

- **Inner hull steel (HY-100)**: High yield plateau, large plastic region before necking → absorbs energy without brittle fracture.
- **Outer hull steel (A36)**: Lower yield, earlier plastic deformation → acceptable since it doesn’t bear pressure.

```
Stress (σ)
  |
  |        HY-100 (Inner Hull)
  |       /¯¯¯¯¯¯¯¯¯¯¯\
  |      /             \______
  |     /
  |    /   A36 (Outer Hull)
  |   /   /¯¯¯¯¯\_____
  |  /   /
  | /   /
  |/___/______________ Strain (ε)
```

The inner hull must remain **elastic** up to design depth; plastic deformation = failure.

***

### 2. Ballast Tanks: Functions & Locations

Submarines use **ballast tanks** to control buoyancy and trim. Key types:

| Tank Type | Location | Function |
|-----------|----------|----------|
| **Main Ballast Tanks (MBTs)** | Between inner & outer hull, along sides & bottom | Flood to submerge; blow with HP air to surface |
| **Trim Tanks (Forward/Aft)** | Inside pressure hull, near bow/stern | Fine-tune longitudinal balance (trim angle) |
| **Negative Tank** | Usually forward, inside pressure hull | Provides **negative buoyancy** for rapid dive; blown early in ascent |
| **Safety Tank** | Often amidships | Emergency buoyancy reserve |
| **Compensation Tank** | Variable | Adjusts for weight changes (e.g., torpedo firing) |

#### Diagram: Ballast Tank Layout (Simplified)

```
         [Outer Hull]
   ┌─────────────────────────┐
   │ MBT │ MBT │ MBT │ MBT   │ ← Main Ballast (floodable)
   │─────┴─────┴─────┴───────│
   │ [Pressure Hull Interior]│
   │ Neg │ Trim F │ Trim A   │ ← Negative + Trim Tanks
   └─────────────────────────┘
```

- **MBTs**: Always vented at top; flood from bottom → air escapes, water enters → submarine loses buoyancy.
- **Trim/Negative**: Pump-controlled; used for precise depth/angle control.

***

### 3. How a Submarine Surfaces & Submerges

#### Submerging:
1. **Open MBT vents** → air escapes, seawater floods tanks.
2. **Buoyancy decreases** → submarine becomes negatively buoyant.
3. **Use diving planes** (bow/stern) to control descent angle.
4. **Trim tanks** adjusted to maintain level dive.

#### Surfacing:
1. **Close MBT vents**, inject **high-pressure air** → forces water out.
2. **Buoyancy increases** → submarine rises.
3. **Blow negative tank early** for positive lift.
4. **Trim tanks** compensate for shifting center of gravity.

```
Submerging:          Surfacing:
  Air out              Air in (HP)
  Water in → ⬇         Water out → ⬆
  Negative buoyancy    Positive buoyancy
```

***

### 4. Role of Negative & Trim Tanks

- **Negative Tank**: Provides **instant negative buoyancy** for emergency dives. During surfacing, it’s blown **first** to initiate ascent.
- **Trim Tanks**: Maintain **zero trim angle** (level). When flooding MBTs, water distribution may shift G (center of gravity); trim tanks pump water fore/aft to realign G with B (center of buoyancy).

Without trim control, the submarine would pitch uncontrollably during depth changes.

***

### 5. Intact Stability: Transverse vs. Longitudinal (Surfaced vs. Submerged)

#### Surfaced Condition:
- Behaves like a **surface ship**.
- **Transverse stability**: Depends on waterplane area → large BMₜ (metacentric radius).
- **Longitudinal stability**: Much larger BMₗ due to elongated waterplane.

#### Submerged Condition:
- **No waterplane** → BM = 0 (no buoyancy shift with heel).
- **B (center of buoyancy)** is fixed relative to hull.
- **Stability depends entirely on G-B separation**:
  - **G below B** → stable (like a pendulum).
  - **G above B** → unstable.

```
Surfaced:          Submerged:
   M                   B
   |                   |
   B                   |
   |                   G (must be < B)
   G
```

- **Transverse GM (submerged)**: \( GM_t = KB - KG \) (since BM = 0)
- **Longitudinal GM (submerged)**: Same formula, but G-B alignment is critical for pitch control.

***

### 6. Righting Moment: Mono-hull Ship vs. Submerged Submarine

#### Surface Ship:
- Heel → **B shifts outward** → creates righting arm GZ.
- **M (metacenter)** is above G → positive GM.
- Righting Moment: \( RM = \Delta \cdot GZ = \Delta \cdot GM \cdot \sin\theta \)

#### Submerged Submarine:
- **B does not shift** (fully submerged, no waterplane).
- **No metacenter (M)** → stability from **G below B**.
- Righting Moment: \( RM = \Delta \cdot (KB - KG) \cdot \sin\theta \)

```
Surface Ship:       Submarine (Submerged):
     M                    B
     |                    |
     B                    |
     |                    G
     G
   GZ = GM·sinθ         GZ = (KB-KG)·sinθ
```

Submarines have **much smaller righting moments** when submerged → rely on active control (planes, trim) rather than passive stability.

***

### 7. GM Longitudinal vs. Transverse in Submarines

| Parameter | Surfaced Submarine | Submerged Submarine | Surface Ship |
|-----------|-------------------|---------------------|--------------|
| **GMₜ (Transverse)** | Large (waterplane exists) | Small (KB – KG only) | Large |
| **GMₗ (Longitudinal)** | Very large (L² effect) | Same as GMₜ (KB – KG) | Very large |
| **Stability Source** | Waterplane + G-B | G-B only | Waterplane + G-B |
| **Risk** | Capsizing if GM too low | Pitch/roll divergence if G > B | Capsizing, parametric roll |

**Key Insight**: In submerged condition, **GMₗ ≈ GMₜ** (both depend only on vertical G-B separation), unlike surface ships where GMₗ >> GMₜ.

***

## Part 2: Wave Mechanics for Ship Stability & Safety

### 1. Trochoidal Waves: Definition & Geometry

A **trochoidal wave** models real ocean waves more accurately than sinusoidal waves. It describes the path of a water particle as a **trochoid curve**—generated by a point on a rolling circle.

#### Definition:
A trochoid is the curve traced by a point at distance \( r \) from the center of a circle of radius \( R \) rolling along a straight line.

- If \( r = R \): **Cycloid** (sharp crest, flat trough)
- If \( r < R \): **Prolate trochoid** (realistic ocean wave)
- If \( r > R \): **Curtate trochoid** (not physical for waves)

#### Key Parameters:
- \( R \): Radius of rolling circle = \( \frac{L}{2\pi} \), where \( L \) = wavelength
- \( r \): Radius of particle orbit = decreases with depth
- **Still Water Line (SWL)**: Datum at mean water level
- **Particle P**: Moves in circular orbit; radius \( r \) at surface, decays exponentially with depth

#### Trochoidal Wave Diagram:

```
        Crest
          *
         / \
        /   \      Particle P at crest:
       /     \     → Moving forward (→)
------*-------*---- Still Water Line (SWL)
     /         \
    /           \   Particle P at trough:
   /             \  → Moving backward (←)
  *               *
 Trough         Crest

Circle radius R = L/2π
Particle orbit radius r (≤ R)
```

**Particle Motion**:
- At **crest**: P moves **forward** (in wave direction)
- At **trough**: P moves **backward**
- At **SWL (rising)**: P moves **upward**
- At **SWL (falling)**: P moves **downward**

Orbit radius at depth \( z \):
\[
r(z) = r_0 \cdot e^{-kz}, \quad k = \frac{2\pi}{L}
\]

***

### 2. Significant Wave Height (\( H_s \) or \( H_{1/3} \))

#### Definition:
The **average height of the highest one-third** of waves in a record. It approximates what an experienced observer would report as “significant” wave height.

#### Calculation Example:
Given 12 wave heights (m):  
\[ 2.1, 3.5, 4.2, 2.8, 5.0, 3.9, 4.5, 3.2, 6.1, 4.8, 3.7, 5.5 \]

1. Sort descending:  
\[ 6.1, 5.5, 5.0, 4.8, 4.5, 4.2, 3.9, 3.7, 3.5, 3.2, 2.8, 2.1 \]

2. Top 1/3 = 4 waves: 6.1, 5.5, 5.0, 4.8  
3. \( H_s = \frac{6.1 + 5.5 + 5.0 + 4.8}{4} = 5.35 \, \text{m} \)

#### Extreme Waves:
- **\( H_{max} \)**: Typically  \approx 1.8–2.0 \times H_s  in fully developed seas
- **North Atlantic**: Design H_s \approx 14–16 \, \text{m} ;  H_{max}  can exceed 25 m → influences hull scantlings, hatch cover loads, freeboard assignment .

***

### 3. Natural Period of Roll (\( T_\phi \))

Derived from **simple harmonic motion** analogy:

Restoring moment for small heel \( \phi \):
\[
M_R = \Delta \cdot GM \cdot \sin\phi \approx \Delta \cdot GM \cdot \phi
\]

Moment of inertia about roll axis:
\[
I = \Delta \cdot k^2 / g
\]
where \( k \) = radius of gyration in roll  \approx 0.35–0.45 \times B .

Equation of motion:
\[
I \cdot \ddot{\phi} + \Delta \cdot GM \cdot \phi = 0
\]

Natural period:
\[
T_\phi = 2\pi \sqrt{\frac{I}{\Delta \cdot GM}} = 2\pi \sqrt{\frac{k^2}{g \cdot GM}}
\]

Simplified empirical formula (Derrett’s):

T_\phi \approx \frac{C \cdot B}{\sqrt{GM}}, \quad C \approx 0.75–0.85


#### Example (Bulk Carrier from your data):
- \( B = 32.6 \, \text{m} \), \( GM = 0.885 \, \text{m} \), assume \( C = 0.8 \)

\[
T_\phi \approx \frac{0.8 \times 32.6}{\sqrt{0.885}} \approx \frac{26.08}{0.941} \approx 27.7 \, \text{s}
\]

This is **dangerously long** → risk of synchronous rolling with typical ocean wave periods (8–15 s).

***

### 4. Synchronous Rolling & Parametric Rolling

#### Synchronous Rolling:
Occurs when **wave encounter period \( T_E \)** matches ship’s natural roll period \( T_\phi \).

**Encounter period** (for heading angle \( \mu \)):
\[
T_E = \frac{L_w}{V_w + V_s \cos\mu}
\]
where \( L_w \) = wavelength, \( V_w \) = wave celerity, \( V_s \) = ship speed.

**Danger**: Even moderate waves can cause **resonant roll amplification** → capsizing (e.g., APL CHINA, 1988) .

**APL CHINA Case**:
- Container ship in North Pacific storm
- Large roll angles (>30°) → container losses
- Cause: **Synchronous rolling** in beam seas + low GM
- Solution: **Increase GM** (counterintuitive: usually mariners reduce GM for comfort) .

#### Parametric Rolling:
Occurs in **head or following seas** when wave passage modulates GM periodically.

**Conditions**:
- Fine bow, wide stern (container ships, cruise vessels)
- Wave length ≈ ship length
- Ship speed such that **pitch period ≈ ½ × roll period**

**Mechanism**:
- Crest amidships → waterplane narrows → GM decreases
- Trough amidships → waterplane widens → GM increases
- If GM variation frequency ≈ 2× roll frequency → **parametric resonance** → roll angles >40° possible.

**Avoidance Strategies**:
1. **Change speed** → alter encounter period
2. **Alter course** → move away from head/following seas
3. **Adjust GM** (ballast transfer)
4. **Activate anti-roll tanks/fins**

***

### 5. Virtual Gravity & Virtual Upright (Trochoidal Waves)

On a trochoidal wave, the **effective gravity vector** tilts due to centrifugal acceleration of water particles.

#### Virtual Gravity (\( g' \)):
\[
g' = g - \omega^2 r
\]
where \( \omega \) = wave angular frequency, \( r \) = particle orbit radius.

#### Virtual Upright:
The direction perpendicular to the **local wave slope** (not horizontal). A ship on a wave crest “feels” upright relative to the sloped surface.

**Danger to Small Craft**:
- Fishing vessels on steep waves → **virtual upright misaligns with true vertical**
- Crew perceives stability when actually **GZ is reduced**
- Sudden wave trough → loss of righting moment → capsize

```
True Vertical      Virtual Upright
     ↓                  ↖
     |                   \
     |                    \  Wave slope
-----*---------------------*---- SWL
     |                   /
     |                  /
     ↓                 ↙
  Gravity           Virtual Gravity
```

***

### 6. MSC Circular 1228: Avoiding Dangerous Situations

#### Core Assumptions:
1. Waves are **trochoidal**, not sinusoidal.
2. Ship motions are **linear** (small angles) — limitation in extreme seas.
3. **Resonant interactions** dominate risk (synchronous roll, parametric roll, surf-riding).

#### Key Parameters:
| Parameter | Symbol | Risk Threshold |
|-----------|--------|----------------|
| Wave height | \( H_w \) | > 0.05 × LBP |
| Wave period | \( T_w \) | ≈ \( T_\phi \) or \( 0.5 T_\phi \) |
| Encounter period | \( T_E \) | Match \( T_\phi \) → synchronous |
| GM | — | Too low → large rolls; too high → short, violent rolls |

#### Limitations:
- Assumes **regular waves** — real seas are irregular (spectral).
- Does not account for **wind drift**, **current**, or **loading changes**.
- **Masters must observe** actual \( T_w \), \( H_w \), and adjust speed/course proactively.

***

### 7. Surfing, Broaching, and Pooping

#### Surfing (Following Seas):
- Ship speed ≈ wave celerity → vessel “surfs” down wave face.
- Risk: **Loss of steerage**, **broaching** (sudden yaw to beam seas).

#### Broaching:
- Stern lifted by wave → rudder/propeller emerge → loss of control.
- Ship turns beam-to-sea → **large roll moment** → capsize.

#### Pooping (Stern Seas):
- Wave breaks over stern → flooding, structural damage.

**Avoidance**:
- **Reduce speed** in following seas > 0.7 × wave celerity.
- **Alter course** to 30–45° off wave direction.

***

### 8. Resonant vs. Non-Resonant Ship-Wave Interactions

```
Flowchart:
Start
  ↓
Measure Tw, Hw, Ship Speed, Heading
  ↓
Calculate TE (Encounter Period)
  ↓
Is TE ≈ Tϕ? ───Yes───> Synchronous Rolling (Resonant) → Change course/speed
  ↓ No
Is TE ≈ 0.5 Tϕ? ─Yes───> Parametric Rolling (Resonant) → Adjust GM/speed
  ↓ No
Is Vs ≈ Vw·cosμ? ─Yes───> Surf-riding/Broaching (Non-resonant) → Slow down
  ↓ No
Safe Zone (Non-resonant) → Monitor continuously
```

**Examples**:
- **Resonant**: APL CHINA (synchronous), modern container ships (parametric)
- **Non-resonant**: RoPax in quartering seas (broaching), fishing vessel pooping

***

### 9. Guidance Note to Masters (Safety Superintendent)

**Subject**: Avoiding Synchronous Rolling & Pooping in Adverse Weather

**Observations Required**:
1. **Wave Period (\( T_w \))**: Time between 5 consecutive crests → average.
2. **Wave Height (\( H_w \))**: Visual estimate or radar.
3. **Ship’s Roll Period (\( T_\phi \))**: Measure 5 rolls → average.

**Actions**:
- If \( T_w \approx T_\phi \): **Alter course by 20–30°** or **change speed by 20%**.
- If following seas: **Ensure \( V_s < 0.7 V_w \)** to avoid surf-riding.
- **Log all observations** in deck logbook + report to shore.

**Diagram: Wave Observation**:

```
Creast:  *     *     *     *
         |<--Tw-->|
         |<------ 5Tw ------>| → Average for accuracy
```

***

### 10. Rolling & Pitching Estimation (Your Bulk Carrier Data)

Given:
- \( L = 217 \, \text{m} \), \( B = 32.6 \, \text{m} \), \( T = 12.2 \, \text{m} \), \( GM = 0.885 \, \text{m} \)

**Roll Period** (as above): \( T_\phi \approx 27.7 \, \text{s} \)

**Pitch Period** (empirical):

T_\theta \approx \frac{L}{\sqrt{g \cdot GM_L}}, \quad GM_L \approx 100\text{~}300 \, \text{m}

Assume \( GM_L = 200 \, \text{m} \):
\[
T_\theta \approx \frac{217}{\sqrt{9.81 \times 200}} \approx \frac{217}{44.3} \approx 4.9 \, \text{s}
\]

**Risk**: \( T_\phi \) is too long → high synchronous roll risk in beam seas of 12–15 s waves (common in North Atlantic).

***


## Part 3: Tanker vs. Bulk Carrier Design & Safety

### 1. Inherent Strength: Tanker vs. Dry Cargo Ship

#### Tanker Advantages:
- **Continuous longitudinal strength**: Cargo tanks act as **integral part of hull girder** → no large hatch openings.
- **Smaller hatchways**: Only for inspection → minimal stress concentration.
- **Double bottom + double sides** (post-MARPOL): Redundant protection, improved torsional rigidity.
- **Uniform cargo density**: Liquid cargo distributes evenly → predictable shear/bending.

#### Bulk Carrier Disadvantages:
- **Large hatch openings** (for grab/crane access) → **reduce deck section modulus by 30–40%**.
- **Stress concentrations** at hatch corners → fatigue cracks.
- **Variable cargo density**: Ore vs. grain → unpredictable loading, risk of **hold flooding**.
- **Single-skin construction** (pre-2000s): Vulnerable to corrosion, grounding.

```
Tanker Hull:          Bulk Carrier Hull:
┌──────────────┐      ┌──────────────────┐
│  Small Hatches│      │  LARGE HATCHES   │ ← Weakens deck
├──────────────┤      ├──────────────────┤
│  Integral Tanks│      │  Topside/Hopper  │ ← Stress risers
└──────────────┘      └──────────────────┘
```

***

### 2. Freeboard Assignment: Why Tankers Get Less Freeboard

#### ILLC (International Load Line Convention) Objectives:
1. **Reserve buoyancy** for wave immersion
2. **Limit deck edge immersion** angle
3. **Ensure watertight integrity** of openings
4. **Account for hull form** (sheer, camber)
5. **Consider cargo type** (permeability, shift risk)
6. **Structural strength** (hull girder, hatch covers)
7. **Survivability after damage**

#### Tanker vs. Bulk Carrier Freeboard:

| Factor | Tanker | Bulk Carrier | Effect on Freeboard |
|--------|--------|--------------|---------------------|
| **Hatch Size** | Small (inspection only) | Very large (cargo access) | Bulk carrier needs **more freeboard** to prevent wave ingress |
| **Cargo Permeability** | ~95% (liquid) | 60–90% (solid, air gaps) | Tanker floods uniformly; bulk carrier risks **free surface + shift** |
| **Hull Strength** | Continuous deck | Hatch corners weaken deck | Bulk carrier requires **higher freeboard** to reduce bending |
| **Damage Stability** | Double hull compartments | Single hold flooding → progressive | Tanker survives 1-compartment damage better |

**Result**: For same L, B, D → **tanker assigned 0.5–1.5 m less freeboard** than bulk carrier.

***

### 3. Pump Room Double Bottom: Survivability Enhancement

#### Regulatory Requirement (SOLAS II-1/12):
- Cargo pumps in tankers must be in **pump rooms with double bottom height ≥ 0.76 m** (or equivalent protection).

#### Safety Benefits:
1. **Grounding protection**: Double bottom absorbs impact → prevents cargo tank rupture.
2. **Flooding isolation**: Pump room flooding ≠ cargo tank flooding → limits free surface effect.
3. **Fire safety**: Pump room is **gas-tight**, separate from engine room → reduces explosion risk.

```
Tanker Midship Section:
┌─────────────────────┐
│  Cargo Tanks        │
├─────────────────────┤
│  Pump Room (Double Bottom)│ ← 0.76m+ protection
├─────────────────────┤
│  Engine Room        │
└─────────────────────┘
```

Without this, grounding could flood pump room + adjacent cargo tanks → **loss of stability + fire hazard**.

***

### 4. Corrosion in Tankers: Problems & Regulatory Solutions

#### Corrosion Mechanisms:
- **Cargo tank coating breakdown** → seawater + oil residue → accelerated wastage.
- **Ballast tank corrosion**: Poor coating, inadequate cathodic protection.
- **Stress corrosion cracking**: High-tensile steel + residual stress + seawater.

#### Notable Losses:
1. **MV Sea Star (1997)**: ULCC, structural failure due to **corroded deck plating** → broke in two.
2. **MV Erika (1999)**: Single-hull tanker, **corroded bottom plating** → grounding → spill.
3. **MV Prestige (2002)**: Age + corrosion → hull fracture in storm.

#### Regulatory Solutions:
- **MARPOL Annex I, Reg. 13**: Mandatory **double hulls** for tankers >5,000 DWT (phased out single hull by 2010).
- **IACS CSR (Common Structural Rules)**: Enhanced corrosion margins, coating standards.
- **ESP (Enhanced Survey Programme)**: Annual thickness measurements for tankers >10 years.

***

### 5. Bulk Carrier Design: Topside & Hopper Tanks

#### Why Included?
1. **Strength**: Triangular structure → resists **racking** (transverse distortion).
2. **Stability**: Lowers VCG (vertical center of gravity) → improves GM.
3. **Flooding control**: Limits cargo shift + free surface in hold flooding.
4. **Ballast management**: Dedicated tanks for trim/draft control.

```
Bulk Carrier Hold:
     Topside Tank
    /¯¯¯¯¯¯¯¯¯¯¯¯\
   │              │
   │   CARGO      │
   │              │
    \____________/
     Hopper Tank
```

**Safety Impact**: After flooding of one hold, topside/hopper tanks prevent **progressive flooding** to adjacent holds → survivability.

***

### 6. Granular Sulphur Ban (Post-Arcadia, 1998)

#### Incident:
- **MV Arcadia**: Bulk carrier, granular sulphur cargo → shifted like grain → **angle of loll** → capsized near Mumbai.

#### Why Banned?
- **Twindex behavior**: Sulphur fines fluidize under vibration → acts like **Bingham plastic** (solid at rest, liquid when disturbed).
- **Angle of repose**: ~35° → exceeds safe heel angle for many bulk carriers.
- **IMO MSC/Circ. 664**: Prohibited carriage unless **treated as grain** (shifting boards, trimming).

**Lesson**: Cargo classification must account for **dynamic behavior**, not just static density.

***

### 7. Single-Skin Bulk Carrier Sinking Scenario

#### Typical Failure Sequence:
1. **Hatch cover failure** (corrosion + overpressure) → seawater ingress.
2. **Hold flooding** → free surface effect → GM reduces.
3. **Bulkhead collapse** (designed for cargo, not water pressure) → progressive flooding.
4. **Loss of longitudinal strength** → hull girder fails → rapid sinking.

```
Progressive Flooding:
Hold 1 → Bulkhead → Hold 2 → Bulkhead → Hold 3
  ↓        ↓         ↓        ↓         ↓
Flooded  Failed    Flooded  Failed    Flooded → Sinking
```

**Survivability Issue**: Single-skin bulk carriers cannot survive **two adjacent holds flooded**.

***

### 8. IMO/IACS Formal Safety Assessment (1995–2000)

#### Main Failures Identified:
1. **Design**: Hatch covers under-designed for wave loads.
2. **Construction**: Poor welding, corrosion allowances insufficient.
3. **Operation**: Overloading, improper ballasting, delayed maintenance.
4. **Survey**: Inadequate thickness measurements.

#### Solutions:

| Regulatory (IMO) | Industry (IACS) |
|------------------|-----------------|
| **SOLAS XII**: Strengthened hatch covers, double sides for new bulk carriers >150m | **CSR Bulk Carriers**: Enhanced scantlings, fatigue analysis |
| **ISM Code**: Mandatory safety management | **ESP**: Annual surveys for bulk carriers >10 years |
| **Load Line Amendments**: Bow height, hatch coaming height | **UR Z10**: Corrosion margin increases |

**Result**: Bulk carrier losses dropped **>70%** post-2005.

***

### 9. Numerical: Hatch Cover Design Load (LLC 2005)

Given:
- Ship length \( L = 300 \, \text{m} \)
- Hatch cover at forepeak (0% L) and 15% L from FP
- Stiffener spacing \( s = 700 \, \text{mm} \)

#### Wave Load Formula (IACS UR S21):
\[
P = f \cdot k_s \cdot (H_w + 0.5 \cdot v^2)
\]
Simplified for forepeak:
\[
P_{fore} = 1.5 \cdot P_{mid} \quad \text{(due to slamming)}
\]

Assume design wave height \( H_w = 12 \, \text{m} \) (North Atlantic):
\[
P_{mid} = \rho g H_w = 1025 \times 9.81 \times 12 \approx 120.6 \, \text{kPa}
\]
\[
P_{fore} = 1.5 \times 120.6 \approx 181 \, \text{kPa}
\]

At 15% L:
\[
P_{15\%} \approx 1.2 \times P_{mid} \approx 145 \, \text{kPa}
\]

#### Minimum Plating Thickness:
\[
t = \frac{s \cdot \sqrt{P}}{k \cdot \sigma_{allow}}
\]
Assume \( \sigma_{allow} = 235 \, \text{MPa} \), \( k = 0.9 \):
\[
t = \frac{700 \cdot \sqrt{181}}{0.9 \cdot 235} \approx \frac{700 \cdot 13.45}{211.5} \approx 44.5 \, \text{mm}
\]

**Note**: Actual design uses **stiffened panels** → thickness ~20–30 mm with stiffeners.

***

### 10. Kinetic & Potential Energy of Waves on Hatches (Type B Ships)

#### Type B Ships:
- Dry cargo ships with **large hatch openings** → reduced deck strength.

#### Wave Energy Effects:
1. **Potential Energy**: Wave elevation → hydrostatic pressure on hatch cover.
2. **Kinetic Energy**: Wave impact (slamming) → dynamic pressure spike.

```
Wave Impact on Hatch:
      Crest
        *
       /|\
      / | \  → Kinetic (impact)
     /  |  \
----*---|---*---- Hatch Cover
        |
        ↓
    Potential (static)
```

**Design Implication**: Hatch covers must withstand **both static + dynamic loads** → LLC 2005 increased requirements.

***


## Part 5: ROPAX Stability & SOLAS 90/90+50 Standards

### 1. Case Studies: Al Salaam & Boccaccio 98

#### MV Al Salaam (2006, Red Sea)
- **Loss**: 950+ lives
- **Cause**: Fire in vehicle deck → water accumulation from firefighting → **free surface effect** → capsized.
- **Stability Failure**:
  - **Firefighting water** not pumped out → GM reduced to negative.
  - **Passengers ran to one side** → heeling moment exceeded righting moment.
  - **No damage stability compliance** (pre-SOLAS 90).

#### MV Boccaccio 98 (1992, Baltic Sea)
- **Loss**: 140+ lives
- **Cause**: Bow door failure → seawater ingress on vehicle deck → **free surface + free communication** → capsized in 30 min.
- **Stability Failure**:
  - **Large undivided vehicle deck** → water spread across beam.
  - **Insufficient reserve buoyancy** → rapid downflooding.

**Common Factor**: Both lacked **SOLAS 90 damage stability** → could not survive one-compartment flooding.

***

### 2. SOLAS 90 Standard for ROPAX Ships

#### Definition:
SOLAS 90 (1990 amendments) requires ROPAX ships to survive **flooding of any one compartment** with:
- **Residual GM ≥ 0.05 m**
- **Righting lever GZ ≥ 0.1 m** over 30° range
- **Equilibrium heel ≤ 15°**

#### Key Requirements:
1. **Subdivision**: Vehicle decks divided by **watertight bulkheads**.
2. **Damage stability calculations**: Probabilistic method (not deterministic).
3. **Free surface correction**: Account for water accumulation on car decks.

**Impact**: Pre-1990 ROPAX ships **failed** this standard → required retrofits or phase-out.

***

### 3. SOLAS 90+50 (Stockholm Agreement, 1996)

#### Background:
After **Estonia disaster (1994)**, IMO adopted **Stockholm Agreement** (1996), enhancing SOLAS 90.

#### Key Provisions:
- **Additional 50 cm freeboard** (hence “+50”) for ROPAX ships.
- **Higher damage stability**: Survive flooding with **50 cm water on vehicle deck**.
- **Mandatory bow door locks** + CCTV monitoring.
- **Phased compliance**: Existing ships to comply by 2010.

#### A and Amax Parameters:
- **A**: Actual **subdivision index** (probability of surviving damage).
- **Amax**: Minimum required index (function of ship length, N passengers).

**Compliance Rule**:
\[
A \geq A_{max} = 1 - \frac{1000}{L_s + N + 1500}
\]
Where \( L_s \) = subdivision length, \( N \) = passenger capacity.

**Effect**: Larger ships with more passengers → **higher Amax** → stricter subdivision.

***

### 4. Stability Failures in Al Salaam/Boccaccio 98 (with Diagrams)

#### (a) Firefighting Operations (Al Salaam)
```
Vehicle Deck:
┌─────────────────────┐
│  Fire → Water Spray │ ← Accumulates on deck
│  ~500 tons water    │
└─────────────────────┘
Effect: Free surface → GM ↓ → Negative → Capsize
```

**Lesson**: ROPAX must have **scuppers + pumps** to remove firefighting water immediately.

#### (b) Passengers Running to One Side
```
Passenger Movement:
   Left Side: 200 pax → Right Side: 800 pax
         ↓                  ↑
   Heeling Moment = 600 pax × 10m (beam) ≈ 6,000 ton-m
   Righting Moment < 6,000 → Capsize
```

**Lesson**: **Crowd control** + **stability margins** for heeling moments.

#### (c) Vessel Making Wide Turn at Speed
```
Turning Maneuver:
   Centrifugal Force = (Δ × V²) / R
   Heeling Angle ≈ 10–15° at 20 knots
   + Water on deck → GM ↓ → Capsize risk
```

**Lesson**: **Speed restrictions** in adverse weather + **anti-rolling systems**.

***

### 5. Structural Alterations for SOLAS 90/90+50 Compliance

#### Retrofit Options for Existing ROPAX:

| Modification | Purpose | Sketch |
|--------------|---------|--------|
| **Watertight bulkheads** on vehicle deck | Limit flooding to one compartment | `├───┼───┼───┤` (divided deck) |
| **Raised coamings** around stairwells | Prevent downflooding | `____` (higher edges) |
| **Additional buoyancy boxes** | Increase reserve buoyancy | `┌─┐` (side sponsons) |
| **Bow door reinforcement** | Prevent sea ingress | Double locks + CCTV |

**Sketch: Watertight Subdivision**:

```
Pre-SOLAS 90:      Post-SOLAS 90:
┌──────────────┐   ┌───┼───┼───┐
│ Undivided    │   │ W │ W │ W │ ← Watertight bulkheads
│ Vehicle Deck │   │ T │ T │ T │
└──────────────┘   └───┴───┴───┘
```

**Sketch: Buoyancy Boxes**:

```
Original:        Retrofitted:
┌──────┐        ┌──┬──┬──┐
│ Ship │        │S │S │S │ ← Sponsons (buoyancy)
└──────┘        └──┴──┴──┘
```

***

### 6. Ro-Ro Ship Fire Safety: SOLAS Definitions

#### SOLAS Definitions:
- **Ro-Ro Space**: Space intended for cargo vehicles with fuel in tanks (SOLAS II-2/3).
- **Special Category Space**: Enclosed Ro-Ro space extending >25% of ship length (SOLAS II-2/3.14).

#### Fire Safety Measures:
1. **Fixed foam/water spray systems** (mandatory for special category spaces).
2. **Smoke extraction**: 10 air changes/hour.
3. **Fire detection**: Heat/smoke sensors every 50 m².
4. **Separation**: Engine rooms, accommodation separated by **A-60 bulkheads**.

**Goal**: Prevent fire spread + maintain stability during firefighting.

***

### 7. Numerical: A/Amax Compliance Example

**Given**:
- ROPAX ship: \( L_s = 150 \, \text{m} \), \( N = 1000 \) passengers

**Calculate Amax**:
\[
A_{max} = 1 - \frac{1000}{150 + 1000 + 1500} = 1 - \frac{1000}{2650} \approx 0.623
\]

**Required**: Subdivision index \( A \geq 0.623 \)

**If actual A = 0.58** → **Non-compliant** → must add bulkheads or buoyancy.

***

### 8. Comparison: Pre-SOLAS 90 vs. SOLAS 90+50 ROPAX

| Parameter | Pre-SOLAS 90 | SOLAS 90 | SOLAS 90+50 |
|-----------|--------------|----------|-------------|
| **Damage survival** | 1 compartment (deterministic) | 1 compartment (probabilistic) | 1 compartment + 50cm water |
| **Freeboard** | Standard | Standard | +50 cm |
| **Bow doors** | Basic locks | Enhanced locks | Double locks + CCTV |
| **Vehicle deck subdivision** | Minimal | Watertight bulkheads | Bulkheads + scuppers |
| **Loss rate (per 1000 ship-years)** | ~2.5 (1980s) | ~0.8 (1990s) | ~0.2 (2000s) |

***


## Part 6: Stability Formulas & Numericals

### 1. Wall-Sided Formula (Large Angle Heel)

#### Derivation:
For a **wall-sided vessel** (vertical sides at waterline), the righting lever \( GZ \) at large heel \( \theta \) is:

\[
GZ = \sin\theta \left( GM + \frac{1}{2} BM \tan^2\theta \right)
\]

**Assumptions**:
- Hull sides are **vertical** near waterline (valid for box barges, some tankers).
- Waterplane area remains **constant** with heel.
- Valid up to **θ ≈ 25°** (before deck edge immersion).

#### Diagram:

```
Heeled Wall-Sided Hull:
       Original WL
         ____
        /    \
       /      \   Heeled WL
      /        \ /
     /__________\
    B → B₁ (shifts outward)
    G fixed
    GZ = GM·sinθ + ½·BM·sinθ·tan²θ
```

**Why “Wall-Sided”?**  
Because the formula assumes the hull behaves like a **vertical-walled box** → waterplane breadth unchanged with heel.

***

### 2. Atwood’s Formula (General Large Angle)

For **any hull form** (not just wall-sided):

\[
GZ = \frac{v \cdot h}{V} - BG \cdot \sin\theta
\]

Where:
- \( v \): Volume of wedge immersed (or emerged)
- \( h \): Horizontal shift of wedge centroid
- \( V \): Total displacement volume
- \( BG \): Distance between B and G

**Derivation Insight**:
- Accounts for **actual hull geometry** (not just vertical sides).
- More accurate than wall-sided for **flared or tumblehome hulls**.

***

### 3. Limitations of \( GZ = GM \sin\theta \)

#### Validity Range:
- **θ < 6°**: Accurate (small-angle approximation).
- **θ > 6°**: **Underestimates GZ** for wall-sided ships, **overestimates** for flared hulls.

#### Why?
- \( GM \) is **initial metacentric height** (at θ = 0°).
- At large angles, **M moves** (prometacentre concept) → GM is no longer constant.

#### Comparison:

| Formula | Valid Range | Accuracy | Use Case |
|---------|-------------|----------|----------|
| \( GZ = GM \sin\theta \) | θ < 6° | High (small angles) | Initial stability checks |
| Wall-sided | θ ≤ 25° | Moderate (vertical sides) | Box barges, tankers |
| Atwood’s | θ ≤ 90° | High (any hull) | Damage stability, GZ curves |

***

### 4. Prometacentre (M_θ)

#### Definition:
The **prometacentre** \( M_\theta \) is the **instantaneous metacentre** at heel angle \( \theta \). Unlike M (at θ = 0°), \( M_\theta \) **moves** as the hull heels.

#### Diagram:

```
Upright:          Heeled (θ):
   M₀                M_θ
   |                 /
   |                /
   B₀              B_θ
   |               |
   G               G
GM₀ = M₀B₀ - BG   GM_θ = M_θB_θ - BG (varies with θ)
```

**Why Calculate Restoring Moments at Large Angles?**
- **GM₀ is irrelevant** beyond 6°.
- **GZ curve** (from Atwood’s or hydrostatics) determines **dynamic stability** (area under curve).
- **Angle of vanishing stability** (GZ = 0) → capsize risk.

***

### 5. Angle of Loll (Unstable Equilibrium)

#### Definition:
An **angle of loll** occurs when:
- **GM < 0** (unstable upright)
- Ship finds **stable equilibrium** at heel angle \( \theta_{loll} \) where \( GZ = 0 \) again.

#### Formula (Wall-Sided):
\[
\tan\theta_{loll} = \pm \sqrt{\frac{-2 \cdot GM}{BM}}
\]

**Example (Derrett’s Q9a)**:
Given: \( GM = -0.3 \, \text{m} \), \( BM = 4.8 \, \text{m} \)

\[
\tan\theta_{loll} = \sqrt{\frac{-2 \times (-0.3)}{4.8}} = \sqrt{\frac{0.6}{4.8}} = \sqrt{0.125} \approx 0.354
\]
\[
\theta_{loll} = \tan^{-1}(0.354) \approx 19.5^\circ
\]

**Danger**: Ship may **loll suddenly** to 20° → cargo shift → capsize.

***

### 6. Derrett’s Numerical: Example 2 (Page 140)

**Problem**: Box-shaped barge, L = 60m, B = 10m, D = 5m, draft = 3m, KG = 4m. Find GZ at 20° heel.

#### Step 1: Calculate KB, BM, GM
- \( KB = \frac{T}{2} = 1.5 \, \text{m} \)
- \( BM = \frac{B^2}{12T} = \frac{10^2}{12 \times 3} = \frac{100}{36} \approx 2.78 \, \text{m} \)
- \( KM = KB + BM = 1.5 + 2.78 = 4.28 \, \text{m} \)
- \( GM = KM - KG = 4.28 - 4.0 = 0.28 \, \text{m} \)

#### Step 2: Wall-Sided GZ at 20°
\[
GZ = \sin 20^\circ \left( 0.28 + \frac{1}{2} \times 2.78 \times \tan^2 20^\circ \right)
\]
\[
\sin 20^\circ = 0.342, \quad \tan 20^\circ = 0.364, \quad \tan^2 20^\circ = 0.133
\]
\[
GZ = 0.342 \left( 0.28 + 1.39 \times 0.133 \right) = 0.342 \left( 0.28 + 0.185 \right) \approx 0.342 \times 0.465 \approx 0.159 \, \text{m}
\]

**Compare with \( GM \sin\theta \)**:
\[
GZ_{small} = 0.28 \times 0.342 \approx 0.096  \text{m} \quad (underestimates by 40%)
\]

***

### 7. Derrett’s Q9b: Box-Shaped Barge Angle of Loll

**Given**: L = 50m, B = 8m, draft = 4m, KG = 5m, KB = 2m, BM = 1.33m.

#### Step 1: Calculate GM
- \( KM = KB + BM = 2 + 1.33 = 3.33 \, \text{m} \)
- \( GM = KM - KG = 3.33 - 5.0 = -1.67 \, \text{m} \) (unstable)

#### Step 2: Angle of Loll
\[
\tan\theta_{loll} = \sqrt{\frac{-2 \times (-1.67)}{1.33}} = \sqrt{\frac{3.34}{1.33}} = \sqrt{2.51} \approx 1.585
\]
\[
\theta_{loll} = \tan^{-1}(1.585) \approx 57.8^\circ
\]

**Interpretation**: Ship will loll to **~58°** → likely capsize if cargo shifts.

***

### 8. GZ Curve & Dynamic Stability

#### GZ Curve Components:
1. **Initial slope**: \( \frac{dGZ}{d\theta} = GM \) at θ = 0°.
2. **Maximum GZ**: At θ ≈ 30–40° (varies by hull).
3. **Angle of vanishing stability**: GZ = 0 → capsize threshold.
4. **Area under curve**: **Dynamic stability** (energy to capsize).

#### Diagram:

```
GZ (m)
  |
  |     Max GZ
  |      *
  |     / \
  |    /   \
  |   /     \
  |  /       \
  | /         \
  |/___________\______ θ (°)
  0   30   60   90
       Angle of Vanishing Stability
```

**Regulatory Minimums** (IMO A.749):
- **Area under GZ curve** ≥ 0.055 m·rad (up to 30°)
- **Max GZ** ≥ 0.20 m at θ ≥ 25°

***

### 9. Rolling Period & GM Relationship

From earlier:
\[
T_\phi = 2\pi \sqrt{\frac{k^2}{g \cdot GM}}
\]

**Rearranged for GM**:
\[
GM = \frac{4\pi^2 k^2}{g T_\phi^2}
\]

**Rolling Test Procedure**:
1. Displace ship slightly (tug push).
2. Measure **time for 5 complete rolls** → average \( T_\phi \).
3. Assume \( k \approx 0.4B \) → calculate GM.

**Example**:
- \( B = 20 \, \text{m} \), \( T_\phi = 12 \, \text{s} \), \( k = 0.4 \times 20 = 8 \, \text{m} \)
\[
GM = \frac{4\pi^2 \times 8^2}{9.81 \times 12^2} = \frac{4 \times 9.87 \times 64}{9.81 \times 144} \approx \frac{2527}{1413} \approx 1.79 \, \text{m}
\]

***

### 10. Summary Table: Stability Formulas

| Formula | Expression | Valid Range | Use Case |
|---------|------------|-------------|----------|
| Small-angle | \( GZ = GM \sin\theta \) | θ < 6° | Initial stability |
| Wall-sided | \( GZ = \sin\theta (GM + \frac{1}{2} BM \tan^2\theta) \) | θ ≤ 25° | Box barges, tankers |
| Atwood’s | \( GZ = \frac{v \cdot h}{V} - BG \sin\theta \) | θ ≤ 90° | Any hull, damage stability |
| Angle of loll | \( \tan\theta_{loll} = \pm \sqrt{\frac{-2GM}{BM}} \) | GM < 0 | Unstable ships |
| Rolling period | \( T_\phi = 2\pi \sqrt{\frac{k^2}{g \cdot GM}} \) | Small angles | GM estimation from roll test |

***


## Part 7: High-Speed Craft & Hydrofoils

### 1. SOLAS Definition of High-Speed Craft

#### SOLAS Chapter X (High-Speed Craft):
A **High-Speed Craft** is defined as (SOLAS Reg. X/1.2):

> “A craft capable of a maximum speed in metres per second (m/s) satisfying:
> \[
> V \geq 3.7 \cdot \nabla^{0.1667}
> \]
> where \( \nabla \) = volume of displacement at design waterline (m³).”

**Simplified**: For most vessels, this translates to:
- **≥ 25 knots** for displacement hulls
- **≥ 35 knots** for planing/semi-planing hulls

#### HSC Code (IMO Resolution A.373):
Mandatory for all HSC engaged on **international voyages**:
- **Construction**: Lightweight materials (aluminum, composites).
- **Stability**: Enhanced damage stability (flooding of one compartment).
- **Fire safety**: Automatic sprinklers, smoke extraction.
- **Navigation**: Redundant systems, weather restrictions.

***

### 2. Hydrofoils: How High Speed is Achieved

#### Principle:
Hydrofoils lift the **hull out of water** at speed → **dramatically reduces drag**.

**Drag Components**:
- **Frictional drag** (hull wetted surface) → eliminated when hull clears water.
- **Wave-making drag** (hull pushing water) → minimized.
- **Foil drag** (small submerged foils) → much lower than full hull drag.

#### Speed Regimes:

| Mode | Speed | Hull Position | Drag |
|------|-------|---------------|------|
| **Displacement** | < 15 knots | Fully in water | High (friction + wave) |
| **Transition** | 15–25 knots | Partially lifted | Moderate |
| **Foil-borne** | > 25 knots | Hull clear of water | Low (foils only) |

**Power Requirement**:
\[
P \propto D \cdot V
\]
Where \( D \) = drag. By reducing \( D \) by 70–80% (foil-borne), speed increases **2–3×** for same power.

#### Diagram:

```
Displacement Mode:     Foil-Borne Mode:
   ____                  ____
  /    \                /    \
 /______\  ← Hull      /______\  ← Hull (clear of water)
 ~~~~~~~~  Water          ||||
                          ||||  ← Foils submerged
```

***

### 3. Transverse & Longitudinal Stability (Hydrofoils)

#### Transverse Stability (Roll):
- **Foil-borne**: Stability from **dihedral angle** of foils (like airplane wings).
  - Heel → lower foil generates more lift → righting moment.
- **Hull-borne**: Conventional waterplane stability (GM-based).

**Key Parameter**: **Dihedral angle** \( \gamma \):
\[
RM_{roll} \approx L_{foil} \cdot \sin\gamma \cdot \Delta V
\]
Where \( L_{foil} \) = foil span, \( \Delta V \) = lift change.

#### Longitudinal Stability (Pitch):
- **Canard configuration** (forward foil + aft foil):
  - Forward foil: Controls pitch, provides lift.
  - Aft foil: Stabilizes, trims.
- **Automatic control systems**: Adjust foil angles to maintain level flight.

**Diagram**:

```
Side View (Canard Hydrofoil):
      Forward Foil (adjustable)
           /
          /
         /
        /___________ Hull (clear)
                 \
                  \
                   \ Aft Foil (stabilizer)
```

**Risk**: **Pitch-poling** (bow dives) if forward foil stalls → automated systems prevent this.

***

### 4. Seakeeping (Hydrofoils)

#### Advantages:
- **Hull clear of waves** → minimal motion sickness.
- **Active foil control** → adjusts to wave slope → smooth ride.

#### Limitations:
- **Foil ventilation** (air drawn into foil) → loss of lift → sudden drop.
- **Wave height limit**: Typically **Hs ≤ 2.5 m** for safe foil-borne operation.
- **Speed restrictions**: Reduce to hull-borne in rough seas.

#### Comparison with Monohull:

| Parameter | Monohull | Hydrofoil |
|-----------|----------|-----------|
| **Roll motion** | Large (GM-dependent) | Small (foil-controlled) |
| **Pitch motion** | Moderate | Minimal (active control) |
| **Comfort (MSI)** | Poor in waves | Excellent (hull clear) |
| **Operational limit** | Hs ≤ 4–5 m | Hs ≤ 2.5 m (foil-borne) |

***

### 5. Propulsion Arrangement (Hydrofoils)

#### Common Systems:
1. **Waterjets** (most common):
   - High efficiency at 30–50 knots.
   - No exposed propellers → safe for passengers.
2. **Surface-piercing propellers**:
   - Reduced drag (partially out of water).
   - Risk: Ventilation, cavitation.
3. **Gas turbines** (military hydrofoils):
   - High power-to-weight ratio.
   - Fuel consumption: Very high.

#### Diagram:

```
Hydrofoil Propulsion:
   Hull (clear)
      ||
      ||  ← Struts (house driveshafts)
      ||
   Foils + Waterjets (submerged)
```

**Advantage**: Waterjets allow **rapid reversal** → excellent maneuverability.

***

### 6. HSC Code: Key Safety Requirements

#### Structural:
- **Lightweight materials**: Aluminum alloys (5083, 6061), carbon fiber composites.
- **Collision protection**: Double bottom, watertight compartments.

#### Stability:
- **Damage stability**: Survive flooding of **one compartment** (similar to SOLAS 90).
- **Intact stability**: GM ≥ 0.15 m (hull-borne), positive righting energy (foil-borne).

#### Fire Safety:
- **Automatic sprinklers** in passenger spaces.
- **Smoke extraction**: 20 air changes/hour.
- **Fire-resistant bulkheads**: A-60 class.

#### Operational Restrictions:
- **Weather limits**: Hs ≤ 2.5 m (typical).
- **Speed limits**: Reduce in restricted visibility.
- **Mandatory reporting**: Position, weather, passenger count.

***

### 7. Comparison: Monohull vs. Multihull vs. Hydrofoil

| Aspect | Monohull | Multihull (Catamaran) | Hydrofoil |
|--------|----------|----------------------|-----------|
| **Speed** | 15–25 knots | 25–35 knots | 35–50 knots |
| **Stability (intact)** | GM-based (moderate) | Wide beam → high GM | Foil-controlled (active) |
| **Drag** | High (friction + wave) | Moderate (two narrow hulls) | Low (hull clear) |
| **Seakeeping** | Poor (large rolls) | Better (less roll) | Best (hull clear) |
| **Power/Speed Ratio** | 1.0 (baseline) | 0.7 (30% less power) | 0.4 (60% less power) |
| **Cost** | Low | Moderate | High (complex foils) |

**Power/Speed Ratio**:
\[
\text{Ratio} = \frac{P}{V^3}
\]
Hydrofoils achieve **2–3× speed** for same power → ideal for fast ferries.

***

### 8. Numerical: HSC Speed Threshold

**Given**: HSC with displacement volume \( \nabla = 500 \, \text{m}^3 \)

**Calculate minimum speed for HSC classification**:
\[
V_{min} = 3.7 \cdot \nabla^{0.1667} = 3.7 \cdot 500^{0.1667}
\]
\[
500^{0.1667} = e^{0.1667 \cdot \ln 500} = e^{0.1667 \cdot 6.215} = e^{1.036} \approx 2.82
\]
\[
V_{min} = 3.7 \times 2.82 \approx 10.4 \, \text{m/s} \approx 20.2 \, \text{knots}
\]

**Interpretation**: This vessel must exceed **20.2 knots** to be classified as HSC → likely a **planing hull** or **hydrofoil**.

***

### 9. HSC Operational Challenges

1. **Weather sensitivity**: Must reduce speed/stop in Hs > 2.5 m.
2. **Foil strike risk**: Submerged foils can hit debris → inspection mandatory.
3. **Passenger comfort**: Sudden transitions (hull-borne ↔ foil-borne) → motion sickness.
4. **Regulatory compliance**: HSC Code requires **annual surveys**, **crew training**.

***


