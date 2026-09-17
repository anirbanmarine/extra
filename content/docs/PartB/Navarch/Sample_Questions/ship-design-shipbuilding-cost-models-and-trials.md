# **Ship Design, Shipbuilding Cost Models, and Trials**

---

## **1. Cost Models in Ship Design and Shipbuilding**

### **A. Overview of Cost Models**
Cost models in shipbuilding are used to **estimate, budget, and optimize** expenses across the **design, construction, and operational phases**. These models help shipyards and owners **predict costs, allocate resources, and ensure profitability**. Common cost models include:

| **Cost Model**               | **Description**                                                                                     | **Application**                                                                                     |
|------------------------------|-----------------------------------------------------------------------------------------------------|-----------------------------------------------------------------------------------------------------|
| **Parametric Cost Models**   | Use **historical data** and **statistical relationships** to estimate costs based on ship parameters (e.g., DWT, LOA, speed). | Early-stage **conceptual design** and **feasibility studies**.                                               |
| **Analogous Cost Models**    | Estimate costs based on **similar past projects** (e.g., a new bulk carrier vs. a previously built one). | **Preliminary design** and **budgeting**.                                                          |
| **Bottom-Up Cost Models**    | Break down the ship into **components (hull, machinery, outfitting)** and sum their individual costs. | **Detailed design** and **contract bidding**.                                                      |
| **Cost Estimating Relationships (CER)** | **Mathematical equations** linking ship characteristics (e.g., displacement, power) to cost. | **Quick cost estimates** during **feasibility and conceptual design**.                              |
| **Activity-Based Costing (ABC)** | Allocates costs based on **activities** (e.g., welding, painting, assembly).                     | **Production planning** and **process optimization**.                                             |
| **Learning Curve Models**     | Account for **efficiency gains** as production progresses (e.g., reduced labor hours per unit).    | **Serial production** (e.g., building multiple ships of the same design).                          |

---

## **2. Cost Estimating Relationship (CER)**

### **A. Definition**
A **Cost Estimating Relationship (CER)** is a **mathematical or statistical model** that relates **ship characteristics** (e.g., displacement, length, power) to **cost**. CERs are derived from **historical data** and **regression analysis**.

### **B. Types of CERs**
| **Type**               | **Description**                                                                                     | **Example**                                                                                     |
|------------------------|-----------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|
| **Simple Linear CER**  | Cost = **a + b × (Ship Parameter)**.                                                               | Cost = 5,000,000 + 20,000 × (DWT)                                                 |
| **Power Law CER**      | Cost = **a × (Ship Parameter)^b**.                                                                  | Cost = 10,000 × (LOA)^1.7                                                          |
| **Multiple Regression CER** | Cost = **a + b₁X₁ + b₂X₂ + ... + bₙXₙ** (where X₁, X₂, etc., are ship parameters like DWT, speed, etc.). | Cost = 2,000,000 + 15,000 × (DWT) + 50,000 × (Speed)                              |

### **C. Advantages of CERs**
- **Quick estimates**: Useful for **early-stage design** when detailed data is unavailable.
- **Scalability**: Can be applied to **different ship sizes** within a class (e.g., bulk carriers, tankers).
- **Data-driven**: Based on **historical trends**, reducing subjective bias.

### **D. Limitations of CERs**
- **Accuracy depends on data quality**: Poor historical data leads to unreliable estimates.
- **Assumes linearity**: May not capture **non-linear cost drivers** (e.g., complex machinery).
- **Less accurate for innovative designs**: Works best for **conventional ships** with existing data.

### **E. Example CER for Shipbuilding**
For a **bulk carrier**, a CER might look like:
```
Cost (USD) = 12,000,000 + 18,000 × (DWT) + 30,000 × (Engine Power in kW)
```
Where:
- **DWT** = Deadweight Tonnage
- **Engine Power** = Main engine power in kW

---

## **3. Hull Block Construction Method (HBCM)**

### **A. Definition**
The **Hull Block Construction Method (HBCM)** is a **modular shipbuilding approach** where the hull is constructed in **pre-fabricated blocks** (sections) that are later **assembled in the dry dock or on the slipway**. This method is widely used in **modern shipyards** (e.g., Hyundai, Samsung Heavy Industries).

