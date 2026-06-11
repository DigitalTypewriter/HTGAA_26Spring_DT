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
1. **Transcription/Translation machinery**<br>
**role: build protein**<br>
**components: Ribosomes / tRNAs / RNA polymerase / Aminoacyl-tRNA synthetases**
2. **Template**<br>
**role: provides the coding sequence**<br>
**components: DNA / mRNA**
3. **Energy system**<br>
**componenets: Adenosine Triphosphate (ATP), Guanosine Triphosphate (GTP)**
4. **Cofactors + environment**<br>
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

**Membrane proteins contain strongly hydrophobic transmembrane regions, which makes them prone to aggregation and misfolding when expressed in a purely aqueous cell‑free system. Without a lipid bilayer, these hydrophobic segments have no suitable environment to insert into, leading to precipitation and loss of functional structure. To overcome this, the experiment must supply a membrane‑like environment during translation, typically by adding liposomes or nanodiscs. Liposomes provide closed vesicles with a natural bilayer, while nanodiscs offer small, soluble, well‑defined lipid patches stabilized by scaffold proteins. In both cases, the goal is to allow the nascent protein to insert into a lipid bilayer co‑translationally, preventing aggregation and promoting correct folding.**

**The experiment is set up by adding the chosen membrane mimic directly into the cell‑free reaction before translation begins, ensuring that liposomes or nanodiscs are available for co‑translational insertion as the protein emerges from the ribosome. Incorporation is supported by maintaining the lipid structures in a stable, dispersed state, which is why a very low concentration of mild detergent may be included: it helps keep lipids from clumping, assists in forming uniform membrane mimics, and slightly increases bilayer fluidity to ease insertion—while avoiding the high detergent levels that would disrupt folding. Optimization then focuses on variables such as lipid composition, protein‑to‑lipid ratio, detergent level, and temperature to maximize proper folding, insertion, and functional yield.**

6. Imagine you observe a low yield of your target protein in a cell-free system. Describe three possible reasons for this and suggest a troubleshooting strategy for each.

**3 Causes of Low Yield:<br>
A low yield in a cell‑free expression system can arise from several bottlenecks. One common issue is DNA or template quality: degraded DNA, impurities, or a weak promoter can all reduce transcription efficiency. A second possibility is energy limitation, where ATP or other high‑energy cofactors become depleted during the reaction, slowing or halting protein synthesis. A third major cause is protein instability, where the nascent protein misfolds or is rapidly degraded by endogenous proteases in the extract. Each of these factors can independently or collectively suppress overall protein yield.**

**Troubleshooting Strategies:<br>
To troubleshoot template‑related problems, verify DNA integrity via gel electrophoresis, ensure clean preparation, and consider switching to a stronger promoter or optimizing codon usage. For energy depletion, supplement or upgrade the energy regeneration system, such as adding phosphoenolpyruvate, creatine phosphate, or improved cofactors to maintain ATP levels throughout the reaction. To address protein instability, adjust conditions to favor proper folding—such as lowering the reaction temperature, adding molecular chaperones, or modifying buffer composition—and, if necessary, include protease inhibitors to reduce degradation. Together, these targeted strategies help diagnose and correct the most common causes of low protein yield in cell‑free systems.**

Homework question from Kate Adamala
Design an example of a useful synthetic minimal cell as follows:
1. Pick a function and describe it.
  - What would your synthetic cell do? What is the input and what is the output?
  - Could this function be realized by cell-free Tx/Tl alone, without encapsulation?
  - Could this function be realized by genetically modified natural cell?
  - Describe the desired outcome of your synthetic cell operation.

**Function description: <br>
The synthetic cell is designed to detect, uptake, and sequester copper ions (Cu²⁺) from its environment, converting them into a non‑toxic, chelated complex. The input is extracellular Cu²⁺, and the output is Cu²⁺ bound to phytochelatins inside the vesicle, effectively lowering free copper concentration in the surrounding medium.**

**Cell‑free vs natural cell: <br>
This function cannot be realized by cell‑free transcription/translation alone, because COPT1 is a membrane copper transporter that requires a lipid bilayer and vectorial transport to move Cu⁺/Cu²⁺ across a membrane and accumulate it in a compartment.**

**Desired outcome: <br>
The desired outcome is that, upon exposure to Cu²⁺, the synthetic cell imports copper via COPT1, converts it to a phytochelatin–copper complex via PCS1, and thereby reduces free Cu²⁺ concentration in the environment while safely storing copper inside the vesicle.**

2. Design all components that would need to be part of your synthetic cell.
  - What would be the membrane made of?
  - What would you encapsulate inside? Enzymes, small molecules.
  - Which organism your Tx/Tl system will come from? Is bacterial OK, or do you need a mammalian system for some reason? (hint: for example, if you want to use small molecule modulated promotors, like Tet-ON, you need mammalian)
  - How will your synthetic cell communicate with the environment? (hint: are substrates permeable? or do you need to express the membrane channel?)

**The synthetic cell membrane will be a phospholipid vesicle (liposome) composed primarily of phosphatidylcholine (PC) and phosphatidylethanolamine (PE), with cholesterol added to improve stability and eukaryote‑like membrane properties (fluidity, packing, and robustness). that said with the given objective of the copper-remediation system, the project would benefit from Using a bacterial system, agrobacterium with optimization (e.g., chaperones, membrane mimics, lower temperature) to improve COPT1 folding and insertion altogether.**

3. Experimental details
  - List all lipids and genes. (bonus: find the specific genes; for example, instead of just saying “small molecule membrane channel” pick the actual gene.)
  - How will you measure the function of your system?

**Lipids**
- **Phosphatidylcholine (PC)**
- **Phosphatidylethanolamine (PE)**
- **Cholesterol; for stability**

**Genes**
- **COPT1 (copper transporter from Arabidopsis)**
- **PCS1 (phytochelatin synthase)**
- **RFP (red fluorescent protein)**

**Measurement**
- **Fluorescence (RFP): Confirms that the cell‑free Tx/Tl system is active inside the vesicles and that the genetic program is being executed.**
- **Copper quantification: Use ICP‑MS or a colorimetric copper assay (e.g., bathocuproine or similar) to measure decrease in external Cu²⁺ and/or increase in copper associated with vesicles.**
- **Vesicle loading/association: Separate vesicles from the external medium (e.g., by centrifugation or size‑exclusion chromatography) and measure copper content in the vesicle fraction vs supernatant to confirm uptake and sequestration.**

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