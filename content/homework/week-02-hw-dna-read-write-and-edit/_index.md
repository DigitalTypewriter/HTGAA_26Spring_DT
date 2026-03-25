---
title: 'Week 2 HW: DNA Read, Write, & Edit'
weight: 10
---

## Part 1: Benchling & In-silico Gel Art<br>
<img src="virtual_digest_sequence_lambda.png" width="400"><br>
## Part 2: Gel Art - Restriction Digests and Gel Electrophoresis

please visit the week2-lab page here: [pages.htgaa.org/2026a/daniel-tseng/labs/week-02-lab-dna-gel-art/](http://pages.htgaa.org/2026a/daniel-tseng/labs/week-02-lab-dna-gel-art/)

## Part 3: DNA Design Challenge

3.1. Choose your protein.

**I chose the protein <mark>Copper Transporter 1 (COPT1)</mark> from Arabidopsis thaliana (UniProt ID: COPT1_ARATH). This protein functions as a membrane transporter responsible for copper uptake in plants. Copper is an essential micronutrient required for many cellular processes, including photosynthesis and enzyme activity, but it can also become toxic at high concentrations. Because of this, organisms require specialized transport proteins such as COPT1 to regulate copper uptake and maintain homeostasis.**

**I am interested in this protein because it is related to a research project I am developing involving the aquatic plant Lemna minor (duckweed). In this project, I am exploring whether introducing or increasing the expression of the copper uptake gene COPT1 could potentially enhance copper uptake in Lemna minor compared to the wild type. This could have implications for phytoremediation, where plants are used to remove heavy metals from contaminated water.**

**To obtain the protein sequence, I searched for COPT1_ARATH on the UniProt database. The amino acid sequence for the COPT1 protein was copied directly from the UniProt entry and is provided below.**

<p><span class="copy-to-clipboard" dir="auto"><code class="copy-to-clipboard-code highlight" data-code="&gt;sp|Q39065|COPT1_ARATH Copper transporter 1 OS=Arabidopsis thaliana OX=3702 GN=COPT1 PE=2 SV=2
MDHDHMHGMPRPSSSSSSSPSSMMNNGSMNEGGGHHHMKMMMHMTFFWGKNTEVLFSGWP
GTSSGMYALCLIFVFFLAVLTEWLAHSSLLRGSTGDSANRAAGLIQTAVYTLRIGLAYLV
MLAVMSFNAGVFLVALAGHAVGFMLFGSQTFRNTSDDRKTNYVPPSGCAC">&gt;sp|Q39065|COPT1_ARATH Copper transporter 1 OS=Arabidopsis thaliana OX=3702 GN=COPT1 PE=2 SV=2
MDHDHMHGMPRPSSSSSSSPSSMMNNGSMNEGGGHHHMKMMMHMTFFWGKNTEVLFSGWP
GTSSGMYALCLIFVFFLAVLTEWLAHSSLLRGSTGDSANRAAGLIQTAVYTLRIGLAYLV
MLAVMSFNAGVFLVALAGHAVGFMLFGSQTFRNTSDDRKTNYVPPSGCAC</code><span class="btn cstyle inline-copy-to-clipboard-button inline notitle interactive"><button type="button" title="Copy text to clipboard"><i class="fa-fw far fa-copy"></i></button></span></span></p>

3.2. Reverse Translate: Protein (amino acid) sequence to DNA (nucleotide) sequence.

><p>COPT1-ARATH Protein Reverse-translated DNA sequence<br><span class="copy-to-clipboard" dir="auto"><code class="copy-to-clipboard-code highlight" data-code="atggatcatgaccatatgcacatgggtatgccgcggccgtcttcttcttcttcttcttcttctccgtcttctatgatgaacaacggttctatgaacgaaggtggtggtcaccaccacatgaaaatgatgatgcacatgacctttttctggggtaaaaacacggaagtgctgttctctggctggccaggcacctcttctggtatgtacgccctgtgtctcatcttcgtcttcttcttggccgtgctgacggaatggctggcgcactcttctctgctgcggggttctactggtgactctgcgaaccgtgcggctgggcttatccaaactgcggtgtacactctgcgtattggcctggcctacgtgctgatggttctggcggtgatgagctttaacgccggtgtgtttctggtggccctggccggtcatgcggtgggtttcatgctgttcggctcccaaaccttccgtaacacctctgatgatcggaagacgaactacgtgccgccatctggttgtgcctgt">atggatcatgaccatatgcacatgggtatgccgcggccgtcttcttcttcttcttcttcttctccgtcttctatgatgaacaacggttctatgaacgaaggtggtggtcaccaccacatgaaaatgatgatgcacatgacctttttctggggtaaaaacacggaagtgctgttctctggctggccaggcacctcttctggtatgtacgccctgtgtctcatcttcgtcttcttcttggccgtgctgacggaatggctggcgcactcttctctgctgcggggttctactggtgactctgcgaaccgtgcggctgggcttatccaaactgcggtgtacactctgcgtattggcctggcctacgtgctgatggttctggcggtgatgagctttaacgccggtgtgtttctggtggccctggccggtcatgcggtgggtttcatgctgttcggctcccaaaccttccgtaacacctctgatgatcggaagacgaactacgtgccgccatctggttgtgcctgt</code><span class="btn cstyle inline-copy-to-clipboard-button inline notitle interactive"><button type="button" title="Copy text to clipboard"><i class="fa-fw far fa-copy"></i></button></span></span></p>

**Because of the <mark>degeneracy of the genetic code</mark>, multiple DNA sequences can encode the same protein sequence. Therefore, the reverse-translated DNA sequence shown above represents only one possible nucleotide sequence that could encode the protein. For the next step, the sequence would often be codon-optimized for the host organism, Lemna minor, to improve gene expression.**

3.3. Codon optimization.

**Codon optimization is necessary because of the <mark>degeneracy of the genetic code</mark>. A single amino acid can be encoded by multiple different codons (DNA sequences). Even though these codons produce the same amino acid, different organisms tend to prefer certain codons over others due to differences in tRNA abundance and translation efficiency.**

**Therefore, once the desired protein sequence is known, the next step is to determine a DNA coding sequence that matches the codon usage preference of the host organism. Codon usage tables provide information about which codons are most frequently used in a particular organism. By selecting codons that are more commonly used in the host organism, the likelihood of efficient protein translation and higher expression levels can be improved.**

**For this project, the codon sequence was optimized for Lemna minor (duckweed). This organism was chosen because the goal of the project is to introduce and express the copper transporter protein COPT1 in Lemna minor in order to potentially enhance copper uptake compared to the wild type. Optimizing the codon usage for Lemna minor increases the chance that the plant’s cellular machinery will efficiently translate the gene and produce the desired protein.**

Lemna minor [gbpln]: 4 CDS's (1597 codons) <br>
fields: [triplet] [frequency: per thousand] ([number]) 
<pre>
UUU 17.5(    28)  UCU 13.8(    22)  UAU  8.8(    14)  UGU  5.0(     8)
UUC 36.3(    58)  UCC 17.5(    28)  UAC 15.7(    25)  UGC 14.4(    23)
UUA  5.6(     9)  UCA 14.4(    23)  UAA  0.0(     0)  UGA  1.9(     3)
UUG 13.8(    22)  UCG 13.8(    22)  UAG  0.6(     1)  UGG 16.3(    26)

CUU 15.7(    25)  CCU 11.9(    19)  CAU  6.9(    11)  CGU  4.4(     7)
CUC 25.7(    41)  CCC 15.7(    25)  CAC 16.9(    27)  CGC 18.2(    29)
CUA  5.0(     8)  CCA 11.3(    18)  CAA 10.0(    16)  CGA  6.3(    10)
CUG 21.3(    34)  CCG 14.4(    23)  CAG 22.5(    36)  CGG 10.6(    17)

AUU 18.8(    30)  ACU  9.4(    15)  AAU 13.8(    22)  AGU 10.0(    16)
AUC 19.4(    31)  ACC 17.5(    28)  AAC 21.9(    35)  AGC 15.0(    24)
AUA  1.9(     3)  ACA  5.0(     8)  AAA 15.7(    25)  AGA 20.7(    33)
AUG 20.7(    33)  ACG 10.0(    16)  AAG 35.7(    57)  AGG 17.5(    28)

GUU 15.0(    24)  GCU 25.0(    40)  GAU 20.0(    32)  GGU  8.1(    13)
GUC 25.0(    40)  GCC 22.5(    36)  GAC 26.3(    42)  GGC 21.9(    35)
GUA  6.3(    10)  GCA 14.4(    23)  GAA 26.3(    42)  GGA 16.9(    27)
GUG 30.7(    49)  GCG 18.2(    29)  GAG 40.1(    64)  GGG 18.2(    29)
</pre>
https://www.kazusa.or.jp/codon/cgi-bin/showcodon.cgi?species=4472

3.4. You have a sequence! Now what?

**For this project, I would use a cell-dependent, plant-based expression system to produce the target proteins in Lemna minor. Specifically, I would use Agrobacterium-mediated transformation, a common method for introducing foreign DNA into plant cells.**

**First, the DNA sequences encoding <mark>COPT1, phytochelatin synthase(PCS), and a red fluorescent protein (RFP)</mark> reporter would be inserted into a plant expression plasmid using molecular cloning techniques such as restriction enzyme digestion and ligation (or Gibson assembly). The construct would include <mark>multiple expression cassettes: a CaMV 35S promoter driving COPT1 to enhance copper uptake, a second promoter (such as ubiquitin or CaMV 35S) driving phytochelatin synthase (PCS) to facilitate heavy metal sequestration, and an RFP reporter gene for visualization.</mark> Each gene would be followed by a suitable terminator such as the NOS terminator, along with a selectable marker gene to identify successfully transformed cells. The recombinant plasmid is then introduced into Agrobacterium tumefaciens, a soil bacterium naturally capable of transferring DNA into plant cells.**

**During Agrobacterium-mediated transformation, the bacterium attaches to plant tissue and transfers a specific region of its plasmid, known as T-DNA, into the plant cell. The engineered genes are placed within this T-DNA region, allowing them to be delivered into the plant cell and, in many cases, integrated into the plant genome. This enables stable expression of all introduced genes in Lemna minor. Once inside the plant cell, the introduced DNA is transcribed into messenger RNA (mRNA) by the plant’s RNA polymerase. The mRNA is then translated by ribosomes into their respective proteins, with each codon specifying an amino acid in the growing polypeptide chains.**

## Part 5 DNA Read/Write/Edit

5.1 DNA Read
(i) What DNA would you want to sequence (e.g., read) and why?

**For the Lemna minor project, I would sequence:**
- **The <mark>engineered plasmid</mark> containing codon‑optimized COPT1, PCS, and RFP to confirm the construct is correct before transformation.**
- **The <mark>T‑DNA insertion region</mark> in transformed Lemna minor to verify that the entire expression cassette integrated properly and without rearrangements.**
- **<mark>Flanking genomic regions</mark> to confirm insertion site(s) and rule out unintended mutations.**<br>
**These sequencing is to ensure that the introduced COPT1 gene is intact, correctly optimized, and stably integrated—critical for evaluating copper‑uptake phenotypes.**

(ii) In lecture, a variety of sequencing technologies were mentioned. What technology or technologies would you use to perform sequencing on your DNA and why?
Also answer the following questions:
    Is your method first-, second- or third-generation or other? How so?
    What is your input? How do you prepare your input (e.g. fragmentation, adapter ligation, PCR)? List the essential steps.
    What are the essential steps of your chosen sequencing technology, how does it decode the bases of your DNA sample (base calling)?
    What is the output of your chosen sequencing technology?
    
**I would use a hybrid approach of both <mark>Illumina Sequencing (2nd) & Oxford Nanopore Sequencing (3rd)</mark>:**

**<mark>Illumina Sequencing (Second‑Generation)</mark>**
- **Why: High accuracy for confirming the exact nucleotide sequence of the plasmid and transgene.**
- **How it works: Sequencing‑by‑synthesis with fluorescently labeled nucleotides; optical detection produces short reads (50–300 bp).**
- **Input & preparation: Extracted DNA → fragmentation → adapter ligation → cluster amplification.**
- **Output: Millions of short, accurate reads ideal for mutation checking.**
- **Project: Ensures the codon‑optimized COPT1 sequence is error‑free.**

**<mark>Oxford Nanopore Sequencing (Third‑Generation)</mark>**
- **Why: Long reads allow full T‑DNA insertion mapping in Lemna minor.**
- **How it works: DNA passes through a nanopore; current disruptions correspond to nucleotide patterns.**
- **Input & preparation: High‑molecular‑weight DNA with ligated adapters.**
- **Output: Long reads (kb–Mb) ideal for structural verification.**
- **Project: Confirms that the entire COPT1/PCS/RFP cassette integrated as a single, intact unit.**

**Citations:**<br>
    Goodwin et al., Nat Rev Genet (2016) – overview of sequencing generations.<br>
    Heather & Chain, Genome Biology (2016) – Illumina workflow.<br>
    Jain et al., Nat Biotechnol (2016) – Nanopore long‑read sequencing.<br>

5.2 DNA Write
(i) What DNA would you want to synthesize (e.g., write) and why?<br>

**I would synthesize:**<br>
- **The <mark>codon‑optimized COPT1 gene</mark> tailored for Lemna minor codon usage.**
- **<mark>PCS and RFP coding sequences</mark>**
- **<mark>Regulatory elements (promoters, terminators)</mark>**
- **The <mark>full multi‑gene expression cassette</mark>, if ordered as a single synthetic construct.**<br>

(ii) What technology or technologies would you use to perform this DNA synthesis and why?
Also answer the following questions:
    What are the essential steps of your chosen sequencing methods?
    What are the limitations of your sequencing method (if any) in terms of speed, accuracy, scalability?<br>

**Commercial DNA Synthesis (Phosphoramidite Chemistry + Enzymatic Assembly)**<br>
- **Why: Industry standard for accurate, customizable gene synthesis.**
- **Essential steps: Chemical synthesis of short oligos -> Purification -> Enzymatic assembly into full genes -> Sequence verification**
- **Limitations:**
  - **Length constraints (long constructs require assembly)**
  - **Slower turnaround time**
  - **Cost increases with size and complexity**

**Citations:**<br>
    Kosuri & Church, Nat Methods (2014) – gene synthesis technologies.<br>
    Beaucage & Caruthers, Tetrahedron (1981) – phosphoramidite chemistry.<br>

5.3 DNA Edit
(i) What DNA would you want to edit and why?<br>

**I would edit:**<br>
- **The <mark>Lemna minor genome</mark> to insert the COPT1/PCS/RFP expression cassette for stable transgenic lines.**
- **Optionally, <mark>endogenous copper‑transport genes</mark> to study synergistic or compensatory effects.**
**This allows direct testing of whether COPT1 overexpression enhances copper uptake.**<br>

(ii) What technology or technologies would you use to perform these DNA edits and why?
Also answer the following questions:
    How does your technology of choice edit DNA? What are the essential steps?
    What preparation do you need to do (e.g. design steps) and what is the input (e.g. DNA template, enzymes, plasmids, primers, guides, cells) for the editing?
    What are the limitations of your editing methods (if any) in terms of efficiency or precision?<br>
**<mark>CRISPR‑Cas9</mark> would be used for genome editing because it enables targeted modifications in plant genomes, including insertions, deletions, and gene replacements. In this project, CRISPR‑Cas9 conceptually allows insertion of the codon‑optimized COPT1/PCS/RFP cassette into the Lemna minor genome.**<br>
**The system uses a guide RNA (gRNA) that directs the Cas9 nuclease to a specific genomic sequence, where Cas9 introduces a double‑strand break. The plant repairs this break either through non‑homologous end joining (NHEJ), which produces small insertions or deletions and can knock out genes, or through homology‑directed repair (HDR) if a donor DNA template is provided, enabling precise insertion of the engineered COPT1 cassette. Inputs include the gRNA design, a Cas9 expression cassette, donor DNA for HDR, and plant tissue.**<br>
**Limitations include low HDR efficiency in plants, potential off‑target edits, and the need to screen many plants to identify those with the correct genomic modification.**