### **B. Cost Savings in HBCM**
| **Cost-Saving Factor**       | **Explanation**                                                                                     |
|------------------------------|-----------------------------------------------------------------------------------------------------|
| **Reduced Labor in Dry Dock** | Blocks are **pre-fabricated in workshops**, reducing **on-site labor** and **construction time**. |
| **Parallel Processing**       | Different blocks can be **built simultaneously**, shortening the **total build time**.       |
| **Improved Quality Control** | Workshop conditions allow for **better precision** and **fewer rework costs**.                  |
| **Economies of Scale**        | **Bulk material procurement** and **standardized processes** reduce costs.                     |
| **Reduced Dry Dock Time**    | Blocks are **assembled quickly** in the dry dock, minimizing **dock rental costs**.              |
| **Lower Skilled Labor Needs** | **Pre-fabrication** reduces the need for **highly skilled labor** on-site.                       |

### **C. HBCM Process**
1. **Block Design**: Hull is divided into **3D-modeled blocks** (e.g., bow, midship, stern).
2. **Pre-Fabrication**: Blocks are **cut, welded, and outfitted** in workshops.
3. **Transport**: Blocks are **moved to the dry dock** using cranes or transporters.
4. **Assembly**: Blocks are **welded together** to form the hull.
5. **Outfitting**: **Piping, electrical, and machinery** are installed.

---

## **4. Advantages of Pre-Fabrication**

### **A. Cost and Time Savings**
| **Advantage**               | **Explanation**                                                                                     |
|-----------------------------|-----------------------------------------------------------------------------------------------------|
| **Reduced Construction Time** | **Parallel processing** of blocks shortens the **total build schedule**.                     |
| **Lower Labor Costs**       | **Workshop-based fabrication** reduces **on-site labor** and **overhead costs**.              |
| **Better Working Conditions** | Workers operate in **controlled environments** (e.g., covered workshops), improving **productivity and safety**. |
| **Higher Precision**        | **CNC cutting and automated welding** improve **dimensional accuracy**, reducing rework.      |
| **Material Efficiency**     | **Optimized nesting** (cutting patterns) reduces **steel wastage**.                              |
| **Easier Quality Control**  | **Inspection and testing** are easier in a **workshop setting**.                                  |
| **Reduced Weather Delays**  | **Indoor fabrication** minimizes **weather-related disruptions**.                               |

### **B. Examples of Pre-Fabrication**
- **Hull Blocks**: Pre-welded sections of the hull.
- **Pipe Spools**: Pre-fabricated piping systems.
- **Electrical Panels**: Pre-assembled and tested electrical distribution boards.
- **Accommodation Modules**: Pre-built living quarters (e.g., cabins, galleys).

---

## **5. Estimating Finished Steel Weight of a Ship**

### **A. Methods for Estimating Steel Weight**
| **Method**               | **Description**                                                                                     | **Accuracy** | **Stage of Design** |
|--------------------------|-----------------------------------------------------------------------------------------------------|--------------|---------------------|
| **Parametric Estimation** | Uses **CERs** or **statistical formulas** based on ship dimensions (e.g., L × B × D).          | Low          | Conceptual Design   |
| **Lightweight Analysis** | Breaks down the ship into **structural components** (hull, decks, bulkheads) and sums their weights. | Medium       | Preliminary Design  |
| **3D CAD Modeling**      | Uses **detailed 3D models** (e.g., NAPA, CADMATIC) to calculate **exact steel weights**.        | High         | Contract Design     |
| **Class Society Rules** | Uses **classification society formulas** (e.g., Lloyd’s Register, ABS, DNV) for minimum scantlings. | Medium       | All Stages          |

### **B. Parametric Formula for Steel Weight**
A simple **parametric formula** for estimating steel weight (for a **bulk carrier**):
```
Steel Weight (tons) = C × (L × B × D)^(2/3)
```
Where:
- **L** = Length Overall (m)
- **B** = Breadth (m)
- **D** = Depth (m)
- **C** = Constant (varies by ship type, e.g., **0.015–0.025** for bulk carriers)

### **C. Lightweight Analysis**
1. **Hull Girder Weight**:
   - **Bottom, side, deck plating** + **longitudinals, transverses, webs, and stiffeners**.
