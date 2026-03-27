---
title: 'Week 4 HW: Protein Design Part I'
weight: 10
---

Part A: Conceptual Questions
Answer any NINE of the following questions from Shuguang Zhang: (i.e. you can select two to skip)
1. How many molecules of amino acids do you take with a piece of 500 grams of meat? (on average an amino acid is ~100 Daltons)

**<mark>6.022×1023 molecules.</mark> A 500‑gram piece of meat contains about 20% protein, so 500 g×0.20=100 g of protein. Using an average amino acid mass of roughly 100 Daltons (≈100 g/mol), this corresponds to 100 g/100 g/mol=1 mol of amino acids. Since one mole contains 6.022×1023 molecules, eating 500 grams of meat provides on the order of 6×1023 individual amino acid molecules.**

2. Why do humans eat beef but do not become a cow, eat fish but do not become fish?

**Humans don’t turn into cows or fish when we eat them because <mark>digestion breaks biological structures down into their simplest components: proteins are dismantled into amino acids, DNA into nucleotides, and lipids into fatty acids</mark>. Once reduced to these basic molecules, the body discards the original organism’s structure and identity and instead uses the raw materials to build human proteins and cells according to human DNA instructions. In other words, we absorb building blocks, not templates, so eating beef or fish provides nutrients but never transfers the biological “identity” of the organism we consumed.**

3. Why are there only 20 natural amino acids?

**There are 20 standard natural amino acids because biological evolution settled on this set that <mark>balances chemical diversity with genetic simplicity: these amino acids collectively provide a wide range of charges, sizes, polarities, and reactivities, yet they fit efficiently into the constraints of the triplet genetic code and minimize the impact of mutations by assigning similar codons to chemically similar residues</mark>. This set turned out to be chemically versatile enough to support protein folding, catalysis, and all core biochemical functions, while remaining stable, error‑tolerant, and easy for early life to encode and reproduce. Although a few additional amino acids exist, such as selenocysteine, the ~20 canonical ones represent an evolutionarily optimized core toolkit rather than a hard physical limit.**

4. Can you make other non-natural amino acids? Design some new amino acids.

**Yes, you can make non‑natural amino acids by designing new chemical side chains and engineering biological systems to incorporate them, which is a major focus of synthetic biology. Because amino acids are modular—each built from the same backbone but with customizable side chains—we can imagine and create new variants with functions not found in nature. Examples include bulky hydrophobic residues to stabilize protein cores, metal‑binding amino acids with tailored coordination groups, photo‑switchable residues that change shape under light, redox‑active side chains that participate in electron transfer, and rigid helix‑forming amino acids that enforce specific secondary structures. These synthetic designs expand the functional possibilities of proteins far beyond what the natural twenty amino acids can provide.**

5. Where did amino acids come from before enzymes that make them, and before life started?

**Amino acids existed long before enzymes or life itself because they can form through <mark>prebiotic chemistry in environments where simple molecules react under the right energy sources.</mark> Classic experiments like the Miller–Urey spark‑discharge setup demonstrated that electric energy acting on gases such as methane, ammonia, and hydrogen can generate amino acids, and similar reactions could have occurred in Earth’s early atmosphere. Additional natural sources include hydrothermal vents, where mineral‑rich, high‑temperature gradients drive organic synthesis, and meteorites such as carbonaceous chondrites, which deliver a diverse suite of amino acids formed in space. Abiotic pathways like the Strecker synthesis—where aldehydes, ammonia, and cyanide react to form amino acids—operate without biological catalysts, showing that these building blocks of life can arise spontaneously. In short, amino acids predate life, emerging from geochemical and extraterrestrial processes long before enzymes evolved to make them.**

6. If you make an α-helix using D-amino acids, what handedness (right or left) would you expect?

**Natural proteins are built from L‑amino acids, which form right‑handed α‑helices, and this handedness is a direct consequence of the chirality of the backbone. D‑amino acids are the mirror‑image enantiomers of L‑amino acids, so the geometry flips: every stereocenter is mirrored, and the resulting α‑helix becomes left‑handed. In other words, <mark>switching from L‑ to D‑amino acids inverts the chirality of the entire secondary structure, giving you a left‑handed α‑helix rather than the right‑handed form found in nature</mark>.**

7. Can you discover additional helices in proteins?

