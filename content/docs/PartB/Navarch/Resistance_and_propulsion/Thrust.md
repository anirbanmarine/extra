---
Title: Features of Propellers
type: docs
sidebar:
  open: true

---


**DIAMETER** \( D \)  
The diameter of the propeller is the diameter of the circle or disc cut out by the blade tips. Increasing a propeller’s diameter will generally increase its efficiency, but this will be limited by the draught and form of the aft part of the ship.

**PITCH** \( P \)  
Pitch is defined as the distance the propeller would move forwards in one revolution if it were working in an unyielding fluid. This is similar to how a screw thread progresses into wood as it is turned. In reality, water is not an unyielding fluid, and so the propeller would not progress as far as the pitch.

**PITCH RATIO** \( p \), or face pitch ratio, is the face pitch divided by the diameter. Thus:

\[
p = \frac{P}{D}
\]

**THEORETICAL SPEED** \( V_t \) is the distance the propeller would advance in unit time if working in an unyielding fluid. Thus, if the propeller turns at \( N \) rev/min,

\[
V_t = P \times N \quad \text{(m/min)}
\]

**APPARENT SLIP**  
As described previously, water is not an unyielding fluid, and so the ship speed \( V \) will normally be less than the theoretical speed. The difference between the two speeds is known as the apparent slip and is usually expressed as a ratio or percentage of the theoretical speed.

\[
\text{Apparent slip speed} = V_t - V \quad \text{(knots)}
\]

If the ship speed is measured relative to the surrounding water, i.e. by means of a log line or paddle wheel speedometer, the theoretical speed will invariably exceed the ship speed, giving a positive apparent slip. If however, the ship speed is measured relative to the land, then any movement of water will affect the apparent slip, and should the vessel be travelling in a following current the ship speed may exceed the theoretical speed, resulting in a negative apparent slip.

**WAKE**  
In its passage through the water, the ship sets in motion particles of water in its neighbourhood. This moving water is known as the wake and is important in propeller calculation since the propeller works in wake water. The speed of the ship relative to the wake is termed the speed of advance.

**SPEED OF ADVANCE** \( V_a \)  
The wake speed is often expressed using:

- Taylor’s Wake Factor  
- Froude’s Wake Factor  

The wake fraction may be obtained approximately from the expression

\[
w_t = 0.5 C_b - 0.05
\]

where \( C_b \) is the block coefficient.

**REAL SLIP OR TRUE SLIP** is the difference between the theoretical speed and the speed of advance, expressed as a ratio or percentage of the theoretical speed.

\[
\text{Real slip speed} = V_t - V_a \quad \text{(knots)}
\]

The real slip is always positive and is independent of current.

**EXAMPLE**  
A propeller of \( 4.5 \) m pitch turns at \( 120 \) rev/min and drives the ship at \( 15.5 \) knots. If the wake fraction is \( 0.30 \), calculate the apparent slip and the real slip.

\[
V_t = \frac{4.5 \times 120 \times 60}{1852} = 17.49 \text{ knots}
\]

Apparent slip:

\[
\frac{V_t - V}{V_t} = \frac{17.49 - 15.5}{17.49} = 11.38\%
\]

Wake speed = wake fraction \( \times \) speed of ship:

\[
w_t V = V - V_a
\]

Therefore:

\[
V_a = V(1 - w_t) = 15.5 \times (1 - 0.3) = 15.5 \times 0.7 = 10.85 \text{ knots}
\]

Real slip:

\[
\frac{V_t - V_a}{V_t} = \frac{17.49 - 10.85}{17.49} = 37.96\%
\]

The relation between the different speeds may be shown clearly by a line diagram.

**PROJECTED AREA** \( A_p \) is the sum of the blade areas projected on to a plane that is perpendicular to the axis of the screw.

**DEVELOPED AREA** is the actual area of the driving faces  
- a) Clear of the boss \( A_D \)  
- b) Including the boss area \( A_B \)

**BLADE AREA RATIO** \( \text{BAR} \) is the developed area excluding boss divided by the area of the circle cut out by the blade tips:

\[
\text{BAR} = \frac{A_D}{\frac{\pi}{4} D^2}
\]

**DISC AREA RATIO** \( \text{DAR} \) is the developed area including boss divided by the area of the circle cut out by the blade tips:

\[
\text{DAR} = \frac{A_B}{\frac{\pi}{4} D^2}
\]

**Thrust**  
The thrust exerted by a propeller may be calculated approximately by regarding the propeller as a disc that increases the momentum of the water coming into it. Water is received into the propeller disc at the speed of advance and projected aft at the theoretical speed.

Consider a time interval of 1 second.  
Let  
\( A \) = Effective disc area in \( \mathrm{m}^2 \) = disc area − boss area  
\( \rho \) = density of water in \( \mathrm{kg/m}^3 \)  
\( P \) = pitch of propeller in \( \mathrm{m} \)  
\( N \) = revs/s  
\( V_a \) = speed of advance in \( \mathrm{m/s} \)

Mass of water passing through disc in 1 second:

\[
M = \rho A P N \quad \text{kg}
\]

Change in velocity:

\[
P N - V_a \quad \text{m/s}
\]

Since this change in velocity occurs within 1 second, the acceleration \( a \) is:

\[
a = P N - V_a \quad \text{m/s}^2
\]

But real slip \( s \) is:

\[
P N - V_a = s \, P N
\]

\[
a = s \, P N
\]

Since Force = mass \( \times \) acceleration,

\[
\text{Thrust } T = M \times a = \rho A P N \times s \, P N = \rho A P^2 N^2 s \quad \text{Newton}
\]

It is interesting to note that increased slip leads to increased thrust and that the propeller will not exert a thrust with zero slip. The power produced by the propeller is known as the thrust power (\( tp \)):

\[
tp = \text{Thrust (N)} \times \text{speed of advance (m/s)} = T \times V_a \quad \text{W}
\]