2. **Superstructure Weight**:
   - **Accommodation, bridge, funnel** (if applicable).
3. **Outfitting Weight**:
   - **Piping, electrical systems, machinery supports** (if included in steel weight).

---

## **6. Basic Ship Design vs. New Ship Design**

### **A. Basic Ship Design (Shipyard’s Standard Design)**
- **Definition**: A **proven, standardized design** that the shipyard has built before (e.g., a **Newcastlemax bulk carrier** or a **Suezmax tanker**).
- **Characteristics**:
  - **Pre-existing drawings, calculations, and specifications**.
  - **Optimized for construction efficiency** (e.g., pre-fabricated blocks, standardized materials).
  - **Lower design costs** (no R&D required).
  - **Faster delivery** (familiar to the shipyard).

### **B. New Ship Design (Custom Design)**
- **Definition**: A **bespoke design** tailored to the owner’s **specific requirements** (e.g., a **specialized LNG carrier** or a **polar icebreaker**).
- **Characteristics**:
  - **Unique hull form, machinery, and outfitting**.
  - **Higher design costs** (R&D, model testing, class approval).
  - **Longer delivery time** (new tooling, training, and processes).
  - **Higher risk** (unproven performance, potential cost overruns).

### **C. Narrowing the Differences**
To bridge the gap between a **basic design** and a **new design**, the following steps are taken:

| **Step**                          | **Description**                                                                                     |
|-----------------------------------|-----------------------------------------------------------------------------------------------------|
| **Feasibility Study**             | Assess **technical and economic viability** of the new design.                                  |
| **Parametric Comparisons**        | Compare **key dimensions** (LOA, DWT, speed) with existing designs.                              |
| **Model Testing**                 | Conduct **towing tank tests** or **CFD analysis** to validate performance.                     |
| **Class Society Approval**       | Obtain **preliminary approval** from classification societies (e.g., ABS, DNV, LR).             |
| **Modular Adaptations**          | Use **pre-existing modules** (e.g., engine room, accommodation) from basic designs.             |
| **Cost-Benefit Analysis**        | Evaluate **trade-offs** between customization and cost.                                          |
| **Iterative Design Refinement** | Gradually **refine the design** through multiple iterations (see **Design Spiral** below).     |

---

## **7. Slog-Slog Method**

### **A. Definition**
The **"Slog-Slog" method** (also called the **"Log-Log" method**) is a **graphical cost estimation technique** used in shipbuilding to **compare costs across different ship sizes or designs**. It involves plotting **cost vs. ship parameter (e.g., DWT, LOA)** on a **logarithmic scale** for both axes.

### **B. When is it Used?**
- **Early-stage cost estimation** (when detailed data is unavailable).
- **Comparing costs of different ship sizes** (e.g., scaling a 50,000 DWT bulk carrier to 80,000 DWT).
- **Benchmarking** against industry standards.

### **C. How It Works**
1. **Plot historical data** (cost vs. ship parameter) on a **log-log graph**.
2. **Draw a best-fit line** (represents the **cost trend**).
3. **Use the line to estimate costs** for new ship sizes.

### **D. Example**
If the cost of a **50,000 DWT bulk carrier** is **$30M**, and the cost of a **100,000 DWT bulk carrier** is **$50M**, the **Slog-Slog method** can estimate the cost of a **75,000 DWT bulk carrier** by interpolating on the log-log plot.

---

## **8. Estimating Labour and Material Costs in Shipbuilding**

### **A. Labour Cost Estimation**
| **Factor**               | **Method**                                                                                     |
|--------------------------|-------------------------------------------------------------------------------------------------|
| **Man-Hours per Task**   | Estimate **labor hours** for each task (e.g., welding, painting, assembly) based on **historical data**. |
| **Wage Rates**           | Multiply man-hours by **hourly wage rates** (varies by country and skill level).                 |
| **Productivity Factors** | Adjust for **worker efficiency** (e.g., learning curve, fatigue, experience).                 |
| **Overhead Costs**       | Include **supervision, training, and administrative costs**.                                    |

#### **Formula for Labour Cost**
```
Labour Cost = Σ (Man-Hours × Hourly Rate × Productivity Factor)
```

