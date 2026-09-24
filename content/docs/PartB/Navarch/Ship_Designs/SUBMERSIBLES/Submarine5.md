---
title: "Short Notes"
type: docs
---
# Q.7 — Short Notes: 
## (a) Manoeuvring of a Submarine, 
## (b) Trim Control During Torpedo Operations, 
## (c) Collapse Depth and Time Available to Collapse Depth (Numerical)

## (a) Manoeuvring of a Submarine

A submarine's manoeuvring is fundamentally three-dimensional (unlike a surface ship's essentially two-dimensional manoeuvring in the horizontal plane alone), since it must control motion in **pitch, roll, and yaw simultaneously**, and depth-keeping is itself an active manoeuvring task rather than a passive, automatically-maintained condition.

**Control surfaces and their functions:**
1. **Rudder** — mounted aft, controls **yaw (turning in the horizontal plane)**, functioning essentially as on a surface ship, deflecting flow to generate a turning moment about the vertical axis.
2. **Hydroplanes** — the primary depth/pitch control surfaces, generating lift (up or down) as they are angled, requiring **forward speed (way on)** to be effective, since they rely on flow over an aerofoil-type surface exactly as an aircraft's control surfaces do:
 - **Fore-planes (bow planes)** — located forward, used primarily for **fine, rapid depth-keeping and initial angle of dive/rise**, and are often rigged in (retracted) when surfaced or alongside to avoid damage, deployed only when submerged/diving.
 - **After-planes (stern planes)** — located aft, near the rudder, used primarily to control **pitch angle (fore-and-aft inclination of the hull)**, working in conjunction with fore-planes for coordinated depth-changes.
3. **Combined plane action**: To change depth while maintaining a level (non-pitched) hull attitude, fore-planes and after-planes are used in a coordinated, sometimes opposing sense (e.g., bow planes angled to dive while stern planes are angled to counteract excessive bow-down pitch), whereas to change depth via a deliberate pitch angle (common at low speed or in some designs without separate bow planes), the planes work in a complementary sense to incline the entire hull.

**Speed and depth interaction:**
- At **higher speed**, hydroplanes are highly effective, and only small angles are needed for a given rate of depth change — this is the primary and most controllable means of managing depth while making way.
- At **very low speed or zero speed**, hydroplanes lose effectiveness (insufficient flow for lift generation), and **depth/attitude control must revert to the ballast tank system** (auxiliary/trim tanks, and negative tank for rapid changes) as discussed in Q.2 and Q.3 — this is an important operational limitation, since a submarine "hovering" at very low speed is much harder to control precisely in depth than one making way with plane authority.

**Horizontal manoeuvring (turning):**
- The **rudder** generates a turning moment as on a surface ship, but a submerged submarine additionally experiences **heel (roll) during a turn**, analogous to an aircraft banking, because the hydrodynamic side force and the vessel's own centrifugal tendency interact with the submarine's transverse stability characteristics (BG, as discussed in Q.5) differently than a surface ship's turn-induced heel — a submarine may heel inward or outward during a turn depending on speed, rudder angle, and hull form, and this coupled roll-yaw-pitch interaction must be managed by the coordinated use of rudder and planes, particularly at higher speeds and larger rudder angles.
- Because the submarine is a **fully three-dimensional body with roll, pitch, and yaw all dynamically coupled** (unlike a surface ship where roll is largely decoupled from ordinary turning manoeuvres), submarine manoeuvring at speed requires continuous, coordinated control of rudder and both sets of hydroplanes to maintain the ordered depth, trim, and heading simultaneously — this is typically managed today through integrated ship control systems that coordinate all control surfaces automatically to an ordered depth/course, though manual "hands-on" planesman/helmsman control remains a fundamental watchkeeping skill.

## (b) Trim Control During Torpedo Operations

Firing a torpedo represents a **sudden, discrete weight loss** from the submarine (a torpedo of substantial mass leaving the tube instantaneously), which, if uncompensated, would cause an abrupt change in the vessel's overall buoyancy/weight balance and, because torpedo tubes are located forward (in the bow), a **significant disturbance to fore-and-aft trim** (a sudden tendency to become bow-light/stern-heavy, causing the bow to rise) — precisely the "sudden trim change" concern referenced in Q.8.

