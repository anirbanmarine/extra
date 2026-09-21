---
Title: "Gnomonic projection tangent to equator"
type: docs
---
## 1. Select the tangent point

```mermaid
flowchart LR
    A["Globe"] --> B["Equator"]
    B --> C["Select central meridian 40°E"]
    C --> D["Tangent point T at Equator ∩ 40°E"]
    D --> E["Projection plane tangent at T"]
```

## 2. Establish the tangent plane

```mermaid
flowchart TB
    O((O<br/>Earth centre))
    T((T<br/>tangent point))
    P["Tangent plane"]

    O ---|"Radius OT"| T
    T ---|"OT perpendicular to plane"| P

    Note["The projection plane touches the globe only at T"]
    P -.-> Note
```

A more geometrical side view is:

```mermaid
flowchart LR
    A["Globe surface"] --> B["T"]
    B --> C["Tangent plane"]
    O((O)) ---|"OT ⟂ tangent plane"| B
```

## 3. Mark the globe meridians

```mermaid
flowchart TB
    E["Equator"]
    M1["20°E"]
    M2["30°E"]
    M3["40°E"]
    M4["50°E"]
    M5["60°E"]

    E --> M1
    E --> M2
    E --> M3
    E --> M4
    E --> M5

    M3 --> C["Central meridian"]
    C --> T["Tangent point at Equator"]
```

The meridian arrangement is:

```mermaid
flowchart LR
    A["20°E"] --- B["30°E"] --- C["40°E"] --- D["50°E"] --- E["60°E"]
    C --- F["Central meridian and tangent point"]
```

## 4. Project the equator

```mermaid
flowchart LR
    G["Point on globe equator"] --> O((O<br/>centre))
    O --> P["Intersection with tangent plane"]
    P --> Q["Transfer to plan"]
    Q --> R["Projected equator"]
```

For several equatorial points:

```mermaid
flowchart TB
    E1["Equator ∩ 20°E"] --> O1((O))
    E2["Equator ∩ 30°E"] --> O2((O))
    E3["Equator ∩ 40°E"] --> O3((O))
    E4["Equator ∩ 50°E"] --> O4((O))
    E5["Equator ∩ 60°E"] --> O5((O))

    O1 --> P1["Tangent plane"]
    O2 --> P2["Tangent plane"]
    O3 --> P3["Tangent plane"]
    O4 --> P4["Tangent plane"]
    O5 --> P5["Tangent plane"]

    P1 --> L["Join transferred points"]
    P2 --> L
    P3 --> L
    P4 --> L
    P5 --> L

    L --> R["Straight projected equator"]
```

## 5. Construct the projected meridians

```mermaid
flowchart LR
    A["Choose globe meridian"] --> B["Mark its equatorial point"]
    B --> C["Join point to globe centre O"]
    C --> D["Extend line to tangent plane"]
    D --> E["Transfer intersection to plan"]
    E --> F["Draw perpendicular to projected equator"]
    F --> G["Projected meridian"]
```

For the complete set:

```mermaid
flowchart TB
    A["Projected equator"]

    M20["20°E point"] --> L20["Perpendicular line"]
    M30["30°E point"] --> L30["Perpendicular line"]
    M40["40°E point"] --> L40["Perpendicular line"]
    M50["50°E point"] --> L50["Perpendicular line"]
    M60["60°E point"] --> L60["Perpendicular line"]

    A --> M20
    A --> M30
    A --> M40
    A --> M50
    A --> M60

    L20 --> R["Five projected meridians"]
    L30 --> R
    L40 --> R
    L50 --> R
    L60 --> R
```

The central meridian is identified separately:

```mermaid
flowchart TB
    A["Projected equator"]
    B["40°E equatorial point"]
    C["Draw perpendicular"]
    D["Central meridian"]
    E["Tangent point T"]

    A --> B --> C --> D
    D --> E
```

## 6. Project the \(30^\circ N\) parallel

```mermaid
flowchart LR
    A["Select intersection of 30°N and a meridian"] --> B["Join point to globe centre O"]
    B --> C["Extend ray to tangent plane"]
    C --> D["Transfer projected point to plan"]
    D --> E["Repeat for every meridian"]
    E --> F["Join points with smooth curve"]
    F --> G["Projected 30°N parallel"]
```