### **B. Material Cost Estimation**
| **Factor**               | **Method**                                                                                     |
|--------------------------|-------------------------------------------------------------------------------------------------|
| **Steel Weight**         | Estimated using **CERs or 3D modeling** (see Section 5).                                       |
| **Unit Cost of Steel**   | Multiply steel weight by **cost per ton** (varies by market prices).                          |
| **Other Materials**      | Include **paint, piping, electrical components, machinery, and outfitting**.                  |
| **Wastage Factor**       | Account for **cutting and fabrication waste** (typically **5–15%** of total material).         |

#### **Formula for Material Cost**
```
Material Cost = (Steel Weight × Cost per Ton) + (Other Materials Cost) × (1 + Wastage Factor)
```

### **C. Productivity Factors**
Productivity factors **adjust labour and material cost estimates** to account for **real-world conditions**. Common factors include:

| **Factor**               | **Impact on Cost**                                                                                     | **Example**                                                                                     |
|--------------------------|-----------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|
| **Learning Curve**       | **Reduces labour hours** as workers gain experience (e.g., **90% learning curve**).              | After building 10 ships, labour hours per ship may drop by **10–20%**.                          |
| **Work Environment**     | **Harsh conditions** (e.g., extreme weather, confined spaces) **increase labour time**.         | Welding in a **cold, open dry dock** may require **20% more time** than in a workshop.             |
| **Skill Level**          | **Higher-skilled workers** are **more efficient** but **cost more per hour**.                    | A **certified welder** may cost **$50/hr** vs. **$30/hr** for an apprentice.                     |
| **Tooling and Equipment**| **Advanced tools** (e.g., **automated welding, CNC cutting**) **reduce labour time**.             | **Robotic welding** can reduce labour costs by **30–40%**.                                     |
| **Fatigue**              | **Long shifts or overtime** can **reduce productivity** by **10–20%**.                            | Workers on **12-hour shifts** may be **15% less productive** than on 8-hour shifts.             |
| **Quality Control**      | **Rework due to defects** increases labour and material costs.                                  | **10% rework rate** can add **5–10%** to total costs.                                           |

---

## **9. Ship Trials**

### **A. Overview of Ship Trials**
Ship trials are conducted to **verify the performance, safety, and compliance** of a newly built or refitted ship. They are typically divided into:
1. **Harbour Acceptance Trials (HAT)**: Basic checks in port (e.g., engine startup, navigation equipment).
2. **Sea Acceptance Trials (SAT)**: Performance tests at sea (e.g., speed, maneuvering, fuel consumption).
3. **Final Acceptance Trials**: Comprehensive tests before **delivery to the owner**.

---

### **B. Measured Mile Trial**

#### **A. Purpose**
- Measure the **ship’s speed and power performance** under **controlled conditions**.
- Verify **contractual speed and fuel consumption** guarantees.

#### **B. Procedure**
1. **Selection of Measured Mile**: A **calibrated, straight track** (typically **1–2 nautical miles long**) with **known current and tide conditions**.
2. **Test Conditions**:
   - **Calm weather** (Beaufort Scale ≤ 3, wave height ≤ 1.25 m).
   - **Stable loading** (ballast or cargo as per contract).
   - **Engine at MCR (Maximum Continuous Rating)** or specified power.
3. **Measurements**:
   - **Speed over ground (SOG)** (using GPS or Doppler log).
   - **Speed through water (STW)** (using a **paddle wheel log** or **electromagnetic log**).
   - **Engine parameters** (RPM, fuel consumption, exhaust temperature).
   - **Propeller shaft power** (using a **torsion meter**).

#### **C. Data Analysis**
- **Speed-Power Curve**: Plots **ship speed vs. engine power** to verify **contractual performance**.
- **Fuel Consumption Analysis**: Compares **actual fuel consumption** vs. **guaranteed values** at different speeds.
- **Hull Efficiency**: Assesses **hull cleanliness and fouling** impact on performance.

---

### **C. Fuel Consumption Trial**

