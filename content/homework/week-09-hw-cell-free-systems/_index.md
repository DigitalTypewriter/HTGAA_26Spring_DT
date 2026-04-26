---
title: 'Week 9 HW: Cell Free Systems'
weight: 10
---
Homework Part A: General and Lecturer-Specific Questions
General homework questions
1. Explain the main advantages of cell-free protein synthesis over traditional in vivo methods, specifically in terms of flexibility and control over experimental variables. Name at least two cases where cell-free expression is more beneficial than cell production. 

**Cell-free systems remove cellular constraints, allowing direct control over reaction conditions; in terms of flexibility, in cell-free system, you can directly add/remove componenets (DNA/RNA/proteins) without maintaining cell viability, allowing rapid protytyping.in terms of control, cell-free systems allows fine tunning transcripiton/translation rates, concentration of enzymes (agent/reagent). 
Cell-free system would be benefitical while incorporating non-naturla amino acids, as well as used to synthesize toxic or hard-to-express protein.**

2. Describe the main components of a cell-free expression system and explain the role of each component.

**Four main compoenets of cell-free system:**
- **Transcription/Translation machinery**<br>
**role: build protein**<br>
**components: Ribosomes / tRNAs / RNA polymerase / Aminoacyl-tRNA synthetases**
- **Template**<br>
**role: provides the coding sequence**<br>
**components: DNA / mRNA**
- **Energy system**<br>
**componenets: ATP, GTP / regeneration system**
- **Cofactors + environment**<br>
**role: maintain proper biochemical conditions**<br>
**componenets: amino acids / Salts (Mg<sup>2+</sup>, K<sup>+</sup>) / Buffer**<br>


3. Why is energy provision regeneration critical in cell-free systems? Describe a method you could use to ensure continuous ATP supply in your cell-free experiment.

**Protein synthesis is energy expensive; Translation consumes ATP + GTP rapidly and without regenration, the systems shuts down shortly after in minutes. Alternatives such as Phosphoenolpyruvate (PEP) system or Creatine phosphate system or Glucose-based metabolic regeneration thats with a high-energy substrate is used to regenerate ATP from ADP.**

4. Compare prokaryotic versus eukaryotic cell-free expression systems. Choose a protein to produce in each system and explain why.
| Feature      | Prokaryotic                    | Eukaryotic        |
| ------------ | ---------------------- | ------------------------- |
| speed | fast | slower |
| post-translational modifications | Limited | Extensive |
| cost | cheap | expensive |

5. How would you design a cell-free experiment to optimize the expression of a membrane protein? Discuss the challenges and how you would address them in your setup.

First: identify the challenge
memebrane proteins are hydrophobic which aggregate easily that needs membrane-like envrionemtns.
Second: design solution
want to include Liposomes or nanodiscs (why)

workflow and strucutre:
set up: add lipid environment to reaction
expression strategy: co-translational insertion intor memebrane mimic
optimization variables: lipid composition, detergent concentration, temperature

6. Imagine you observe a low yield of your target protein in a cell-free system. Describe three possible reasons for this and suggest a troubleshooting strategy for each.

Possibility 1: DNA/template issues
cause:
- degraded DNA
- poor promoter
fix:
- check DNA quality
- use stronger promoter
Possibility 2: energy limiation
cause: ATP depletion
fix: improve regenration system
Possibility 3: protein instability
cause: degradation or misfolding
fix:
- add chaperones
- lower temperature
- modify conditions

Homework question from Kate Adamala
Design an example of a useful synthetic minimal cell as follows:
1. Pick a function and describe it.
  - What would your synthetic cell do? What is the input and what is the output?
  - Could this function be realized by cell-free Tx/Tl alone, without encapsulation?
  - Could this function be realized by genetically modified natural cell?
  - Describe the desired outcome of your synthetic cell operation.

To reference back to the final project that im developing along the course, implementing a designed cell-dependent system into a synthetic cell design to achieve the goal.
the functiuon could be described as heavy metal (copper) uptake and sequestration using COPT1 and phytochelatin synthase./a synthetic cell that detects and removes copper ions from its envrionment and sequesters them into a non-toxic complex.
- Cell-free Tx/Tl alone cannot replicate vectorial transport across a membrnace. this function (vectorial transport) cannot be realized by cell-free Tx/Tl alone beause COPT1 is a memnbrane transporter while requires a lipid bilayer. the compartmentalization to accumulate copper
- genetically modified natural cell is exactlty the aim of my final project; a cell that sequester copper with phytochelatin synthase.
- the desire outcome is for Cu<sup>2+</sup> concentration 