**Compensating measures — Water Round Torpedo (WRT) tanks:**
- Submarines are fitted with a **WRT (Water Round Torpedo) tank** system associated with each torpedo tube, specifically designed to **automatically or manually admit an equivalent weight of seawater into the tube/WRT tank at the instant of firing**, replacing the weight of the departed torpedo essentially simultaneously with its departure.
- This is typically achieved by the **torpedo tube firing/flooding sequence itself**: as the torpedo is ejected (by impulse water or air ram), seawater floods in behind it to fill the vacated volume in the tube, and this water mass is drawn from/accounted via the WRT tank system, so that the **net weight of the submarine remains essentially unchanged** at the moment of firing, rather than suddenly becoming lighter forward.
- Without this compensation, the sudden forward weight loss would cause an **immediate bow-up trim moment and a tendency to rise**, which at shallow/periscope depth could risk **broaching (breaking surface unintentionally)** — a serious tactical and safety concern, particularly during a submerged attack when remaining undetected is essential.

**Additional trim management:**
- Beyond the immediate WRT compensation, the **trim tanks and trim pump** (Q.2, Q.3) are used to fine-tune and restore precise fore-aft balance following the firing sequence, since the WRT system compensates weight but the *distribution* of that compensating water (in the WRT tank, near the bow) may not exactly replicate the original torpedo's centre of gravity contribution to the vessel's overall trim — minor residual trim correction via the trim pump is typically still required after a torpedo firing (or salvo of firings) to restore the boat to a fully balanced condition.
- Firing **multiple torpedoes in quick succession (a salvo)** compounds this challenge, requiring rapid, sequential WRT compensation for each tube fired plus ongoing trim monitoring, since cumulative small errors in compensation across a multi-torpedo salvo could produce a more significant net trim disturbance than a single firing.

## (c) Collapse Depth and Time Available to Collapse Depth — Numerical

**Definitions:**
- **Test depth**: The maximum depth to which the submarine is certified/proven to dive routinely in service, incorporating a safety margin below collapse depth.
- **Collapse depth (crush depth)**: The depth at which the external hydrostatic pressure exceeds the pressure hull's structural capacity, causing catastrophic buckling/collapse of the pressure hull — this is a **theoretical/design limit**, not a depth the submarine is ever intended to reach in service, and is typically **1.5 to 2 times the test depth** depending on the navy/design safety factor convention.
- The "**time available to collapse depth**" refers to the time interval between the moment an uncontrolled/emergency descent begins (e.g., following a flooding casualty, loss of hydroplane control, or loss of buoyancy) and the moment the submarine would reach collapse depth if the descent rate continues unchecked — this interval represents the **window available for the crew to take corrective action** (blowing ballast tanks, using the safety tank, correcting planes, etc.) before catastrophic failure.

**Illustrative numerical approach** (the type of calculation typically posed in this specimen question):

Given:
- Depth at which the casualty/uncontrolled descent begins: $D_1$
- Collapse depth: $D_c$
- Rate of descent (sinking rate), $R$ (in metres/second or metres/minute), either given directly or derived from a stated rate of flooding/negative buoyancy and the vessel's response characteristics.

$$\text{Time available} = \frac{D_c - D_1}{R}$$

**Worked example (illustrative figures):**
Suppose a submarine with a collapse depth of 600 m suffers a casualty at an operating depth of 200 m, and begins an uncontrolled descent at a rate of 2 m/s due to loss of buoyancy/planes control.

$$\text{Time available} = \frac{600 - 200}{2} = \frac{400}{2} = 200 \text{ seconds} \approx 3\ \text{minutes } 20\ \text{seconds}$$

**Interpretation and significance:**
- This time interval, though it may appear to allow a few minutes, is in practice **extremely short** given that corrective action requires the crew to first **recognize** the casualty, diagnose its cause, and then execute the correct emergency procedure (e.g., blowing all main ballast tanks with emergency HP air, hard-rise on all hydroplanes, and possibly an emergency full-astern/full-ahead order depending on doctrine) — the numerical "time available" figure is intended to emphasize **why submarine emergency drills place such heavy emphasis on immediate, near-instinctive crew reaction** rather than a considered, deliberative response, since the margin for delay is measured in seconds to a few minutes, not a leisurely timeframe.
- The calculation also illustrates why **operating depth is kept at a substantial, deliberate margin below test depth (and hence far below collapse depth)** in normal service — the deeper the initial casualty depth (i.e., the closer routine operating depth is to test/collapse depth), the less time is available for corrective action, which is precisely why navies maintain conservative operating-depth-to-test-depth-to-collapse-depth margins as a fundamental safety philosophy, and why any inadvertent excursion beyond normal operating depth is treated as a serious emergency requiring immediate, practiced corrective drill rather than routine handling.

---

