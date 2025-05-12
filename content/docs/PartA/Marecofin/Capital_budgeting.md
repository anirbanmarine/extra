---
title: Capital budgeting
type: docs
toc: true
math: true
sidebar:
  open: close
---

### Capital Budgeting: Deciding Whether to Invest

Capital budgeting is the process companies use for decision-making on capital projects – those projects with a life of a year or more. It helps determine whether a project is worth pursuing based on its potential profitability and risk.

### Discounted Cash Flow (DCF) Criteria

DCF techniques consider the **time value of money**, meaning that a rupee received today is worth more than a rupee received in the future due to its potential earning capacity. These methods discount future cash flows back to their present value.

Here are the primary DCF criteria used to decide on project investments:

#### 1. Net Present Value (NPV)

NPV calculates the present value of all expected future cash inflows minus the present value of all expected future cash outflows of a project.

**Formula:**

$\qquad NPV = \sum_{t=0}^{n} \frac{CF_t}{(1 + r)^t}$

Where:
* $NPV$ = Net Present Value
* $CF_t$ = Cash flow at time $t$ (CF₀ is usually the initial investment and is negative)
* $r$ = Discount rate (cost of capital)
* $n$ = Number of periods

**Decision Rule:**

* If $NPV > 0$: **Accept** the project. It is expected to add value to the firm.
* If $NPV < 0$: **Reject** the project. It is expected to decrease the firm's value.
* If $NPV = 0$: The project is neither adding nor destroying value. Acceptance might depend on other factors.

#### 2. Internal Rate of Return (IRR)

IRR is the discount rate at which the NPV of a project equals zero. It represents the effective rate of return a project is expected to yield.

**Formula:**

The IRR is the value of $r$ that satisfies the following equation:

$\qquad 0 = \sum_{t=0}^{n} \frac{CF_t}{(1 + IRR)^t}$

This formula is typically solved using financial calculators or spreadsheet software.

**Decision Rule:**

* If $IRR > \text{Cost of Capital (r)}$: **Accept** the project. The project's return exceeds the required rate of return.
* If $IRR < \text{Cost of Capital (r)}$: **Reject** the project. The project's return is less than the required rate of return.
* If $IRR = \text{Cost of Capital (r)}$: Acceptance is marginal and might depend on other factors.

#### 3. Profitability Index (PI)

The Profitability Index (also known as the Benefit-Cost Ratio) measures the present value of the future cash flows relative to the initial investment.

**Formula:**

$\qquad PI = \frac{\sum_{t=1}^{n} \frac{CF_t}{(1 + r)^t}}{|CF_0|}$

Where:
* $PI$ = Profitability Index
* $\sum_{t=1}^{n} \frac{CF_t}{(1 + r)^t}$ = Present value of future cash inflows
* $|CF_0|$ = Absolute value of the initial investment (cash outflow at time 0)

**Decision Rule:**

* If $PI > 1$: **Accept** the project. The present value of benefits is greater than the cost.
* If $PI < 1$: **Reject** the project. The present value of benefits is less than the cost.
* If $PI = 1$: The present value of benefits equals the cost. Acceptance might depend on other factors.

### Non-Discounted Cash Flow Criteria

Non-discounted cash flow techniques **do not consider the time value of money**. They are simpler to calculate but may not provide as accurate a picture of a project's profitability, especially for long-term projects.

Here are the primary non-discounted cash flow criteria:

#### 1. Payback Period (PB)

The payback period is the number of years it takes for a project to recover its initial investment from the cumulative cash inflows.

**Calculation:**

* **For projects with equal annual cash flows:**
    $\qquad \text{Payback Period} = \frac{\text{Initial Investment}}{\text{Annual Cash Inflow}}$

* **For projects with unequal annual cash flows:** The payback period is determined by adding up the cash inflows year by year until the initial investment is recovered.

**Decision Rule:**

* If the payback period is **less than** a predetermined target period: **Accept** the project.
* If the payback period is **greater than** a predetermined target period: **Reject** the project.

**Limitations:** This method ignores the time value of money and cash flows occurring after the payback period.

#### 2. Accounting Rate of Return (ARR)

The Accounting Rate of Return (also known as the Average Rate of Return) is the average annual profit after tax divided by the average investment.

**Formula:**

$\qquad ARR = \frac{\text{Average Annual Profit After Tax}}{\text{Average Investment}}$

Where:
* Average Investment is often calculated as (Initial Investment + Salvage Value) / 2.

**Decision Rule:**

* If $ARR$ is **greater than** a predetermined target rate of return: **Accept** the project.
* If $ARR$ is **less than** a predetermined target rate of return: **Reject** the project.

**Limitations:** This method is based on accounting profits rather than cash flows and ignores the time value of money.

### Which Criteria to Use?

While non-discounted methods are simpler, **Discounted Cash Flow (DCF) methods are generally preferred** for capital budgeting decisions because they account for the time value of money and provide a more accurate assessment of a project's economic viability.

* **NPV** is often considered the most reliable method as it directly measures the value a project adds to the firm.
* **IRR** is also popular but can have issues with mutually exclusive projects or projects with non-conventional cash flows (multiple sign changes).
* **PI** is useful for ranking projects, especially when there are capital constraints.
* Non-discounted methods like **Payback Period** can provide a quick measure of liquidity and risk but should not be the sole basis for long-term investment decisions. **ARR** is also limited due to its reliance on accounting profits and neglect of the time value of money.

In practice, companies often use a combination of these methods to get a comprehensive view of a project's potential before making an investment decision.
