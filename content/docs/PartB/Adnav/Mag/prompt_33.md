---
title: Marine Magnetic Compass adjustment:obtaining and explaining the approximate
  coefficients A, B, C, D and E;
type: docs
sidebar:
  open: true
---

Of course. This is a fundamental topic in marine navigation. Let's break down the approximate coefficients for magnetic compass adjustment in a clear, structured way.

### **Introduction: Why Do We Need Coefficients?**

A ship's magnetic compass is affected by the ship's own magnetic field, which is created by its steel hull (permanent magnetism) and soft iron components (induced magnetism). This interference causes the compass to point away from Magnetic North. This error, which changes as the ship changes heading, is called **Deviation**.

The process of "swinging the ship" is done to measure the deviation on various headings. The resulting data is then mathematically analyzed to understand the different magnetic forces at play. This analysis breaks the deviation down into five principal components, known as **Coefficients A, B, C, D, and E**.

These coefficients represent specific types of magnetic interference. By calculating them, a compass adjuster can:
1.  **Understand the source** of the deviation (e.g., permanent vs. induced magnetism).
2.  **Physically correct** the major errors using magnets and soft iron correctors in the binnacle.
3.  **Create a residual deviation card** for any small, remaining errors.

---

### **Obtaining the Data: Swinging the Ship**

Before you can calculate any coefficients, you must first measure the deviation. This is done by "swinging the ship":

1.  The ship is slowly turned through 360 degrees.
2.  At steady intervals (usually every 45 degrees: N, NE, E, SE, S, SW, W, NW), the ship is held on a constant heading.
3.  On each heading, the ship's **Compass Heading (CH)** is compared to the known **Magnetic Heading (MH)**. The Magnetic Heading is found using a reliable reference, like a gyrocompass with a known error, or by taking bearings of a distant object.
4.  The difference is the deviation: **Deviation = Magnetic Heading - Compass Heading**.
    *   If Magnetic is greater than Compass, the deviation is **Easterly (+)**.
    *   If Compass is greater than Magnetic, the deviation is **Westerly (-)**.

The deviations are recorded for each heading, forming the dataset needed to calculate the coefficients.

---

### **Explaining and Calculating the Approximate Coefficients**

The total deviation on any heading can be expressed by the approximate formula:
`Deviation ≈ A + B sin(CH) + C cos(CH) + D sin(2CH) + E cos(2CH)`

Here's what each coefficient means and how to calculate it using the deviation data from the swing.

### **Coefficient A**

*   **Explanation:** This is the **Constant Coefficient**. It represents a constant deviation that is the same on all headings.
*   **Physical Cause:**
    *   The primary cause is a physical misalignment of the compass lubber's line with the ship's fore-and-aft line.
    *   It can also be caused by consistent observer error or an error in the reference heading (e.g., gyro error) used during the swing.
*   **How to Obtain (Formula):** It is the average of the deviations on the four cardinal headings (N, E, S, W).
    `A = (Dev on N + Dev on E + Dev on S + Dev on W) / 4`
*   **Correction:** Coefficient A is not corrected by magnets. It is corrected by physically rotating the compass bowl to align the lubber's line correctly.

---

### **Coefficient B**

*   **Explanation:** This is a **Semicircular Coefficient**. It causes maximum deviation on **East** and **West** headings and is zero on North and South headings.
*   **Physical Cause:** It is caused by the interaction of the Earth's magnetic field with the **permanent magnetism in the ship's fore-and-aft direction** and the induced magnetism in vertical soft iron (like funnels or masts).
*   **How to Obtain (Formula):** It is the average of the deviations on East and West (with the sign of the Westerly deviation reversed).
    `B = (Dev on E - Dev on W) / 2`
*   **Correction:** Corrected by placing small permanent magnets in the binnacle in the **fore-and-aft** direction.

---

### **Coefficient C**