For the five required meridians:

```mermaid
flowchart TB
    N20["30°N ∩ 20°E"] --> O20((O))
    N30["30°N ∩ 30°E"] --> O30((O))
    N40["30°N ∩ 40°E"] --> O40((O))
    N50["30°N ∩ 50°E"] --> O50((O))
    N60["30°N ∩ 60°E"] --> O60((O))

    O20 --> P20["Projected point"]
    O30 --> P30["Projected point"]
    O40 --> P40["Projected point"]
    O50 --> P50["Projected point"]
    O60 --> P60["Projected point"]

    P20 --> C["Smooth connecting curve"]
    P30 --> C
    P40 --> C
    P50 --> C
    P60 --> C

    C --> R["30°N projected parallel"]
```

## 7. Project the \(30^\circ S\) parallel

```mermaid
flowchart LR
    A["Select intersection of 30°S and a meridian"] --> B["Join point to globe centre O"]
    B --> C["Extend ray to tangent plane"]
    C --> D["Transfer projected point to plan"]
    D --> E["Repeat for every meridian"]
    E --> F["Join points with smooth curve"]
    F --> G["Projected 30°S parallel"]
```

```mermaid
flowchart TB
    S20["30°S ∩ 20°E"] --> O20((O))
    S30["30°S ∩ 30°E"] --> O30((O))
    S40["30°S ∩ 40°E"] --> O40((O))
    S50["30°S ∩ 50°E"] --> O50((O))
    S60["30°S ∩ 60°E"] --> O60((O))

    O20 --> P20["Projected point"]
    O30 --> P30["Projected point"]
    O40 --> P40["Projected point"]
    O50 --> P50["Projected point"]
    O60 --> P60["Projected point"]

    P20 --> C["Smooth connecting curve"]
    P30 --> C
    P40 --> C
    P50 --> C
    P60 --> C

    C --> R["30°S projected parallel"]
```

## 8. Descriptive-geometry transfer

```mermaid
flowchart LR
    A["Globe plan"] --> B["Project point vertically to elevation"]
    B --> C["Locate corresponding point in elevation"]
    C --> D["Join point to O"]
    D --> E["Intersect tangent plane"]
    E --> F["Project intersection back to plan"]
    F --> G["Final map point"]
```

For each graticule intersection:

```mermaid
flowchart TB
    A["Intersection on globe"]
    B["Plan view"]
    C["Elevation view"]
    D["Line from O"]
    E["Tangent-plane intersection"]
    F["Transferred point on map"]

    A --> B
    B --> C
    C --> D
    D --> E
    E --> F
```

## 9. Final construction sequence

```mermaid
flowchart TD
    A["Choose tangent point at 40°E on Equator"]
    B["Draw tangent plane"]
    C["Mark globe meridians 20°E–60°E"]
    D["Project equatorial points"]
    E["Draw five projected meridians"]
    F["Mark 30°N intersections on globe"]
    G["Project 30°N points"]
    H["Join them smoothly"]
    I["Mark 30°S intersections on globe"]
    J["Project 30°S points"]
    K["Join them smoothly"]
    L["Complete equatorial gnomonic graticule"]

    A --> B --> C --> D --> E
    E --> F --> G --> H
    H --> I --> J --> K
    K --> L
```

## 10. Final schematic graticule

This is only a conceptual Mermaid representation; it is not geometrically to scale.

```mermaid
flowchart TB
    N["30°N curved parallel"]
    E["Equator"]
    S["30°S curved parallel"]

    M20["20°E"] --- M30["30°E"] --- M40["40°E"] --- M50["50°E"] --- M60["60°E"]

    N --- E --- S
    M20 --- M30 --- M40 --- M50 --- M60
    M40 --> C["Central meridian"]
    C --> T["Tangent point at 40°E"]
```

The operational rule represented by all the diagrams is:

> Select a point on the globe, join it to the globe’s centre, extend that line to the tangent plane, and transfer the intersection to the map. Repeat for every required graticule intersection.