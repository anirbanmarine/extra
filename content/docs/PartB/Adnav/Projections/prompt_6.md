---
title: Discuss with respect to the theory and general appreciation of cartographical
  projections Lambert's orthomorphic and
type: docs
sidebar:
  open: true
---

Of course. Let's delve into a detailed discussion of the **Lambert Conformal Conic** projection, often known by its older name, Lambert's orthomorphic projection.

We will discuss it from two perspectives:
1.  **The Theory:** The geometric and mathematical principles behind its construction and properties.
2.  **The General Appreciation:** Its practical strengths, weaknesses, applications, and why it holds such an esteemed place in cartography.

***

### A Note on Terminology: Orthomorphic vs. Conformal

First, it's essential to clarify the term **"orthomorphic."** Coined from Greek (*orthos* = right, *morphe* = shape), it literally means "right-shaping." In modern cartography, the term **"conformal"** is used almost exclusively.

A **conformal (or orthomorphic) projection** is one that preserves angles locally. This means that if two lines on the globe intersect at a 90-degree angle, their corresponding lines on the map will also intersect at a 90-degree angle. A direct and highly valuable consequence of this property is that the **shapes of very small features are preserved**. A small island, for instance, will have the correct shape on the map, even if its size is distorted.

This preservation of shape comes at a cost: **area is not preserved**. On a conformal map, you cannot use the map to accurately compare the sizes of different regions.

---

### 1. The Theory of the Lambert Conformal Conic (LCC)

The LCC was designed by the brilliant Swiss mathematician and cartographer Johann Heinrich Lambert in 1772. It is a **conic** projection, meaning its construction is based on the idea of projecting the globe onto a cone.

#### The Geometric Concept: A Cone on a Globe

Imagine the Earth as a transparent globe with a light source at its center.
1.  A **cone** is placed over the globe, like a dunce cap. The axis of the cone is aligned with the Earth's axis of rotation (the North-South pole line).
2.  The features of the globe (continents, latitude/longitude lines) are "projected" from the central light source onto the surface of the cone.
3.  Finally, the cone is "unrolled" by cutting it along a line (a meridian), laying it flat to create the map.

This simple concept gives rise to the projection's fundamental characteristics:
*   **Parallels of latitude** are projected as concentric circles (or arcs of circles) on the cone.
*   **Meridians of longitude** are projected as straight lines radiating from a single point—the apex of the cone.

#### Tangent vs. Secant Case (The Key to its Usefulness)

There are two ways the cone can be placed, and this is crucial to understanding the LCC's genius.

*   **Tangent Cone:** The cone touches the globe along a single line of latitude. This line is called the **Standard Parallel**. Along this line, the map scale is perfectly true, and there is zero distortion. Distortion increases as you move away (north or south) from this standard parallel.

*   **Secant Cone (More Common):** The cone **slices through the globe**, intersecting it at two lines of latitude. These are the **two Standard Parallels**.
    *   Along these two parallels, the scale is perfectly true and distortion is zero.
    *   **Between** the two standard parallels, the scale is slightly smaller than reality (the map is compressed).
    *   **Outside** the two standard parallels, the scale becomes progressively larger than reality (the map is stretched).

The secant case is far more useful because it distributes the unavoidable distortion over a much larger area. By carefully choosing the two standard parallels, a cartographer can create a map with extremely low distortion across a wide band of latitude.