**You can discover additional helices in proteins because the α‑helix is just one of several helical solutions that polypeptide backbones can adopt. Natural proteins also contain 3₁₀ helices and π‑helices, which are less common but follow the same geometric principle of repeating backbone hydrogen bonds with different spacing and pitch. Beyond biology, synthetic systems such as foldamers and peptoids can form an even wider range of helical structures, showing that helices are a general geometric outcome of constrained backbones rather than something specific to the α‑helix or to natural amino acids.**

8. Why are most molecular helices right-handed?

**Most molecular helices are right‑handed because the <mark>stereochemistry of the monomers (L‑amino acids)</mark> that make up biological polymers imposes geometric and steric constraints that strongly favor a right‑handed twist. The opposite handedness would place substituents in crowded, unfavorable positions, so left‑handed helices in proteins built from L‑amino acids are rare and usually very short.**

9. Why do β-sheets tend to aggregate? What is the driving force for β-sheet aggregation?
10. Why do many amyloid diseases form β-sheets?
        Can you use amyloid β-sheets as materials?
11. Design a β-sheet motif that forms a well-ordered structure.

Part B: Protein Analysis and Visualization
1. Briefly describe the protein you selected and why you selected it.
2. Identify the amino acid sequence of your protein.
        How long is it? What is the most frequent amino acid? You can use this Colab notebook to count the frequency of amino acids.
        How many protein sequence homologs are there for your protein? Hint: Use Uniprot’s BLAST tool to search for homologs.
        Does your protein belong to any protein family?
3. Identify the structure page of your protein in RCSB
        When was the structure solved? Is it a good quality structure? Good quality structure is the one with good resolution. Smaller the better (Resolution: 2.70 Å)
        Are there any other molecules in the solved structure apart from protein?
        Does your protein belong to any structure classification family?
4. Open the structure of your protein in any 3D molecule visualization software:
        PyMol Tutorial Here (hint: ChatGPT is good at PyMol commands)
        Visualize the protein as “cartoon”, “ribbon” and “ball and stick”.
        Color the protein by secondary structure. Does it have more helices or sheets?
        Color the protein by residue type. What can you tell about the distribution of hydrophobic vs hydrophilic residues?
        Visualize the surface of the protein. Does it have any “holes” (aka binding pockets)?

Part C: Using ML-Based Protein Design Tools
C1. Protein Language Modeling
1. Deep Mutational Scans
        Use ESM2 to generate an unsupervised deep mutational scan of your protein based on language model likelihoods.
        Can you explain any particular pattern? (choose a residue and a mutation that stands out)
        (Bonus) Find sequences for which we have experimental scans, and compare the prediction of the language model to experiment.
2. Latent Space Analysis
        Use the provided sequence dataset to embed proteins in reduced dimensionality.
        Analyze the different formed neighborhoods: do they approximate similar proteins?
        Place your protein in the resulting map and explain its position and similarity to its neighbors.

C2. Protein Folding
Folding a protein

    Fold your protein with ESMFold. Do the predicted coordinates match your original structure?
    Try changing the sequence, first try some mutations, then large segments. Is your protein structure resilient to mutations?

C3. Protein Generation
Inverse-Folding a protein: Let’s now use the backbone of your chosen PDB to propose sequence candidates via ProteinMPNN

    Analyze the predicted sequence probabilities and compare the predicted sequence vs the original one.
    Input this sequence into ESMFold and compare the predicted structure to your original.

Part D. Group Brainstorm on Bacteriophage Engineering
1. Find a group of ~3–4 students
2. Read through the Phage Reading material listed under “Reading & Resources” below.
3. Review the Bacteriophage Final Project Goals for engineering the L Protein:
        Increased stability (easiest)
        Higher titers (medium)
        Higher toxicity of lysis protein (hard)
4. Brainstorm Session
        Choose one or two main goals from the list that you think you can address computationally (e.g., “We’ll try to stabilize the lysis protein,” or “We’ll attempt to disrupt its interaction with E. coli DnaJ.”).
        Write a 1-page proposal (bullet points or short paragraphs) describing:
            Which tools/approaches from recitation you propose using (e.g., “Use Protein Language Models to do in silico mutagenesis, then AlphaFold-Multimer to check complexes.”).
            Why do you think those tools might help solve your chosen sub-problem?
            Name one or two potential pitfalls (e.g., “We lack enough training data on phage–bacteria interactions.”).
            Include a schematic of your pipeline.
        This resource may be useful: HTGAA Protein Engineering Tools
5. Each individually put your plan on your HTGAA website
        Include your group’s short plan for engineering a bacteriophage