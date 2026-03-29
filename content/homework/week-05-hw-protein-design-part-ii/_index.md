---
title: 'Week 5 HW: Protein Design Part II'
weight: 10
---
## Part 1: Generate Binders with PepMLM
1. Begin by retrieving the human SOD1 sequence from UniProt (P00441) and introducing the A4V mutation.
2. Using the PepMLM Colab linked from the HuggingFace PepMLM-650M model card:
3. Generate four peptides of length 12 amino acids conditioned on the mutant SOD1 sequence.
4. To your generated list, add the known SOD1-binding peptide FLYRWLPSRRGG for comparison.
5. Record the perplexity scores that indicate PepMLM’s confidence in the binders.

|index|Type|Binder|Pseudo Perplexity|
|---|---|---|---|
|0|Known Binder|FLRYWLPSRRGG|21\.73592494089691|
|1|Generated|AWWPVYVGVKAWRKX|12\.725233370840693|
|2|Generated|AWWGVYTVRYAWAAX|12\.277514856931905|
|3|Generated|AWYPVLVAVYELKAA|20\.11580123195301|
|4|Generated|WWWGPYAAVKELRKK|16\.584271595654002|

**The known SOD1-binding peptide FLYRWLPSRRGG yielded a pseudo-perplexity score of ~21.74, suggesting moderate model confidence. This value provides a baseline for comparing PepMLM-generated peptides, where lower scores would indicate potentially stronger or more compatible binders.**

## Part 2: Evaluate Binders with AlphaFold3
Navigate to the AlphaFold Server: alphafoldserver.com
- For each peptide, submit the mutant SOD1 sequence followed by the peptide sequence as separate chains to model the protein-peptide complex.
- Record the ipTM score and briefly describe where the peptide appears to bind. Does it localize near the N-terminus where A4V sits? Does it engage the β-barrel region or approach the dimer interface? Does it appear surface-bound or partially buried?
- In a short paragraph, describe the ipTM values you observe and whether any PepMLM-generated peptide matches or exceeds the known binder.

<script type="module" src="https://unpkg.com/@google/model-viewer/dist/model-viewer.min.js"></script>
<model-viewer src="797C077560F0F202.glb" auto-rotate camera-controls style="width: 800px; height: 600px;"></model-viewer>

**ipTM = 0.3 (confidence in interaction interface); pTM = 0.81 (confidence in protein fold)**
|Type|Copies|Sequence|
|---|---|---|
|Peptide|1|FLRYWLPSRRGG|
|A4V Mutant SOD1|1|MTVKVVCVLKGDGPVQGIINFEQKESNGPVKVWGSIKGLTEGLHGFHVHEFGDNTAGCTSAGPHFNPLSRKHGGPKDEERHVGDLGNVTADKDGVADVSIEDSVISLSGDHCIIGRTLVVHEKADDLGKGGNEESTKTGNAGSRLACGVIGIAQ|

**The AlphaFold3 prediction yielded an ipTM score of 0.30, indicating low confidence in the peptide–protein interaction, while the pTM score of 0.81 suggests that the overall SOD1 structure is well predicted. This disparity indicates that although the protein fold is reliable, the positioning of the peptide is uncertain and likely does not represent a stable binding interaction.**

## Part 3: Evaluate Properties of Generated Peptides in the PeptiVerse
Structural confidence alone is insufficient for therapeutic development. Using PeptiVerse, let’s evaluate the therapeutic properties of your peptide! For each PepMLM-generated peptide:<br>
Compare these predictions to what you observed structurally with AlphaFold3. In a short paragraph, describe what you see.<br> 
Do peptides with higher ipTM also show stronger predicted affinity?<br>
Are any strong binders predicted to be hemolytic or poorly soluble?<br>
Which peptide best balances predicted binding and therapeutic properties?<br>
Choose one peptide you would advance and justify your decision briefly.<br>

|Input|Property|Prediction|Value|Unit|
|---|---|---|---|---|
|FLRYWLPSRRGG|💧 Solubility|Soluble|1.000|Probability|
|FLRYWLPSRRGG|🩸 Hemolysis|Non-hemolytic|0.039|Probability|
|FLRYWLPSRRGG|🔗 Binding Affinity|Weak binding|5.973|pKd/pKi|
|FLRYWLPSRRGG|📏 Length||12|aa|
|FLRYWLPSRRGG|⚖️ Molecular Weight||1507.7|Da|
|FLRYWLPSRRGG|⚡ Net Charge (pH 7)||2.76||
|FLRYWLPSRRGG|🎯 Isoelectric Point||11.71|pH|
|FLRYWLPSRRGG|💦 Hydrophobicity (GRAVY)||-0.71|GRAVY|

**<mark>The PeptiVerse predictions are consistent with the structural results obtained from AlphaFold3. The peptide FLYRWLPSRRGG was predicted to have weak binding affinity (pKd ≈ 5.97), which aligns with the low ipTM score (~0.30), indicating a lack of strong or specific interaction with mutant SOD1.</mark> AlphaFold3 performs structure-based prediction by modeling the three-dimensional protein–peptide complex and assessing whether a stable binding interface can form, whereas PeptiVerse uses sequence-based modeling to estimate binding affinity from learned statistical patterns without explicitly resolving structure. The agreement between these orthogonal approaches strengthens the conclusion that this peptide is unlikely to be an effective binder.**

**Despite the weak binding, the peptide shows favorable therapeutic properties, including a non-hemolytic profile, indicating low predicted toxicity. This highlights an important trade-off: while the peptide may be safe, it lacks sufficient binding strength to be a strong therapeutic candidate. Overall, no strong correlation between high binding affinity and structural confidence is observed in this case, as both metrics consistently indicate weak interaction.**

## Part 4: Generate Optimized Peptides with moPPIt