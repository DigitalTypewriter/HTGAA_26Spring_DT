---
title: 'Week 3 HW: Lab Automation'
weight: 10
---
| GUI design                            | Opentron                            |
| ----------------------------------- | ----------------------------------- |
|<img src="well_plate_design.png" width="1000">|<img src="PXL_20260323_200001106.RAW-02.ORIGINAL~3.jpg" width="1000">|

Python Script for Opentrons Artwork
upload the code

Post-Lab Questions
1. Find and describe a published paper that utilizes the Opentrons or an automation tool to achieve novel biological applications.

**Example Paper: [Automated Cell Culture Splitter (ACCS) Using the Opentrons OT‑2](https://www.biorxiv.org/content/10.1101/2024.12.27.629034v1)**
**An example of a novel usage of automation workflow is the Automated Cell Culture Splitter (ACCS), described in a 2024 bioRxiv preprint. The ACCS uses the Opentrons OT‑2 liquid‑handling robot to automate the passaging of both adherent and suspension cells in 96‑well plates.
The system:**
- **<makr>Integrated on‑deck imaging‑based cell counting</mark>**
**The ACCS incorporates a custom imaging module directly on the OT‑2 deck. This module captures images of each well and quantifies cell density using image‑analysis algorithms. In theory, this allows the robot to adjust seeding volumes dynamically through numerical controls, enabling adaptive decision‑making rather than fixed pipetting steps.**
- **<mark>Adaptive, per‑well control of cell numbers</mark>**
**Instead of applying the same dilution to every well, the system uses quantitative imaging data to normalize cell density across wells. The more formal term for “accounting for marginal error through hand‑handling” is error propagation control or error‑aware adaptive pipetting — meaning the automation adjusts for variability introduced by biological noise, pipetting imprecision, or uneven growth.**

2. Write a description about what you intend to do with automation tools for your final project. You may include example pseudocode, Python scripts, 3D printed holders, a plan for how to use Ginkgo Nebula, and more. You may reference this week’s recitation slide deck for lab automation details.

**For my final project, I plan to use lab‑automation tools to streamline the experimental workflow for testing copper‑uptake efficiency in genetically modified Lemna minor. The biological goal is to compare wild‑type plants with engineered lines expressing COPT1, PCS, and an RFP. The automation component focuses on <mark>standardizing liquid handling, exposure conditions, and measurement steps</mark> to ensure reproducibility and high‑throughput data collection.**