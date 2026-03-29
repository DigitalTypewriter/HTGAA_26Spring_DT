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

**ipTM = 0.3; pTM = 0.81**
|Type|Copies|Sequence|
|---|---|---|
|Peptide|1|FLRYWLPSRRGG|
|SOD1|1|MATKAVCVLKGDGPVQGIINFEQKESNGPVKVWGSIKGLTEGLHGFHVHEFGDNTAGCTSAGPHFNPLSRKHGGPKDEERHVGDLGNVTADKDGVADVSIEDSVISLSGDHCIIGRTLVVHEKADDLGKGGNEESTKTGNAGSRLACGVIGIAQ|

**The AlphaFold3 prediction yielded an ipTM score of 0.30, indicating low confidence in the peptide–protein interaction, while the pTM score of 0.81 suggests that the overall SOD1 structure is well predicted. This disparity indicates that although the protein fold is reliable, the positioning of the peptide is uncertain and likely does not represent a stable binding interaction.**

## Part 3: Evaluate Properties of Generated Peptides in the PeptiVerse
## Part 4: Generate Optimized Peptides with moPPIt