#### **A. Inputs to be Measured and Recorded**
| **Category**               | **Inputs**                                                                                     |
|----------------------------|-------------------------------------------------------------------------------------------------|
| **Ship Parameters**        | Displacement, draft, trim, stability (GM), wind and current conditions.                      |
| **Engine Parameters**      | Engine RPM, fuel flow rate, fuel density, exhaust gas temperature, turbocharger pressure.    |
| **Propulsion Parameters**  | Propeller pitch, shaft RPM, torque, thrust.                                                   |
| **Environmental Conditions** | Air temperature, humidity, sea temperature, wave height, wind speed/direction.            |
| **Navigation Data**        | GPS position, speed over ground (SOG), speed through water (STW), course.                   |

#### **B. Outputs to be Measured and Recorded**
| **Category**               | **Outputs**                                                                                     |
|----------------------------|-------------------------------------------------------------------------------------------------|
| **Performance Metrics**    | Maximum speed at MCR, fuel consumption at various speeds, specific fuel consumption (SFC).  |
| **Engine Efficiency**      | Brake specific fuel consumption (BSFC), thermal efficiency.                                 |
| **Propulsion Efficiency**  | Propulsive efficiency, hull efficiency, wake fraction.                                       |
| **Emissions Data**         | CO₂, NOx, SOx emissions (for compliance with **IMO 2020, EEXI, CII**).                         |
| **Vibration and Noise**    | Vibration levels (in engine room, accommodation), noise levels (dB).                          |

---

### **D. Ship Maneuvering Trials**

#### **A. Turning Circle Trial**
- **Purpose**: Measure the **ship’s turning ability** and **tactical diameter**.
- **Procedure**:
  1. Ship approaches the **turning point** at **steady speed** (e.g., **80% of service speed**).
  2. **Hard starboard/port rudder** (typically **35°**) is applied.
  3. **Turning circle** is recorded using **GPS or radar tracking**.
- **Key Metrics**:
  - **Tactical Diameter**: Distance between the **initial and final course lines** (should be **≤ 5 × LOA** for most ships).
  - **Advance**: Distance traveled **along the original course** before the ship turns **90°**.
  - **Transfer**: Distance traveled **perpendicular to the original course** when the ship turns **90°**.
  - **Time to Turn 90°**: Should be **≤ 2–3 minutes** for most commercial ships.

#### **B. Crash Stop Trial**
- **Purpose**: Measure the **ship’s stopping ability** in an emergency.
- **Procedure**:
  1. Ship is brought to **full ahead speed** (e.g., **80–100% MCR**).
  2. **Full astern power** is applied, and **engine is reversed** (if applicable).
  3. **Stopping distance** and **time** are recorded.
- **Key Metrics**:
  - **Stopping Distance**: Distance traveled from **full ahead to full stop** (should be **≤ 15 × LOA** for most ships).
  - **Stopping Time**: Time taken to **come to a complete stop** (typically **10–20 minutes** for large ships).
  - **Head Reach**: Distance traveled **ahead of the initial position** before stopping.

#### **C. Fuel Consumption at MCR**
- **Purpose**: Verify **fuel efficiency** at **Maximum Continuous Rating (MCR)**.
- **Procedure**:
  1. Ship is brought to **MCR power** (100% engine load).
  2. **Fuel consumption** is measured over a **steady-state period** (e.g., 1–2 hours).
  3. **Exhaust emissions** are analyzed for compliance.
- **Key Metrics**:
  - **Specific Fuel Consumption (SFC)**: **kg of fuel per kWh** (should match **contractual guarantees**).
  - **Brake Specific Fuel Consumption (BSFC)**: **g/kWh** (typically **170–210 g/kWh** for modern diesel engines).
  - **Emissions**: **CO₂, NOx, SOx** (must comply with **IMO Tier III, EEXI, CII**).

---

## **10. Short Notes with Diagrams**

---

### **A. Lines Plan**

#### **A. Definition**
The **Lines Plan** is a **2D representation** of a ship’s **hull form**, showing the **shape and dimensions** of the hull in three views:
1. **Body Plan** (Cross-sectional views).
2. **Sheer Plan** (Side view).
3. **Half-Breadth Plan** (Top view).

#### **B. Components of a Lines Plan**
```
+-------------------+-------------------+-------------------+
|     Body Plan     |    Sheer Plan     | Half-Breadth Plan |
+-------------------+-------------------+-------------------+
| - Forward (FP)    | - Deck lines      | - Waterlines      |
| - Midship (MS)    | - Sheer lines     | - Buttock lines   |
| - Aft (AP)        | - Keel line       | - Diagonal lines  |
| - Vertical sections | - Stem profile    | - Station lines   |
+-------------------+-------------------+-------------------+
```

