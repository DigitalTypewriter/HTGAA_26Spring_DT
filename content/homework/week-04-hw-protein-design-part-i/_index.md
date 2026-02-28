---
title: 'Week 4 HW: Protein Design Part I'
weight: 10
---

Part A: Conceptual Questions
Answer any NINE of the following questions from Shuguang Zhang: (i.e. you can select two to skip)
1. How many molecules of amino acids do you take with a piece of 500 grams of meat? (on average an amino acid is ~100 Daltons)
2. Why do humans eat beef but do not become a cow, eat fish but do not become fish?
3. Why are there only 20 natural amino acids?
4. Can you make other non-natural amino acids? Design some new amino acids.
5. Where did amino acids come from before enzymes that make them, and before life started?
6. If you make an α-helix using D-amino acids, what handedness (right or left) would you expect?
7. Can you discover additional helices in proteins?
8. Why are most molecular helices right-handed?
9. Why do β-sheets tend to aggregate?
        What is the driving force for β-sheet aggregation?
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