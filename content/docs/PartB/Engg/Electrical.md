---
title: Electrical Machines Revision Notes
toc: true
type: docs
math: true

---

 

## 1. Transformers
**Principle:** Static device that transfers AC electrical power between circuits via **electromagnetic induction** (Faraday’s Law) without changing frequency.
- **Core:** Laminated silicon steel (0.3–0.5 mm) to minimize **eddy current losses**.
- **Types:** Step-up/Step-down, Core-type / Shell-type, Single/Three-phase.

### 🔑 Key Formulas
- **Faraday’s Law:** $$e = -N \frac{d\phi}{dt}$$
- **Turns Ratio (Ideal):** $$\frac{V_1}{V_2} = \frac{N_1}{N_2} = \frac{I_2}{I_1} = K$$
- **EMF Equation:** $$E_1 = 4.44 f N_1 \Phi_m$$  and  $$E_2 = 4.44 f N_2 \Phi_m$$
  *(where $$f$$ = frequency, $$N$$ = turns, $$\Phi_m$$ = max flux)*
- **Voltage Regulation:** $$\%VR = \frac{V_{nl} - V_{fl}}{V_{fl}} \times 100\%$$
- **Efficiency:** $$\eta = \frac{P_{out}}{P_{in}} \times 100\% = \frac{P_{out}}{P_{out} + P_{cu} + P_{core}} \times 100\%$$
- **Max Efficiency Condition:** Copper Loss ($$I^2R$$) = Core (Iron) Loss

### 🧪 Testing
- **Open Circuit (O.C.) Test:** Done on HV side. Finds **core losses**, no-load current ($$I_0$$), and shunt parameters ($$G_0, B_0$$).
- **Short Circuit (S.C.) Test:** Done on LV side. Finds **full-load copper losses** and series impedance ($$R_{01}, X_{01}$$).

### 🔌 Special Transformers
- **Auto-transformer:** Single winding acts as both primary and secondary. Economical for small voltage adjustments.
- **3-Phase Connections:** Y-Y, Y-$$\Delta$$, $$\Delta$$-Y, $$\Delta$$-$$\Delta$$. ($$\Delta$$-$$\Delta$$ can operate as "Open Delta" or V-V connection if one transformer fails).

---

## 2. Induction Motors (IM)
**Principle:** Stator's 3-phase supply creates a **Rotating Magnetic Field (RMF)**, which induces voltage and current in the short-circuited rotor, producing torque.
- **Construction:** 
  - *Stator:* Stationary, laminated core with 3-phase slots.
  - *Rotor:* Squirrel-cage (robust, low maintenance) or Wound-rotor (slip rings, external resistance possible).

### 🔑 Key Formulas
- **Synchronous Speed:** $$n_{sync} = \frac{120 f_e}{P}$$ *(in rpm)*
- **Slip ($$s$$):** $$s = \frac{n_{sync} - n_m}{n_{sync}}$$ 
  *(where $$n_m$$ = mechanical rotor speed; $$s=1$$ at standstill, $$s=0$$ at sync speed)*
- **Rotor Frequency:** $$f_r = s \cdot f_e$$
- **Induced Torque:** $$\tau_{ind} = k (B_R \times B_S)$$
- **Starting Torque Relation:** $$T_{start} \propto V_{start}^2 \propto I_{start}^2$$

### 🚦 Starting Methods (to limit high inrush current)
1. **D.O.L. (Direct-On-Line):** Full voltage applied. Simple, cheap, but high starting current. Used for motors $$< 5$$ kW.
2. **Star-Delta:** Starts in Star (voltage per phase = $$1/\sqrt{3}$$ of rated), switches to Delta at ~80% speed. Reduces starting current and torque to **1/3** of DOL values.
3. **Auto-transformer Starter:** Uses taps to reduce starting voltage. Suitable for large motors ($$> 20$$ kW).
4. **Rotor Resistance Starter:** (Slip-ring only) Adds external resistance to increase starting torque and reduce starting current.
5. **Soft Starter:** Uses back-to-back SCRs to smoothly ramp up voltage/current.

---

## 3. Synchronous Machines (Generators & Motors)
### 🔄 Synchronous Generators (Alternators)
**Principle:** Converts mechanical energy to 3-phase AC electrical energy. Field winding is on the **rotor** (DC excited via 2 slip rings), armature winding is on the **stator** (easier to insulate for high voltage, no large slip rings needed).

#### Rotor Types:
| Feature | Salient Pole | Non-Salient (Cylindrical) |
| :--- | :--- | :--- |
| **Speed** | Low/Medium (120–400 rpm) | High (1500–3000 rpm) |
| **Prime Mover** | Hydro/Water turbine | Steam turbine (Turboalternator) |
| **Geometry** | Large diameter, short length | Small diameter, long length |
| **Air Gap** | Non-uniform ($$X_d \neq X_q$$) | Uniform ($$X_d = X_q = X_s$$) |
| **Poles** | $$> 4$$ poles | $$\le 4$$ poles |

#### 🔑 Key Formulas
- **Frequency:** $$f = \frac{P \cdot N}{120}$$ *(Hz)*
- **Induced EMF per phase:** $$E_{ph} = 4.44 \Phi f T K_w$$ 
  *(where $$K_w = K_p K_d$$ is the winding factor)*
- **Line Voltage (Star-connected):** $$E_L = \sqrt{3} E_{ph}$$

#### ⚙️ Automatic Voltage Regulator (AVR)
- **Function:** Maintains constant generator terminal voltage under varying loads by automatically adjusting the DC excitation current to the rotor field winding.

### 🔄 Synchronous Motors
**Principle:** Stator RMF locks with the DC-excited rotor poles. 
- **Critical Trait:** **Not self-starting**. Net average starting torque is zero because the torque reverses every half-cycle ($$T \propto \sin\delta$$), and rotor inertia prevents it from following the rapidly reversing field.

#### Starting Methods:
1. **Damper Winding (Amortisseur):** Copper bars embedded in rotor poles (acts like a squirrel-cage IM). Motor starts as an IM, and once near $$n_{sync}$$, DC is applied to "pull into synchronism".
2. **Auxiliary Motor:** A small AC/DC motor brings the synchronous motor to near synchronous speed before DC excitation is applied.
3. **Slip-Ring Induction Start:** High external resistance is used to start as a wound-rotor IM, then switched to DC supply for synchronous operation.

---

### 💡 Quick Cross-Machine Comparisons
- **Transformer vs. IM:** Both work on mutual induction. In a transformer, the secondary is stationary; in an IM, the secondary (rotor) rotates, causing the rotor frequency to be $$f_r = s \cdot f_e$$.
- **Max Efficiency:** Achieved in transformers and motors when **Variable Losses (Copper) = Constant Losses (Core/Iron)**.
- **Slip:** Unique to induction machines. $$s=0$$ means rotor is at synchronous speed (no induced rotor current, no torque).
