Here's the derivation for the relationship between geocentric latitude (ψ) and geographic latitude (φ):

**Reference Surfaces and Ellipsoid Parameters:**

* We'll consider the Earth approximated by an oblate spheroid represented by an ellipsoid. 
* The ellipsoid has an equatorial radius (a) and a polar radius (b), with a > b due to the Earth's bulge.

**Geometry:**

1.  **Geographic Latitude (φ):** Imagine a point P on the Earth's surface.  Draw a line from P to the center of the Earth (O), designated PO.  Extend this line further upwards to pierce the equatorial plane at point Q.   Angle φ is the geographic latitude, which is the angle between the equatorial plane (EQ) and the line normal (perpendicular) to the ellipsoid at point P.

2. **Geocentric Latitude (ψ):**  Again, consider point P on the surface. Draw line PO connecting P to the Earth's center (O). Angle ψ is the geocentric latitude, which is the angle between the equatorial plane (EQ) and line PO.

**Relating the Angles:**

1. **Ellipsoid Normality:**  Line OP is normal (perpendicular) to the ellipsoid's surface at point P. This implies that angle OPQ (represented by ε) is 90 degrees.

2. **Angle Relationships:** Angles φ + ε and ψ sum to 90 degrees because OQ and OP lie on a straight line.  Therefore:

```
ψ + ε = 90°  (Equation 1)
```

**Relating Ellipsoid Geometry to ε:**

1. **Ellipsoid and Point P:**  Since P is on the ellipsoid's surface, point P is a distance 'a' from the center (O) along the equatorial plane and a distance 'b' from the center (O) along the polar axis.

2. **Triangle OPQ:** Triangle OPQ is a right triangle with right angle at Q.  We can use trigonometry to relate side lengths and angle ε.  In this case, we'll use the sine function (sin) because ε is opposite to side PQ and adjacent to side OP.

```
sin(ε) = PQ / OP  (Equation 2)
```

3. **PQ from Ellipsoid:**  From the ellipsoid definition, distance PQ is equal to the difference between the equatorial radius (a) and the distance from the center (O) to point P along the polar axis.  This distance along the polar axis is often denoted by 'z'.  Therefore:

```
PQ = a - z
```

4. **z from φ:** We can relate distance 'z' to geographic latitude (φ) using the concept of flattening.  Imagine a sphere inscribed within the ellipsoid, tangent to it at the equator. The distance from the center (O) to the equator on this sphere would be exactly 'a'.  As we move away from the equator towards the poles, the ellipsoid bulges outwards compared to the inscribed sphere. Distance 'z' represents the distance between the ellipsoid surface at point P and the surface of the inscribed sphere at the same latitude. There are various ways to calculate 'z' depending on the specific ellipsoid model being used. A common approach uses the following formula:

```
z = b * [1 - (1 - e^2) * sin^2(φ)]^(1/2)
```

where 'e' is the eccentricity of the ellipse, defined as:

```
e = sqrt(1 - (b^2 / a^2))
```

**Substituting and Simplifying:**

1. Substitute Equation 4 (z formula) into Equation 3 (PQ formula):

```
PQ = a - b * [1 - (1 - e^2) * sin^2(φ)]^(1/2)
```

2. Substitute Equation 5 (PQ formula) and OP (which is simply the equatorial radius 'a') into Equation 2 (sin(ε) formula):

```
sin(ε) = [a - b * [1 - (1 - e^2) * sin^2(φ)]^(1/2)] / a
```

3. Using trigonometric identities, we can rewrite sin(ε) as 1 - cos(ε)^2. Substitute this and rearrange the equation to solve for cos(ε):

```
cos(ε) = sqrt[ 1 - ( (a^2 - b^2) / a^2 ) * sin^2(φ)]
```

**Relating ε to ψ:**

1. Substitute Equation 1 (ψ + ε = 90°) and solve for cos(ε):

```
cos(ε) = sin(ψ)
```

2. Equate the two expressions for
