---
title: Time Value of Money
type: docs
toc: true
sidebar:
  open: close
---

### Time Value of Money (TVM)

The fundamental principle of the time value of money is that a sum of money is worth more now than the same sum will be worth at a future date due to its earnings potential in the interim. This potential earning capability is often referred to as the **opportunity cost** of not having the money now.

### 1. Future Value (FV)

Future Value is the value of a current asset at a specified date in the future based on an assumed rate of growth.

**Formula:**

$\qquad FV = PV \times (1 + r)^n$

Where:
* $FV$ = Future Value
* $PV$ = Present Value (the initial amount)
* $r$ = Interest rate per period (expressed as a decimal)
* $n$ = Number of periods (e.g., years)

**Example:** If you invest ₹1,000 today at an annual interest rate of 5% for 10 years, the future value would be:

$\qquad FV = 1000 \times (1 + 0.05)^{10} \approx ₹1,628.89$

### 2. Present Value (PV)

Present Value is the current value of a future sum of money or stream of cash flows given a specified rate of return. It's essentially the reverse of future value.

**Formula:**

$\qquad PV = \frac{FV}{(1 + r)^n}$

Where:
* $PV$ = Present Value
* $FV$ = Future Value (the amount to be received in the future)
* $r$ = Discount rate per period (expressed as a decimal)
* $n$ = Number of periods

**Example:** If you are promised to receive ₹1,000 in 5 years, and the discount rate is 8% per year, the present value of that ₹1,000 is:

$\qquad PV = \frac{1000}{(1 + 0.08)^5} \approx ₹680.58$

### 3. Interest Factor

An interest factor is a multiplier used to calculate the future or present value of a single sum or an annuity. It simplifies TVM calculations, especially when using tables (though less common now with calculators and software).

There are various types of interest factors, including:

* **Future Value Interest Factor (FVIF):** $(1 + r)^n$ (used in the future value formula)
* **Present Value Interest Factor (PVIF):** $\frac{1}{(1 + r)^n}$ (used in the present value formula)

You can find these factors in financial tables or calculate them directly using the formulas above.

### 4. Doubling Period

The doubling period is the time it takes for an investment to double in value at a given interest rate, assuming compounding. A common approximation for this is the **Rule of 72**.

**Approximate Formula (Rule of 72):**

$\qquad \text{Doubling Period} \approx \frac{72}{r}$

Where:
* Doubling Period is in years
* $r$ is the annual interest rate (as a percentage, not a decimal)

**More Precise Formula:**

$\qquad \text{Doubling Period} = \frac{\log(2)}{\log(1 + r)}$

Where:
* $r$ is the interest rate per period (as a decimal)
* $\log$ is the logarithm function (can be natural logarithm or base-10, as long as it's consistent)

**Example:** Using the Rule of 72, an investment growing at 8% per year will approximately double in $72 / 8 = 9$ years.

Using the more precise formula:

$\qquad \text{Doubling Period} = \frac{\log(2)}{\log(1 + 0.08)} \approx \frac{0.693}{0.077} \approx 9.01 \text{ years}$

### 5. Annuity

An annuity is a series of equal payments or receipts made at regular intervals over a specified period.

There are two main types of annuities we often consider in TVM:

* **Ordinary Annuity:** Payments occur at the *end* of each period.
* **Annuity Due:** Payments occur at the *beginning* of each period.

**Future Value of an Ordinary Annuity (FVOA):**

$\qquad FVOA = PMT \times \frac{(1 + r)^n - 1}{r}$

Where:
* $FVOA$ = Future Value of the Ordinary Annuity
* $PMT$ = Payment amount per period
* $r$ = Interest rate per period
* $n$ = Number of periods

**Present Value of an Ordinary Annuity (PVOA):**

$\qquad PVOA = PMT \times \frac{1 - (1 + r)^{-n}}{r}$

Where:
* $PVOA$ = Present Value of the Ordinary Annuity
* $PMT$ = Payment amount per period
* $r$ = Discount rate per period
* $n$ = Number of periods

**For an Annuity Due, you simply multiply the formulas for an ordinary annuity by $(1 + r)$:**

$\qquad FVAD = FVOA \times (1 + r) = PMT \times \frac{(1 + r)^n - 1}{r} \times (1 + r)$

$\qquad PVAD = PVOA \times (1 + r) = PMT \times \frac{1 - (1 + r)^{-n}}{r} \times (1 + r)$


