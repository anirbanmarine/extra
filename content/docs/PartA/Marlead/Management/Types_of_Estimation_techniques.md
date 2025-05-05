---
title: Types of Estimation Technique
type: docs
toc: true
sidebar:
  open: close
---

**1. PERT (Program Evaluation and Review Technique)**

*   **Focus:** Project scheduling and time estimation, considering uncertainty.
*   **Method:** Uses three estimates for each activity:
    *   **Optimistic (O):** Best-case scenario.
    *   **Most Likely (M):** Most probable duration.
    *   **Pessimistic (P):** Worst-case scenario.
*   **Calculation:**
    *   **Expected Time (TE) = (O + 4M + P) / 6** (weighted average)
    *   **Standard Deviation (SD) = (P - O) / 6** (measure of variability)
*   **Use:** Helps determine the overall project duration and identify critical path activities.
*   **Software:** PERT charts can be created with project management software like Microsoft Project, Primavera P6, and others.

**2. WBS Method (Work Breakdown Structure)**

*   **Focus:** Breaking down a project into smaller, manageable components.
*   **Method:**
    *   Decompose the project into hierarchical levels of tasks and subtasks.
    *   Estimate the effort (time, cost, resources) for each low-level task.
    *   Aggregate the estimates up the hierarchy to get the total project estimate.
*   **Use:** Provides a clear structure for estimation and helps ensure that all work is accounted for.
*   **Relationship to other methods:** WBS can be used in conjunction with other estimation techniques like 3-point estimation or use-case points.

**3. Use-Case Point Method**

*   **Focus:** Estimating software development effort based on the number and complexity of use cases.
*   **Method:**
    *   Identify and define use cases (how users interact with the system).
    *   Classify use cases as simple, average, or complex.
    *   Assign weights to each type of use case.
    *   Calculate the unadjusted use-case points (UUCP).
    *   Consider technical and environmental factors to adjust the UUCP and get the final use-case points.
    *   Use historical data or industry benchmarks to convert use-case points into effort (e.g., person-hours).
*   **Use:** Suitable for object-oriented software development projects.

**4. 3-Point Estimation**

*   **Focus:** Improving estimation accuracy by considering a range of possible outcomes.
*   **Method:** Similar to PERT, it uses three estimates:
    *   **Optimistic (O):** Best-case scenario.
    *   **Most Likely (M):** Most probable duration.
    *   **Pessimistic (P):** Worst-case scenario.
*   **Calculation:**
    *   **Triangular Distribution: TE = (O + M + P) / 3** (simple average)
    *   **Beta Distribution (PERT): TE = (O + 4M + P) / 6** (weighted average)
*   **Use:** Can be applied to various types of projects and activities.

**5. Wideband Delphi Technique**

*   **Focus:** Reaching a consensus among a group of experts on an estimate.
*   **Method:**
    *   A coordinator presents a problem or task to a group of experts.
    *   Experts independently provide their estimates and justifications.
    *   The coordinator summarizes the estimates and provides feedback to the experts.
    *   Experts revise their estimates based on the feedback.
    *   The process is repeated in multiple rounds until a consensus is reached or a satisfactory level of agreement is achieved.
*   **Use:** Useful when there is high uncertainty or when expert judgment is needed.

**Choosing the right estimation technique**

The choice of estimation technique depends on factors such as:

*   **Project phase:** Early phases may require less precise estimates than later phases.
*   **Project type:** Different types of projects may be better suited to different techniques.
*   **Available data:** Some techniques require historical data or expert judgment.
*   **Level of accuracy required:** More complex techniques may provide more accurate estimates but require more effort.

It's often beneficial to use a combination of techniques to get a more comprehensive and reliable estimate.

