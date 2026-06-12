---
title: 'Week 10 HW: Advanced Imaging & Measurement Technology'
weight: 10
---
Homework: Final Project<br>
For your final project:
  - Please identify at least one (ideally many) aspect(s) of your project that you will measure. It could be the mass or sequence of a protein, the presence, absence, or quantity of a biomarker, etc.
  - Please describe all of the elements you would like to measure, and furthermore describe how you will perform these measurements.
  - What are the technologies you will use (e.g., gel electrophoresis, DNA sequencing, mass spectrometry, etc.)? Describe in detail.

**To evaluate the performance of the engineered system, I will measure three major categories: <mark>construct expression, copper uptake, and copper sequestration</mark>. Construct expression will be monitored through RFP fluorescence linked to the COPT1 cassette, allowing rapid screening of successfully transformed Lemna minor lines. I will verify gene integration using PCR and sequencing and quantify transcriptional activity through RT‑qPCR to confirm expression of COPT1 (and PCS1, if included). Protein‑level confirmation can be obtained using Western blotting with epitope‑tagged constructs.**

**Copper accumulation and sequestration will be assessed by exposing engineered and control wild-type plants to defined Cu²⁺ concentrations, then separating plant tissue from the surrounding water. Copper retained inside plant biomass will be quantified using <mark>ICP‑MS, atomic absorption spectroscopy, or a colorimetric copper assay</mark> after acid digestion of tissue samples. In parallel, I will <mark>collect water samples</mark> from the growth basin at multiple time points to measure how quickly dissolved copper decreases over time. Comparing copper levels in the water phase between engineered plants, wild‑type plants, and no‑plant controls will reveal whether the modified Lemna minor actively reduces environmental copper concentrations.**

**If PCS1 or other sequestration machinery is included, I will additionally measure phytochelatin or thiol production using <mark>HPLC or LC‑MS</mark> to confirm biochemical binding of copper inside the plant. Growth and viability assays under copper stress will help determine whether sequestration reduces toxicity. Together, these measurements create a complete monitoring pipeline: <mark>RFP for screening, molecular assays for expression, tissue‑level copper quantification for uptake, and water‑phase copper testing for environmental cleanup performance,</mark> providing an evaluation of both copper accumulation and remediation efficiency.**

Homework: Waters Part I — Molecular Weight<br>
1. Based on the predicted amino acid sequence of eGFP (see below) and any known modifications, what is the calculated molecular weight?


**With eGFP, the full construct contains 246 amino acids; using the standard approximation of 110 Da per amino acid, the estimated molecular weight is 246 × 110 Da ≈ 27,060 Da, or roughly 27 kDa. The theoretical molecular weight calculated by online tools is 28,006.60 Da (≈28 kDa), which is consistent with the rough estimate of 246 aa × 110 Da ≈ 27,060 Da.**

2. Calculate the molecular weight of the eGFP using the adjacent charge state approach described in the recitation. Select two charge states from the intact LC-MS data (Figure 1) and:


- Determine for each adjacent pair of peaks

**<mark>z= 966.0390/1000.4302−966.0390 = 966.0390/34.3912 ≈ 28</mark>**

- Determine the MW of the protein using the relationship between m/Zn, MW, and z

**Molecular Weight Calculation Using Charge State z**
  
**For a given charge state z, the relationship between molecular weight MW and the observed m/z is:**<br>
<mark>**m/z = (MW+z)/z**</mark><br>
**rearragne to solve for MW:**<br>
<mark>**MW = (m/z)*z-z</mark>**<br>
**using the peak at m/z = 1000.4302 and z = 28**<br>
<mark>**MW = 1000.4302*28-28 ≈ 28012.046−28 ≈ 27,984 Da**</mark>

**So the protein’s molecular weight from this charge state is ≈27,984 Da (≈28.0 kDa), in excellent agreement with the theoretical ~28,006.6 Da.**

- Calculate the accuracy of the measurement using the deconvoluted MW from 2.2 and the predicted weight of the protein

**The measurement is off by about −0.081%, meaning your experimental mass is extremely close to the theoretical value — well within typical intact‑protein LC‑MS accuracy.**

- Can you observe the charge state for the zoomed-in peak in the mass spectrum for the intact eGFP? If yes, what is it? If no, why not?

**You generally cannot determine the charge state from the zoomed‑in intact eGFP peak, because the zoom only shows a single broad peak without either of the two features needed to assign a charge state: adjacent charge‑state peaks or resolved isotopic spacing. Charge states are identified by comparing neighboring peaks in the charge envelope or by measuring the spacing between isotopes (which is 1/z), and neither of those patterns is visible when only one isolated peak is shown. Without that structural context, the zoomed‑in view does not provide enough information to confidently assign a charge state.**

Homework: Waters Part II — Secondary/Tertiary structure<br>
Homework: Waters Part III — Peptide Mapping - primary structure<br>
1. How many Lysines (K) and Arginines (R) are in eGFP?
**I counted 20 Lysines (K) and 6 Arginines (R).**
2. How many peptides will be generated from tryptic digestion of eGFP?
**Using the Expasy website, it output a table of 19 peptides that >500 Dalton.**
3. Based on the LC-MS data for the Peptide Map data generated in lab (please use Figure 5a as a reference) how many chromatographic peaks do you see in the eGFP peptide map between 0.5 and 6 minutes? You may count all peaks that are >10% relative abundance.
**I counted 19 peaks that >10% abudance at above 1.2e6.**
4. Assuming all the peaks are peptides, does the number of peaks match the number of peptides predicted from question 2 above? Are there more peaks in the chromatogram or fewer?
**The peaks does match with the Expasy prediction with 19 being the total count.**
5. Identify the mass-to-charge of the peptide shown in Figure 5b. What is the charge of the most abundant charge state of the peptide (use the separation of the isotopes to determine the charge state). Calculate the mass of the singly charged form of the peptide.
- **Most abundant isotopic peak (m/z): 525.76712**
- **Isotope spacing between adjacent peaks Δ(m/z): 526.27−525.77 ≈ 0.50 m/z → z = 2⁺**
- **Singly charged peptide mass [M+H]⁺: 2*525.76712 − 1.0073 ≈ 1050.53Da**
6. Identify the peptide based on comparison to expected masses in the PeptideMass tool. What is mass accuracy of measurement? Please calculate the error in ppm.
- **Measured [M+H]⁺ mass: 1050.5300 Da**
- **Closest theoretical mass (from PeptideMass): 1050.5214 Da**<br>
**Mass error: Δ𝑚 = 1050.5300−1050.5214 = 0.0086 Da**<br>
**Mass accuracy: ppm error = Δ𝑚/𝑚<sub>theoretical</sub>×10<sup>6</sup> ≈ 8.18 ppm**<br>
7. What is the percentage of the sequence that is confirmed by peptide mapping? (see Figure 6)<br>
**88%**<br>
Homework: Waters Part IV — Oligomers<br>
Homework: Waters Part V — Did I make GFP?<br>