#### **C. Diagram (Text Representation)**
```
Sheer Plan (Side View):
  ___________ Deck Line
 /           \
|             | Sheer Line
|_____________| Keel Line

Body Plan (Cross-Section):
   _______
  /       \
 /         \
|           | Midship Section
 \         /
  \_______/

Half-Breadth Plan (Top View):
   ___________
  /           \
 /             \
|               |
 \             /
  \___________/
```

#### **D. Significance**
- **Hull Fairing**: Ensures **smooth curves** for **hydrodynamic efficiency**.
- **Structural Design**: Basis for **scantling calculations** and **strength analysis**.
- **Regulatory Compliance**: Used for **stability calculations** (e.g., **GZ curve, intact/damage stability**).
- **Construction Reference**: Guides **hull fabrication** and **block assembly**.

---

### **B. Design Spiral**

#### **A. Definition**
The **Design Spiral** is an **iterative process** used in ship design to **refine and optimize** the ship’s characteristics. It involves **multiple cycles** of analysis, evaluation, and modification.

#### **B. Stages of the Design Spiral**
```
1. Initial Design → 2. Weight Estimate → 3. Stability Check → 4. Powering Estimate →
5. Resistance Calculation → 6. Propulsion Selection → 7. Cost Estimate →
8. Feasibility Review → [If not satisfactory, return to Step 1]
```

#### **C. Diagram (Text Representation)**
```
       +------------------+
       | Initial Design   |
       +--------+---------+
                |
                v
       +--------+---------+
       |  Weight Estimate  |
       +--------+---------+
                |
                v
       +--------+---------+
       | Stability Check  |
       +--------+---------+
                |
                v
       +--------+---------+
       | Powering Estimate|
       +--------+---------+
                |
                v
       +--------+---------+
       |Resistance Calc.  |
       +--------+---------+
                |
                v
       +--------+---------+
       |Propulsion Select.|
       +--------+---------+
                |
                v
       +--------+---------+
       |   Cost Estimate  |
       +--------+---------+
                |
                v
       +--------+---------+
       |Feasibility Review|
       +------------------+
                |
                +---> [If OK: Final Design]
                |
                +---> [If Not OK: Revise Initial Design]
```

#### **D. Significance**
- **Iterative Refinement**: Allows designers to **adjust parameters** (e.g., dimensions, power) based on **performance feedback**.
- **Balancing Trade-Offs**: Optimizes **speed, fuel efficiency, cargo capacity, and cost**.
- **Feasibility Assurance**: Ensures the design meets **technical, regulatory, and economic** requirements.

---

### **C. Iterations in Ship Design**

#### **A. Definition**
**Iterations** are **repetitive cycles** of design refinement, where each cycle **improves the ship’s performance, cost, or compliance** with requirements.

#### **B. Types of Iterations**
| **Iteration Type**       | **Purpose**                                                                                     | **Example**                                                                                     |
|--------------------------|-------------------------------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------|
| **Parametric Iterations** | Adjust **key parameters** (e.g., L, B, D, speed) to meet performance targets.                | Increasing **LOA** to improve **cargo capacity** but checking impact on **resistance**.     |
| **Structural Iterations**| Optimize **scantlings** (thickness of plates, stiffeners) for **strength and weight**.        | Reducing **plate thickness** to save weight but ensuring **buckling strength** is maintained. |
| **Hydrodynamic Iterations** | Refine **hull form** for **better resistance, seakeeping, or maneuverability**.              | Adjusting **bow shape** to reduce **wave-making resistance**.                                |
| **Economic Iterations**  | Balance **capital cost (CAPEX)** and **operating cost (OPEX)**.                                | Choosing between a **higher-speed design** (more fuel cost) and a **slower-speed design** (lower fuel cost but longer voyage time). |

#### **C. Diagram (Text Representation)**
```
Initial Design → [Iteration 1: Adjust L, B, D] → Check Performance →
[Iteration 2: Optimize Scantlings] → Check Strength →
[Iteration 3: Refine Hull Form] → Check Resistance →
[Iteration 4: Balance CAPEX/OPEX] → Final Design
```

#### **D. Significance**
- **Convergence to Optimal Design**: Each iteration **narrows down** the best possible design.
- **Risk Mitigation**: Identifies and **resolves issues early** (e.g., stability, strength).
- **Cost Optimization**: Ensures the design is **economically viable**.

---

### **D. Contract Design**

#### **A. Definition**
The **Contract Design** is the **finalized ship design** agreed upon between the **shipyard and the owner**, forming the basis of the **construction contract**. It includes:
- **General Arrangement Plan (GA)**.
- **Lines Plan**.
- **Structural Drawings**.
- **Machinery and Outfitting Specifications**.
- **Performance Guarantees** (e.g., speed, fuel consumption, cargo capacity).

#### **B. Key Features**
- **Technical Specifications**: Detailed **dimensions, materials, and systems**.
- **Regulatory Compliance**: Meets **SOLAS, MARPOL, class society rules** (e.g., ABS, DNV, LR).
- **Commercial Terms**: **Price, delivery schedule, payment milestones**.
- **Performance Clauses**: **Speed, fuel efficiency, maneuvering** guarantees.

#### **C. Diagram (Text Representation)**
```
Contract Design Components:
+-------------------------------------+
| 1. General Arrangement Plan (GA)     |
| 2. Lines Plan                        |
| 3. Structural Drawings               |
| 4. Machinery Specifications          |
| 5. Outfitting Specifications         |
| 6. Performance Guarantees             |
| 7. Regulatory Certificates            |
+-------------------------------------+
```

#### **D. Significance**
- **Legal Binding**: Forms the **basis of the construction contract**. 
- **Construction Reference**: Guides **shipyard production** and **quality control**.
- **Owner’s Requirements**: Ensures the ship meets the **owner’s operational needs**.

---

### **E. Preliminary Design**

#### **A. Definition**
The **Preliminary Design** is an **intermediate stage** between **conceptual design** and **contract design**. It refines the **basic ship characteristics** and provides a **detailed feasibility assessment**.

#### **B. Key Activities**
1. **Hull Form Optimization**: Refine **lines plan** for **hydrodynamic efficiency**. 
2. **Weight and Stability Analysis**: Estimate **lightweight, deadweight, and stability** (GZ curve).
3. **Powering and Propulsion**: Select **engine type, power, and propeller design**. 
4. **Structural Design**: Define **scantlings, materials, and construction methods**. 
5. **Cost Estimation**: Develop a **detailed cost breakdown** (materials, labor, overheads).
6. **Regulatory Compliance Check**: Ensure design meets **SOLAS, MARPOL, class rules**.

#### **C. Diagram (Text Representation)**
```
Preliminary Design Process:
+-------------------+     +---------------------+     +-------------------+
|   Conceptual      |---->|  Preliminary Design |---->|  Contract Design   |
|   Design          |     |                     |     |                   |
+-------------------+     +---------------------+     +-------------------+
       |
       v
+-------------------+
| - Hull Form       |
| - Weight Estimate |
| - Stability Check |
| - Powering        |
| - Structural      |
| - Cost Estimate   |
+-------------------+
```

#### **D. Significance**
- **Feasibility Confirmation**: Validates **technical and economic viability**. 
- **Owner Feedback**: Allows the owner to **review and modify** the design before finalizing the contract.
- **Shipyard Planning**: Helps the shipyard **prepare for construction** (e.g., material procurement, block planning).

---

## **11. Discussion Questions**
1. How does the **Hull Block Construction Method (HBCM)** compare to **traditional shipbuilding** in terms of **cost and time savings**?
2. What are the **key challenges** in estimating **labour costs** for a **new ship design** with **unfamiliar features**?
3. How can **productivity factors** (e.g., learning curve, tooling) be **quantified and incorporated** into cost estimates?
4. What **lessons from the Emma Maersk fire** can be applied to **improve fire safety in modern ship designs**?
5. How does the **Slog-Slog method** help in **scaling costs** for ships of different sizes?
6. What are the **critical differences** between a **preliminary design** and a **contract design**?
7. How do **ship trials** ensure that a vessel meets its **contractual performance guarantees**?
8. What **innovations in shipbuilding** (e.g., **automation, AI**) are likely to **reduce costs** in the future?