*   **Explanation:** This is also a **Semicircular Coefficient**. It causes maximum deviation on **North** and **South** headings and is zero on East and West headings.
*   **Physical Cause:** It is caused by the interaction of the Earth's magnetic field with the **permanent magnetism in the ship's athwartships (side-to-side) direction**.
*   **How to Obtain (Formula):** It is the average of the deviations on North and South (with the sign of the Southerly deviation reversed).
    `C = (Dev on N - Dev on S) / 2`
*   **Correction:** Corrected by placing small permanent magnets in the binnacle in the **athwartships** direction.

---

### **Coefficient D**

*   **Explanation:** This is a **Quadrantal Coefficient**. It is maximum on the intercardinal headings (**NE, SE, SW, NW**) and zero on the cardinal headings (N, E, S, W). It changes sign every 90 degrees.
*   **Physical Cause:** It is caused by **induced magnetism** in the ship's symmetrical horizontal soft iron (e.g., deck beams). This magnetism is induced by the Earth's horizontal magnetic field.
*   **How to Obtain (Formula):** It is the average of the deviations on the intercardinal headings (with the signs of SE and NW deviations reversed).
    `D = (Dev on NE - Dev on SE + Dev on SW - Dev on NW) / 4`
*   **Correction:** Corrected by placing soft iron spheres or cylinders (**Kelvin's Spheres**) on either side of the compass binnacle.

---

### **Coefficient E**

*   **Explanation:** This is also a **Quadrantal Coefficient**. It is maximum on the cardinal headings (**N, E, S, W**) and zero on the intercardinal headings. It is typically very small.
*   **Physical Cause:** It is caused by **induced magnetism** in horizontal soft iron that is arranged **asymmetrically** relative to the compass.
*   **How to Obtain (Formula):** It is the average of the deviations on the cardinal headings (with the signs of E and W deviations reversed).
    `E = (Dev on N - Dev on E + Dev on S - Dev on W) / 4`
*   **Correction:** On most modern vessels, Coefficient E is so small that it is considered negligible and is not corrected. It is left as part of the residual deviation. If it were to be corrected, it would involve slewing (angling) the Kelvin's Spheres.

---

### **Worked Example**

Let's say after swinging the ship, you recorded the following deviations:

| Compass Heading | Deviation (Dev) |
| :-------------- | :---------------- |
| N (000°)        | +2.0° E           |
| NE (045°)       | +5.0° E           |
| E (090°)        | +6.0° E           |
| SE (135°)       | +3.0° E           |
| S (180°)        | -1.0° W           |
| SW (225°)       | -4.0° W           |
| W (270°)        | -5.0° W           |
| NW (315°)       | -2.0° W           |

*(Remember: Easterly = Positive (+), Westerly = Negative (-))*

**Now, let's calculate the coefficients:**

*   **Coefficient A:**
    `A = (+2.0 + 6.0 - 1.0 - 5.0) / 4 = +2.0 / 4 = +0.5°`

*   **Coefficient B:**
    `B = (+6.0 - (-5.0)) / 2 = (+6.0 + 5.0) / 2 = +11.0 / 2 = +5.5°`

*   **Coefficient C:**
    `C = (+2.0 - (-1.0)) / 2 = (+2.0 + 1.0) / 2 = +3.0 / 2 = +1.5°`

*   **Coefficient D:**
    `D = (+5.0 - (+3.0) + (-4.0) - (-2.0)) / 4 = (5 - 3 - 4 + 2) / 4 = 0 / 4 = 0°`
    *(In this example, Coefficient D happens to be zero, which is unlikely in reality but simplifies the math here).*

*   **Coefficient E:**
    `E = (+2.0 - (+6.0) + (-1.0) - (-5.0)) / 4 = (2 - 6 - 1 + 5) / 4 = 0 / 4 = 0°`
    *(Also happens to be zero in this specific example).*

This analysis tells the compass adjuster that there is a small constant error (**A**), a large semicircular error from fore-and-aft magnetism (**B**), and a smaller semicircular error from athwartships magnetism (**C**). They would then use the correctors in the binnacle to reduce B and C as close to zero as possible.