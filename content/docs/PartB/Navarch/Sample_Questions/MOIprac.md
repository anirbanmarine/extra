---
Title: "Moment of Inertia"
type: docs
---
![problem diagram](g8.svg)

draft =4m ,even keel, dimensions as above. GM = 5.2m

### **1. Divide the Waterplane into Simple Shapes**

We divide the waterplane into three sections:

* **Section 1 (Rectangle):** Length = \( 60\text{ m} \), Breadth = \( 20\text{ m} \)
* **Section 2 (Forward Triangle):** Base = \( 30\text{ m} \), Height = \( 20\text{ m} \)
* **Section 3 (Aft Triangle):** Base = \( 30\text{ m} \), Height = \( 20\text{ m} \)

### **2. Calculate Area and Local Moment of Inertia (\( I_{local} \))**

We need the local moment of inertia for each shape about its **own centroid**.

* **Rectangle:**
  * Area (\( A_{rect} \)) = \( 60 \times 20 = 1200\text{ m}^2 \)
  * \( I_{rect} = \frac{1}{12} \times \text{Breadth} \times \text{Length}^3 \)
  * \( I_{rect} = \frac{1}{12} \times 20 \times 60^3 = \mathbf{360,000\text{ m}^4} \)
  * Centroid is at midships (\( x = 0 \)).

* **One Triangle (e.g., Forward):**
  * Area (\( A_{tri} \)) = \( \frac{1}{2} \times 30 \times 20 = 300\text{ m}^2 \)
  * \( I_{tri\_local} = \frac{1}{36} \times \text{Base} \times \text{Height}^3 \)
  * \( I_{tri\_local} = \frac{1}{36} \times 30 \times 20^3 = \mathbf{6,666.67\text{ m}^4} \)
  * Centroid distance from midships (\( d \)): The centroid of a triangle is \( \frac{1}{3} \) from its base. The base is at \( x = 30\text{ m} \) from midships. So the centroid is at \( 30 + \frac{30}{3} = \mathbf{40\text{ m}} \) from midships.

### **3. Calculate Total Moment of Inertia (\( I_{total} \)) using Parallel Axis Theorem**

Formula: \( I_{total} = \sum (I_{local} + A \times d^2) \)

* **Rectangle:**
  * \( I_{rect\_total} = 360,000 + (1200 \times 0^2) = \mathbf{360,000\text{ m}^4} \)

* **Forward Triangle:**
  * \( I_{tri\_fwd} = 6,666.67 + (300 \times 40^2) \)
  * \( I_{tri\_fwd} = 6,666.67 + (300 \times 1600) = 6,666.67 + 480,000 = \mathbf{486,666.67\text{ m}^4} \)

* **Aft Triangle:**
  * Because the vessel is symmetrical, the aft triangle has the same area and is the same distance (\( d = 40\text{ m} \)) from midships.
  * \( I_{tri\_aft} = \mathbf{486,666.67\text{ m}^4} \)

* **Total Moment of Inertia (\( I_{total} \)):**
  * \( I_{total} = 360,000 + 486,666.67 + 486,666.67 = \mathbf{1,333,333.34\text{ m}^4} \)
  * *(Exact fraction: \( 360,000 + \frac{1,460,000}{3} + \frac{1,460,000}{3} = \frac{1,080,000 + 2,920,000}{3} = \frac{4,000,000}{3} \approx 1,333,333.33\text{ m}^4 \))*

### **4. Calculate Volume of Displacement (\(\nabla\))**

* Waterplane Area (\( A_w \)) = \( 1200 + 300 + 300 = 1800\text{ m}^2 \)
* Draft (\( d \)) = \( 4\text{ m} \)
* \( \nabla = A_w \times d = 1800 \times 4 = \mathbf{7,200\text{ m}^3} \)

### **5. Calculate BM (Metacentric Radius)**

* \( BM = \frac{I_{total}}{\nabla} \)
* \( BM = \frac{1,333,333.33}{7,200} = \mathbf{185.185\text{ m}} \)

### **6. Calculate KM (Height of Metacenter)**

* \( KB = \frac{\text{Draft}}{2} = \frac{4}{2} = \mathbf{2\text{ m}} \)
* \( KM = KB + BM = 2 + 185.185 = \mathbf{187.185\text{ m}} \)

### **7. Calculate GM (Metacentric Height)**

* Given \( KG = 5.2\text{ m} \)
* \( GM = KM - KG = 187.185 - 5.2 = \mathbf{181.985\text{ m}} \)

### **8. Calculate MCTC**

Formula: \( MCTC = \frac{W \times GM}{100 \times L} \)
*(Assuming standard sea water density \( \rho = 1.025\text{ t/m}^3 \))*

* \( W = \nabla \times \rho = 7200 \times 1.025 = \mathbf{7,380\text{ tonnes}} \)
* Total Length (\( L \)) = \( 30 + 60 + 30 = \mathbf{120\text{ m}} \)
* \( MCTC = \frac{7380 \times 181.985}{100 \times 120} \)
* \( MCTC = \frac{1,343,049.3}{12,000} \)
* \( MCTC \approx \mathbf{111.92\text{ tonnes-m/cm}} \)

*(Note: If fresh water density \( \rho = 1.0 \) is assumed, \( W = 7200\text{ t} \) and MCTC \( \approx 109.19\text{ tonnes-m/cm} \).)*

**Corrected Final Answer:**
**MCTC \(\approx\) 111.92 tonnes-m/cm** (assuming sea water).
