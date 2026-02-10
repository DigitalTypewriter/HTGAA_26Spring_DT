---
title: 'Week 1 HW: Principles and Practices'
weight: 10
---
| pre-fire                            | post-fire                            |
| ----------------------------------- | ----------------------------------- |
|<img src="lm_prefire_edit.jpg" width="1000">|<img src="post-fire.jpg" width="1000">|

<!-- One of the questions this week asks you to fill in a table; that table is copied here from the course page's markdown
     (https://edit.htgaa.org/2026a-course-pages/webpages.git/src/branch/main/content/weeks/week-01/_index.md?display=source)
     just as a convenience -- you DON'T have to use this to complete your homework!  Any form, format or content which is
     responsive to the question is acceptable (the more creative the better!).

     If you want to use this form, you can fill in the table by putting your scoring for each action between the |  | markers
     for each column; DO NOT enter any newlines between the |  | markers, that starts a new table row right there!
 -->
 ## Week 1 Class Assignment
 1. First, describe a biological engineering application or tool you want to develop and why.

**I want to develop a biologically integrated microsensing tool that can detect heavy metal intoxication in living Lemna minor tissue at the cellular level. This idea grew out of a group project facilitated by Dr. Andrew Scarpelli through the ChiTownBio node, where we demonstrated Lemna minor’s ability to phytoremediate heavy metals using a ceramic kiln burnout process to visualize metal accumulation. While this approach confirmed effective metal uptake, its irreversible thermal processing of the plant tissue to generate a readout, making the method qualitative and not easily scalable. Developing a microsensing system that can read biochemical or protein-level responses in living plant cells would allow for more accurate, non-destructive, and low-cost detection of environmental metal contamination.**

 2. Next, describe one or more governance/policy goals related to ensuring that this application or tool contributes to an “ethical” future, like ensuring non-malfeasance (preventing harm). Break big goals down into two or more specific sub-goals.

**A primary governance goal for this project is to ensure <mark>non-malfeasance and biological safety</mark> in the development of a microsensing tool that interfaces with living Lemna minor tissue to detect heavy metal intoxication. Key sub-goals include establishing risk assessment protocols for exposing living organisms to potentially toxic metal concentrations and ensuring that sensing mechanisms do not exacerbate cellular stress, impair plant viability, or introduce unintended environmental release of contaminants during testing or deployment. Clear system boundaries must also be defined to distinguish biological responses from engineered sensing components, particularly when integrating electronics or materials at the cellular or tissue scale.**

**A second governance goal is to promote <mark>transparency, traceability, and ethical biological use</mark>. Sub-goals include documenting the sourcing, cultivation, and post-use handling of Lemna minor, even though it is a non-engineered organism, and ensuring lifecycle considerations such as responsible disposal and environmental impact are addressed. Additionally, because the sensing output is empirical and interpretive, governance should include standards for public communication to prevent misinterpretation of results, especially in community or environmental decision-making contexts.**

https://www.sciencedirect.com/science/article/pii/S0045653506013361?via%3Dihub

 3. Next, describe at least three different potential governance “actions” by considering the four aspects below (Purpose, Design, Assumptions, Risks of Failure & “Success”).

### Governance Action 1: Strengthened Safety and Containment Protocols for Heavy Metal Research

**This governance action establishes dedicated safety and containment procedures for handling heavy metals in Lemna minor microsensing experiments. Because phytoremediation concentrates metals inside plant tissue, the resulting biomass becomes a hazardous waste stream that must be managed with the same rigor as chemical waste.**

**These protocols would define safe concentration limits, specify engineering controls and PPE, and outline approved disposal pathways for contaminated liquids, plant biomass, and sensing hardware. The action assumes that training and infrastructure vary widely, and that contaminated plant material is often underestimated as a hazard. Formalizing procedures and disposal routes can reduce risk while supporting responsible experimentation.**

### Governance Action 2: Open, Modular Standards for Microsensing Hardware
**This governance action promotes transparency, accessibility, and ethical design by encouraging open standards for the microsensing hardware used with Lemna minor. Many microsensing systems—whether based on small PCBs, flexible circuits, microfabricated electrodes, or other substrates—are developed through proprietary processes that limit reproducibility and prevent external review of design choices that affect biological safety. By contrast, open, modular hardware architectures with publicly available schematics, fabrication files, and material specifications would allow researchers, community labs, and environmental groups to inspect, adapt, and audit the sensing system.**

**The action assumes that openness can improve safety and democratize participation, though it also introduces risks: users with varying levels of expertise may replicate the hardware, and widespread deployment of low‑cost sensors could lead to inconsistent calibration or uneven data quality. Still, by making the sensing system transparent and modular, this governance approach aims for reproducibility, ethical oversight, and broader community engagement.**


 4. Next, score (from 1-3 with, 1 as the best, or n/a) each of your governance actions against your rubric of policy goals. The following is one framework but feel free to make your own:

| Does the option:                                    | Option 1 | Option 2 | Option 3 |
|-----------------------------------------------------|----------|----------|----------|
| **Enhance Biosecurity**                             |          |          |          |
| &bull; By preventing incidents                      |          |          |          |
| &bull; By helping respond                           |          |          |          |
| **Foster Lab Safety**                               |          |          |          |
| &bull; By preventing incident                       |          |          |          |
| &bull; By helping respond                           |          |          |          |
| **Protect the environment**                         |          |          |          |
| &bull; By preventing incidents                      |          |          |          |
| &bull; By helping respond                           |          |          |          |
| **Other considerations**                            |          |          |          |
| &bull; Minimizing costs and burdens to stakeholders |          |          |          |
| &bull; Feasibility?                                 |          |          |          |
| &bull; Not impede research                          |          |          |          |
| &bull; Promote constructive applications            |          |          |          |

5. Last, drawing upon this scoring, describe which governance option, or combination of options, you would prioritize, and why. Outline any trade-offs you considered as well as assumptions and uncertainties.

---
## Week 2 Lecture Prep
### Homework Questions from Professor Jacobson:
1. Nature’s machinery for copying DNA is called polymerase. What is the error rate of polymerase? How does this compare to the length of the human genome. How does biology deal with that discrepancy?
2. How many different ways are there to code (DNA nucleotide code) for an average human protein? In practice what are some of the reasons that all of these different codes don’t work to code for the protein of interest?
### Homework Questions from Dr. LeProust:
1. What’s the most commonly used method for oligo synthesis currently?
2. Why is it difficult to make oligos longer than 200nt via direct synthesis?
3. Why can’t you make a 2000bp gene via direct oligo synthesis?
### Homework Question from George Church: