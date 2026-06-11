---
title: 'Week 9 HW: Cell Free Systems'
weight: 10
---
Homework Part A: General and Lecturer-Specific Questions
General homework questions
1. Explain the main advantages of cell-free protein synthesis over traditional in vivo methods, specifically in terms of flexibility and control over experimental variables. Name at least two cases where cell-free expression is more beneficial than cell production. 

**Cell‑free systems remove the constraints of living cells, giving researchers direct control over reaction conditions. In terms of flexibility, a cell‑free system allows you to add or remove components—such as DNA, RNA, or proteins—without needing to maintain cell viability, which makes rapid prototyping much easier. In terms of control, cell‑free expression enables precise tuning of transcription and translation rates, as well as the concentrations of enzymes, cofactors, and other reagents.**

**Cell‑free expression is especially beneficial in cases where you want to incorporate non‑natural amino acids, since the open reaction environment allows direct addition of orthogonal tRNAs or modified substrates. It is also advantageous for producing toxic or hard‑to‑express proteins, because there is no living cell to damage and no stress response to interfere with protein synthesis.**

2. Describe the main components of a cell-free expression system and explain the role of each component.

**Four main compoenets of cell-free system:**
I. **Transcription/Translation machinery**<br>
**role: build protein**<br>
**components: Ribosomes / tRNAs / RNA polymerase / Aminoacyl-tRNA synthetases**
II. **Template**<br>
**role: provides the coding sequence**<br>
**components: DNA / mRNA**
III. **Energy system**<br>
**componenets: Adenosine Triphosphate (ATP), Guanosine Triphosphate (GTP)**
IV. **Cofactors + environment**<br>
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

**Three Causes of Low Yield:<br>
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

**One‑sentence pitch:<br>
A portable, freeze‑dried cell‑free test strip that detects copper ions in water and produces a visible color change, serving as a low‑cost sampling kit to guide copper remediation efforts.**

**How the idea works:<br>
Cell‑free transcription/translation reactions are freeze‑dried onto a paper strip or small plastic cartridge, along with a copper‑responsive genetic circuit. When a water sample is applied, the system rehydrates and, if Cu²⁺ is present above a threshold, a copper‑sensing regulator activates expression of a visible reporter such as a chromoprotein or fluorescent protein. The intensity or presence of the color change reflects the copper concentration range, allowing semi‑quantitative readout by eye or with a simple phone app. These test strips can be used in the field to map contamination and decide where to deploy your copper‑sequestering system.**

**Societal challenge or market need:<br>
This addresses the need for accessible, low‑cost, on‑site water quality testing, especially in communities with aging infrastructure, industrial runoff, or limited access to centralized lab facilities. It enables non‑experts—residents, schools, local agencies—to quickly assess whether copper levels may be problematic and to prioritize remediation or further laboratory testing.**

**Addressing limitations of cell‑free reactions:<br>
The cell‑free reactions are freeze‑dried with stabilizers (e.g., trehalose, sugars, polymers) to maintain activity during storage and transport at room temperature. Activation is intentionally one‑time and water‑triggered: the user adds a small volume of water, the reaction runs for a defined time window, and then naturally stops as energy substrates are consumed. Because they are single‑use, the strips are designed to be cheap and disposable, and can be packaged in sealed pouches to extend shelf life. For more advanced versions, you could calibrate the response time or color intensity to approximate copper concentration ranges relevant to health guidelines.**

Homework question from Ally Huang
Freeze-dried cell-free reactions have great potential in space, where resources are constrained. As described in my talk, the Genes in Space competition challenges students to consider how biotechnology, including cell-free reactions, can be used to solve biological problems encountered in space. While the competition is limited to only high school students, your assignment will be to develop your own mock Genes in Space proposal to practice thinking about biotech applications in space!

For this particular assignment, your proposal is required to incorporate the BioBits® cell-free protein expression system, but you may also use the other tools in the Genes in Space toolkit (the miniPCR® thermal cycler and the P51 Molecular Fluorescence Viewer). For more inspiration, check out https://www.genesinspace.org/ .

1. Provide background information that describes the space biology question or challenge you propose to address. Explain why this topic is significant for humanity, relevant for space exploration, and scientifically interesting. (Maximum 100 words)
2. Name the molecular or genetic target that you propose to study. Examples of molecular targets include individual genes and proteins, DNA and RNA sequences, or broader -omics approaches. (Maximum 30 words)
3. Describe how your molecular or genetic target relates to the space biology question or challenge your proposal addresses. (Maximum 100 words)
4. Clearly state your hypothesis or research goal and explain the reasoning behind it. (Maximum 150 words)
5. Outline your experimental plan - identify the sample(s) you will test in your experiment, including any necessary controls, the type of data or measurements that will be collected, etc. (Maximum 100 words)

**Background:<br>
Long‑duration space missions rely on closed‑loop water recycling systems, where even small failures in filtration can lead to the gradual buildup of trace contaminants such as copper ions. Elevated copper can damage cells, disrupt enzymes, and threaten astronaut health, yet current monitoring methods are bulky, slow, or Earth‑dependent. A lightweight, freeze‑dried, cell‑free diagnostic that can be run entirely on‑orbit would provide rapid, on‑demand assessment of water quality. This is significant for safe human habitation in space and scientifically interesting for understanding how closed life‑support systems behave over time.**

**Molecular/genetic target:<br>
A copper‑responsive genetic circuit using a CueR‑regulated promoter driving expression of a fluorescent reporter protein in the BioBits cell‑free system.**

**Target–challenge connection:<br> 
CueR is a copper‑responsive transcription factor that activates gene expression when intracellular copper levels rise. By placing a fluorescent reporter under control of a CueR‑regulated promoter, the BioBits cell‑free system can be engineered to “light up” in response to copper in a water sample. This directly links the molecular target—copper‑regulated transcription—to the space challenge of monitoring trace metal contamination in recycled water. Measuring fluorescence intensity provides a simple, visual readout of copper levels that astronauts could interpret using the P51 Molecular Fluorescence Viewer, without needing complex analytical instruments.**

**Hypothesis / research goal:<br>
A freeze‑dried BioBits cell‑free reaction containing a CueR‑based copper sensor can be rehydrated with spacecraft water samples and produce a fluorescence signal proportional to copper concentration under spaceflight conditions.
The goal is to develop and characterize a compact, on‑orbit assay that allows astronauts to rapidly assess whether copper levels in recycled water remain within safe limits. This is based on prior work showing that cell‑free systems and fluorescent reporters remain functional after freeze‑drying and rehydration, and that metal‑responsive transcription factors can be wired into synthetic gene circuits. Testing this system in microgravity will reveal whether reaction kinetics, diffusion, or mixing affect sensor performance, and whether calibration curves generated on Earth remain valid in space.**

**Experimental plan:<br>
Pepare freeze‑dried BioBits reactions containing the CueR sensor circuit in PCR tubes or paper‑based formats. On‑orbit, astronauts will rehydrate reactions with water samples from the spacecraft recycling system and with defined copper standards as controls (0, low, medium, high). After incubation at a controlled temperature, fluorescence will be measured using the P51 Molecular Fluorescence Viewer and recorded as relative intensity. Negative controls (no DNA, no copper) and positive controls (known copper spike‑ins) will validate specificity and sensitivity. Data will be used to generate a calibration curve and assess the sensor’s usability for routine monitoring.**