2. Design all components that would need to be part of your synthetic cell.
  - What would be the membrane made of?
  - What would you encapsulate inside? Enzymes, small molecules.
  - Which organism your Tx/Tl system will come from? Is bacterial OK, or do you need a mammalian system for some reason? (hint: for example, if you want to use small molecule modulated promotors, like Tet-ON, you need mammalian)
  - How will your synthetic cell communicate with the environment? (hint: are substrates permeable? or do you need to express the membrane channel?)

instead of plant cells, Phospholipid vesicle (liposome) or possibly include cholesterol (if mimicing eukaryotic properties)
- inside the synthetic cells would consist with core componenets like Tx/Tl machinery with COPT1/PCS/RFP DNA encodings while also amino acids, ATP regeneration system and Cofactors (especially Glutathione for PCS as substrate)
- im trying to use E.coli for agrobacterium Tx/Tl system; the trade off is that while bacteria extract is easier, cheaper, faster, but poor at expressing eukaryotic memebrane proteins, which bacterial system might misfold COPT1 plant membrane protein. could switch to a eukaryotic lysate or bacterial with optimization.
- as copper ion sequestered by the organism, we've successfully engineered a synthetic cell that communicate with the environment, to be specific, the copper ions must cross the membrnace and express COPT1 as a memebrance transporter.

3. Experimental details
  - List all lipids and genes. (bonus: find the specific genes; for example, instead of just saying “small molecule membrane channel” pick the actual gene.)
  - How will you measure the function of your system?

Lipids
- Phosphatidylcholine (PC)
- Phosphatidylethanolamine (PE)
- Cholesterol; for stability

Genes
- COPT1 (copper transporter from Arabidopsis)
- PCS1 (phytochelatin synthase)
- RFP (red fluorescent protein)

Measurement
- Fluorescence: RFP expression confirms Tx/Tl activity
- ICP-MS or colorimetric assay: copper quantification
- Vesicle loading

Homework question from Peter Nguyen
Freeze-dried cell-free systems can be incorporated into all kinds of materials as biological sensors or as inducible enzymes to modify the material itself or the surrounding environment. Choose one application field — Architecture, Textiles/Fashion, or Robotics — and propose an application using cell-free systems that are functionally integrated into the material. Answer each of these key questions for your proposal pitch:
  - Write a one-sentence summary pitch sentence describing your concept.
  - How will the idea work, in more detail? Write 3-4 sentences or more.
  - What societal challenge or market need will this address?
  - How do you envision addressing the limitation of cell-free reactions (e.g., activation with water, stability, one-time use)?

Homework question from Ally Huang
Freeze-dried cell-free reactions have great potential in space, where resources are constrained. As described in my talk, the Genes in Space competition challenges students to consider how biotechnology, including cell-free reactions, can be used to solve biological problems encountered in space. While the competition is limited to only high school students, your assignment will be to develop your own mock Genes in Space proposal to practice thinking about biotech applications in space!

For this particular assignment, your proposal is required to incorporate the BioBits® cell-free protein expression system, but you may also use the other tools in the Genes in Space toolkit (the miniPCR® thermal cycler and the P51 Molecular Fluorescence Viewer). For more inspiration, check out https://www.genesinspace.org/ .

1. Provide background information that describes the space biology question or challenge you propose to address. Explain why this topic is significant for humanity, relevant for space exploration, and scientifically interesting. (Maximum 100 words)
2. Name the molecular or genetic target that you propose to study. Examples of molecular targets include individual genes and proteins, DNA and RNA sequences, or broader -omics approaches. (Maximum 30 words)
3. Describe how your molecular or genetic target relates to the space biology question or challenge your proposal addresses. (Maximum 100 words)
4. Clearly state your hypothesis or research goal and explain the reasoning behind it. (Maximum 150 words)
5. Outline your experimental plan - identify the sample(s) you will test in your experiment, including any necessary controls, the type of data or measurements that will be collected, etc. (Maximum 100 words)