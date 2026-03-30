---
title: 'Week 6 HW: Genetic Circuits Part I'
weight: 10
---
## Assignment: DNA Assembly
Answer these questions about the protocol in this week’s lab:
1. What are some components in the Phusion High-Fidelity PCR Master Mix and what is their purpose?
- **High‑fidelity DNA polymerase:**<br>
  **Catalyzes DNA synthesis with very low error rates, ensuring accurate amplification.**
- **dNTPs (deoxynucleotide triphosphates):**<br>
  **Serve as the building blocks incorporated into the newly synthesized DNA strands.**
- **Reaction buffer:**<br>
  **Maintains optimal pH and ionic strength so the polymerase can function efficiently.**
- **Mg²⁺ ions:**<br>
  **Act as an essential cofactor required for polymerase activity and proper primer–template interaction.**
- **Primers:**<br>
  **Short DNA sequences that define the start and end points of the region to be amplified.**

2. What are some factors that determine primer annealing temperature during PCR?

- **Primer length:**<br>
  **Longer primers generally have a higher melting temperature (Tm), which increases the annealing temperature needed for stable binding.
- **GC content:**<br>
  **G–C pairs form three hydrogen bonds (vs. two for A–T), so primers with higher GC content have higher Tm values and require higher annealing temperatures.**
- **Sequence mismatches:**<br>
  **Imperfect complementarity between primer and template lowers the effective Tm, reducing binding stability and lowering the optimal annealing temperature.**
- **Salt concentration (ionic strength):**<br>
  **Higher salt stabilizes DNA duplex formation by shielding negative charges on the phosphate backbone, increasing Tm. Lower salt does the opposite.**

3. There are two methods from this class that create linear fragments of DNA: PCR, and restriction enzyme digests. Compare and contrast these two methods, both in terms of protocol as well as when one may be preferable to use over the other.

**Comparing PCR and Restriction Enzyme Digests for Generating Linear DNA Fragments:**
| Feature      | PCR                    | Restriction Digest        |
| ------------ | ---------------------- | ------------------------- |
| Mechanism    | Uses thermal cycling and a DNA polymerase to amplify a defined region of DNA | Uses restriction endonucleases to cut DNA at specific recognition sequences |
| Requirements | Primers, template DNA, thermostable polymerase, dNTPs, buffer | Purified DNA substrate, restriction enzyme(s), appropriate buffer |
| Output       | A newly synthesized, amplified DNA fragment defined entirely by primer design | Linear fragments produced by cutting at existing restriction sites |
| Flexibility  | Very high — any sequence can be targeted as long as primers can be designed | Limited — only sequences containing the enzyme’s recognition sites can be cut |
|Precision     | Primer design determines exact start and end points; can introduce mutations or add sequences | Extremely precise at known recognition sites but cannot modify sequence |
| Use case     | Creating new fragments, adding tags or mutations, amplifying regions without convenient restriction sites | Opening plasmids, isolating inserts, cloning when restriction sites are already present |

**When to Use Each Method**
- **PCR is preferable when:**
  - **You need to generate a fragment that doesn’t already exist in the plasmid**
  - **You want to add or modify sequences (e.g., tags, overhangs, mutations)**
  - **Restriction sites are absent or inconveniently located**
  - **You need many copies of a specific region**
- **Restriction digests are preferable when:**
  - **You want to cut a plasmid at known, reliable sites**
  - **You’re preparing a vector and insert for cloning using compatible ends**
  - **You need clean, predictable fragment boundaries defined by enzyme recognition sequences**
  - **You want to avoid introducing PCR‑derived mutations**

4. How can you ensure that the DNA sequences that you have digested and PCR-ed will be appropriate for Gibson cloning?

Gibson assembly does not rely on restriction sites — it relies on overlapping homologous ends (typically 20–40 bp). To make sure your fragments are compatible:
- **Add appropriate overlaps:**<br>
  **Design PCR primers that append 20–40 bp of homology to the adjacent fragment or vector. For digested plasmids, ensure the linearized backbone has matching overlap regions.**
- **Confirm correct orientation:**<br>
  **Overlaps must match the sequence direction you want the insert to join. Reverse‑complement overlaps when needed so the insert aligns properly.**
- **Check melting temperatures of overlaps:**<br>
  **Overlap regions should have similar Tm values (usually ≥50–55 °C) to ensure efficient annealing during the Gibson reaction.**
- **Avoid problematic secondary structures:**<br>
  **Screen overlaps for strong hairpins, repeats, or high GC stretches that could interfere with exonuclease chewing or annealing.**
- **Verify sequence accuracy:**<br>
  **Ensure PCR products are clean and correct (no unintended mutations or primer‑dimer artifacts). Confirm that restriction digests fully linearize the vector and remove unwanted fragments.**

5. How does the plasmid DNA enter the E. coli cells during transformation?
6. Describe another assembly method in detail (such as Golden Gate Assembly)
  - Explain the other method in 5 - 7 sentences plus diagrams (either handmade or online).
  - Model this assembly method with Benchling or Asimov Kernel!

## Assignment: Asimov Kernel
1. Create a Repository for your work
2. Create a blank Notebook entry to document the homework and save it to that Repository
3. Explore the devices in the Bacterial Demos Repo to understand how the parts work together by running the Simulator on various examples, following the instructions for the simulator found in the “Info” panel (click the “i” icon on the right to open the Info panel)
4. Create a blank Construct and save it to your Repository
  - Recreate the Repressilator in that empty Construct by using parts from the Characterized Bacterial Parts repository
  - Search the parts using the Search function in the right menu
  - Drag and drop the parts into the Construct
   - Confirm it works as expected by running the Simulator (“play” button) and compare your results with the Repressilator Construct found in the Bacterial Demos repository
  - Document all of this work in your Notebook entry - you can copy the glyph image and the simulator graphs, and paste them into your Notebook
5. Build three of your own Constructs using the parts in the Characterized Bacterials Parts Repo
  - Explain in the Notebook Entry how you think each of the Constructs should function
  - Run the simulator and share your results in the Notebook Entry
  - If the results don’t match your expectations, speculate on why and see if you can adjust the simulator settings to get the expected outcome