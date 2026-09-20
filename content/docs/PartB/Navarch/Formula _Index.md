---
title: Formulae
type: docs
math: true  
---
## Form Coefficients
WPA = Waterplane area
L = Length overall
B = maximum breadth
d = maximum depth
\[C_w\] = coefficient of waterplane area
\[C_m\] = coefficient of midship area


\[ WPA = L\times B \times C_w \]

\[ Area Amidships = B \times d\times C_m \]

## when displacement is constant ( box shaped vessels)
\[\frac {New Displacement}{Old Displacement} = \frac{New Density}{Old Density}\]

\[TPC_{SW}= \frac {WPA} {97.56} \]

\[FWA = \frac {W} { 4 times TPC_{SW}} \]

change in draft 
\[ = \frac {FWA \times (1025-\rho_{DW}) }{25} \]

## Trim 

\[MCTC = \frac {W \times GM_L}{100 \times L}\]

\[GM_L = KM_L-KG \]
\[KM_L = KB + BM_L\]
\[BM_L = \frac{I_{LL}}{\nabla}\]

Change in Trim \(\Delta_T\)

\[\Delta_T = \frac{Trimming moment}{MCTC}= \frac{ W \times (LCB_{foap}-LCG_{foap})}{MCTC}\]

Change of draft Aft \(\delta_{aft} = \frac{1}{L} \times \Delta_T\) 

distance 'd' to keep aft draft constant \(\frac{MCTC \times L}{TPC \times l}\)

## Simpson's Rules
Common Area = h

* \[Area = \frac{1}{3} \times h \times \Sigma_1\] 
Multipliers (1,4,1)
* \[ Area = \frac {3h}{8} \times \Sigma_1\] 
Multipliers (1,3,3,1)
* \[Area = \frac{h}{12}(5a+8b-c)\]

## Second Moment of Inertia (**I**)

Essentially moment of an Area about an axis .
Here the formulas are given for its own centroidal axis.

### rectangle\(B \times L \)

For rectangular waterplane Area \[ I_{CG} = \frac { L \times B^3}{12}\]

\[BM = \frac{I}{V}\]
### triangle base ='B', height ='H'

\[I_{CG}= \frac{B\times H^3}{36}\]

### Circle of Radius 'R'

\[I_{CG} = \frac{\pi \times R^4}{4}\]

Polar moment is (for rudder stock problem) \(J = \frac{\pi \times R^4}{2}\)

### Prism base 'B','C' and height 'H'

\[I_{CG}= \frac {H^3}{36} \times \frac{B^2+4BC+C^2}{B+C}\]

### for the Sectional Modulus Problem:

where b is the horizontal length and h can be height or can be thickness 

\[I_{CG} = \frac {bh^3}{12}\]
  


### **General Formula (Inclined Surface)**
\[h_{CP} = \bar{h} + \frac{I_G \sin^2\theta}{A\bar{h}}\]
*For vertical surfaces \(\theta = 90°\):* \(\quad h_{CP} = \bar{h} + \dfrac{I_G}{A\bar{h}}\)

---

### **Shape Properties & Center of Pressure**

| Shape | Area \(A\) | Centroid Depth \(\bar{h}\)* | \(I_G\) (about centroid) | \(h_{CP}\) (Vertical Surface) |
| :--- | :--- | :--- | :--- | :--- |
| **Rectangle** width \(b\), height \(h\) | \(bh\) | \(\frac{h}{2}\) (top at surface) | \(\frac{bh^3}{12}\) | \(\frac{2h}{3}\) |
| **Triangle** (base \(b\), height \(h\), apex up) | \(\frac{1}{2}bh\) | \(\frac{2h}{3}\) (top/apex at surface) | \(\frac{bh^3}{36}\) | \(\frac{3h}{4}\) |
| **Circle** (radius \(R\)) | \(\pi R^2\) | \(R\) (top at surface) | \(\frac{\pi R^4}{4}\) | \(\frac{5R}{4}\) |
| **Trapezoid** (bases \(B\) bottom, \(C\) top, height \(h\)) | \(\frac{B+C}{2}h\) | \(\frac{h}{3}\cdot\frac{B+2C}{B+C}\) (top at surface) | \(\frac{h^3}{36}\cdot\frac{B^2+4BC+C^2}{B+C}\) | \(\bar{h} + \frac{h^2}{18\bar{h}}\cdot\frac{B^2+4BC+C^2}{(B+C)^2}\) |
| **Semicircle** (radius \(R\), flat side up) | \(\frac{\pi R^2}{2}\) | \(\frac{4R}{3\pi}\) (diameter at surface) | \(0.1098R^4\) | \(\bar{h} + \frac{0.1098R^4}{\frac{\pi R^2}{2}\cdot\bar{h}}\) |

*\*Measured from the free surface to the shape's centroid. For submerged cases, add the depth of the top edge.*

---

### **Quick Exam Shortcuts**
*   **Rectangle (top at surface):** \(h_{CP} = \frac{2}{3}h\) (measured from top)
*   **Triangle (apex at surface):** \(h_{CP} = \frac{3}{4}h\) (measured from apex)
*   **Circle (top at surface):** \(h_{CP} = \frac{5}{4}R\) (measured from top)
*   **Universal Check:** \(h_{CP}\) is always **below** the centroid ( \( \bar{h}\)) for vertical/inclined surfaces.

### **Bilging Connection (from your previous point)**
*   **Sinkage:** \(\dfrac{\text{Lost Volume}}{\text{Intact Waterplane Area}}\)
*   **New \(GM_T\):** Use \(I_{T,\text{intact}}\) (about centerline) \(\rightarrow BM_T = \frac{I_T}{\nabla}\)
*   **New \(GM_L\):** Use \(I_{L,\text{intact}}\) (about midships) \(\rightarrow BM_L = \frac{I_L}{\nabla}\)

**Pro Tip:** If the surface is **inclined**, remember the \(\sin^2\theta\) factor. If the tank wall is **curved**, find the horizontal/vertical force components first; the center of pressure formula above applies only to **plane** surfaces.





