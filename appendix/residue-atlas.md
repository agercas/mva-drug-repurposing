# BubR1 residue atlas and ligandability census

BubR1 is a 1,050-residue scaffold protein of the spindle assembly checkpoint, the mechanism that delays chromosome separation until every chromosome is attached to the spindle. The residue atlas is a table that scores 32 regions of the protein on structure, function, regulation and disease-variant coverage, with 42 residue-resolved sites beneath them. A count of the experimental structures and a review of recorded ligand data (a test of ligandability, the capacity to bind a small molecule) sit beside it.

The results are a screening bar of 9.67 µM (the strongest recorded potency, which a new screen must beat) and a ranking of restoration designs by the number of unmeasured premises (statements on which a design fails if false) each needs.

## Findings

1. **Knowledge concentrates on the half of BubR1 that C-terminal disease alleles leave intact.** The best-understood regions are the 18-residue domain that docks the phosphatase PP2A-B56 (protein phosphatase 2A with its B56 subunit), the tetratricopeptide-repeat domain (a protein-binding module) and the two KEN boxes (degradation signals). The pseudokinase C-lobe (the C-terminal part of the kinase-like domain) scores high only because it carries every patient allele that has been measured. Seventeen of 32 regions score 2 or less on a 12-point scale.

2. **The human pseudokinase domain has no experimental structure.** Nine Protein Data Bank entries map to the human sequence. The newest was released on 2020-02-19, and no atom of residues 766 to 1050 has been modelled. Three independent database routes with a passing control agree. The fold was crystallised in *Drosophila* at 1.85 and 1.95 Å, a weak template for the human domain.

3. **Few measurements exist against BubR1.** The ChEMBL activity record (a public bioactivity database) holds 24 values over 15 molecules in 7 documents, with no dissociation or inhibition constant. The five IC50 values (half-maximal inhibitory concentrations: 9.67, 10.36, 13.08 and 67.3 µM, plus one above 100 µM) come from one 2025 paper (PMID [39818011](https://pubmed.ncbi.nlm.nih.gov/39818011/)) in a radiometric assay on recombinant protein.

   We rated that paper weak on a full-text read: one cell line, a single-temperature thermal-shift assay (a measure of ligand-induced protein stabilisation), and docking on a structure the paper itself calls the BUB1 kinase domain. The paralog BUB1 (a related kinase) holds 4,123 records over 1,565 molecules, including 226 dissociation constants, the best of which is 2.1 nM.

4. **A screen has to beat 9.67 µM to add to the ChEMBL record.** One approved drug (ceritinib) has a BubR1 IC50 of 13 µM, too weak to define a selectivity window. A compound that inhibits BUB1 at 1.0 to 6.5 nM (BAY 1816032) is recorded with a BubR1 IC50 above 100 µM, a censored bound, so selectivity is known only as a lower bound: more than 52-fold against its 1.9 µM IC50 in the high-ATP (adenosine triphosphate) BUB1 assay (100 / 1.9 = 52.6). 

   A separate paper reports bubristatin, a BubR1 kinase antagonist found by computational modelling (PMID [31201382](https://pubmed.ncbi.nlm.nih.gov/31201382/); abstract read); ChEMBL holds no potency value for it [UNVERIFIED: full text not read].

5. **A public tractability label may overstate the evidence.** Open Targets, a public target-assessment platform, labels BubR1 "High-Quality Ligand" (tractability is how likely a target is to bind a drug). The best record is pChEMBL 5.01 (the negative logarithm of the molar potency). A floor of 5.5 would put that record below the label's bar, so the label would depend on an exception for equivalent activity measures.

   [UNVERIFIED: the floor and the exception are the project's reading of the Open Targets pipeline; the platform documentation read on 2026-10-24 defines the label by ligand property and scaffold counts and states no pChEMBL floor.]

6. **Homology search returns only orthologues, the paralog and generic kinases.** Orthologues are the same protein in other species. A pocket search whose control recovered two known ligand sites found no stabiliser-grade pocket.

7. **Tools for one half of a stabiliser exist.** A 2026 paper reports improved covalent ligands (ligands that bond permanently to the protein) of the deubiquitinase OTUB1 (an enzyme that removes ubiquitin, the tag that marks proteins for destruction) and a deubiquitinase-recruiting chimera for the protein CFTR (cystic fibrosis transmembrane conductance regulator) built from one of them (PMID [42083385](https://pubmed.ncbi.nlm.nih.gov/42083385/); abstract read; the working concentration is not in the abstract).

   The ligand recruits the stabilising enzyme and needs a BubR1-binding partner. The BubR1-binding half remains to be found.

8. **A C-terminal fragment supplied separately failed in the one test reported.** In a preprint (DOI [10.1101/733378](https://doi.org/10.1101/733378), version 1 full text read), a free C-terminal fragment neither reached kinetochores (the chromosome sites where spindle microtubules attach) nor licensed the key phosphorylation. Both were restored only when a chemical dimerizer (a small molecule that joins two proteins) forced the fragment against a polypeptide bearing the docking domain. The published version (PMID [33207204](https://pubmed.ncbi.nlm.nih.gov/33207204/)) has not been read [UNVERIFIED].

   The finding excludes supplying the C-terminal module as a separate payload. A fusion that holds the fragment next to the endogenous N-terminus is the one untested alternative.

9. **The minimal rescue fragment is a minimum for survival.** Residues 1 to 363 supported viability in p53-null and hypomorphic (partial loss of function) mouse fibroblasts (PMID [19154723](https://pubmed.ncbi.nlm.nih.gov/19154723/); full text read). Checkpoint activity reached 43% of normal, premature sister separation was 9% against 1% for full-length protein, and aneuploidy was not measured.

## Dose anchors

The table lists five BubR1 levels (dose anchors), the outcome at each level and the source with its limit.

| Anchor | Value | Source and limit |
|---|---|---|
| Heterozygous carriers | 0.5 of diploid; healthy | Human genetics |
| Segregation fidelity in one human cell line | About 13% of normal had virtually no effect; about 6% caused missegregation in most cells | PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/); full text read, results text on Fig. 4D; HeLa cells, doxycycline-titrated short hairpin RNA (shRNA), one readout. A related study reports residual BubR1 of 8.5, 10, 14, 58 and 77% in HeLa cells, with aneuploidy detected below 50% (PMID [18932004](https://pubmed.ncbi.nlm.nih.gov/18932004/); abstract read) |
| Mouse transgene line T7, moderate (about 5-fold over wild type in fibroblasts, inferred: the high line is 10-fold over wild type and 2-fold over T7) | Did not reduce Ras-induced aneuploidy; did not attenuate age-related aneuploidy, retinal degeneration or cardiac stress tolerance | PMID [23242215](https://pubmed.ncbi.nlm.nih.gov/23242215/); full text read; supplementary figures not opened |
| Mouse transgene line T23, high (about 10-fold over wild type in fibroblasts) | Reduced tumour development and Ras-induced aneuploidy; extended median and maximum lifespan (maximum lifespan by one-sided Wang-Allison tests, p = 0.05 and 0.0056 against two control groups); bone marrow and small intestine showed the same age-related aneuploidy as wild type | PMID [23242215](https://pubmed.ncbi.nlm.nih.gov/23242215/); full text read; chromosome fluorescence in situ hybridisation (FISH) on 3 males per genotype and tissue |
| Aneuploidy at BubR1 above wild type | No increase in aneuploidy or missegregation at about 10-fold in fibroblasts and splenocytes (3 samples per genotype) | PMID [23242215](https://pubmed.ncbi.nlm.nih.gov/23242215/); one species, one transgene, constitutive expression |

A target level above the carrier level carries unquantified risk. A titratable copy of BubR1 with a degron tag (a tag that makes degradation controllable), taken from well below to well above wild type in one human cell type with a segregation readout, would quantify this risk.

## Ranking of restoration designs by unmeasured premises

A premise is an unmeasured statement on which the design fails if false. The table ranks eight restoration designs by their premise count, and fewer premises rank higher.

| Rank | Design | Premises |
|---|---|---|
| 1 | Measure abundance, half-life and specific activity of a missense allele | 1 |
| 2 | Ex vivo prime editing of a truncating allele in haematopoietic stem cells | 4 |
| 3 | Ex vivo lentiviral addition of the coding sequence | 4 |
| 4 | Delivered tether that docks the phosphatase at the kinetochore | 6 |
| 5 | Adeno-associated virus (AAV) to a post-mitotic tissue | 7 |
| 5 | mRNA in lipid nanoparticles timed to one division | 7 |
| 6 | Bifunctional stabiliser blocking degradation of a missense protein | 8 |
| 6 | Pharmacological chaperone, intrabody or nanobody stabiliser | 8 |

The count is an ordinal ranking of designs. The two lowest-ranked rows cover three modality families (a deubiquitinase-recruiting chimera, a pharmacological chaperone, an intrabody or nanobody) that depend on the same missing BubR1 ligand, so one binder screen moves all three. Every therapeutic design addresses marrow or heart; growth, brain and skeleton are outside this scope.

## Verification

An independent AI verifier (a separate Claude session) reread the primary papers and queried the databases again behind eight load-bearing claims. Of 20 design proposals sent to blind review by AI agents, four held, five were excluded by the preprint experiment in finding 8 and the rest were narrowed.

## References

- Bohers E et al. (2008). Gradual reduction of BUBR1 protein levels results in premature sister-chromatid separation then in aneuploidy. *Hum Genet*. PMID [18932004](https://pubmed.ncbi.nlm.nih.gov/18932004/)
- Malureanu LA et al. (2009). BubR1 N terminus acts as a soluble inhibitor of cyclin B degradation by APC/C(Cdc20) in interphase. *Dev Cell*. PMID [19154723](https://pubmed.ncbi.nlm.nih.gov/19154723/)
- Suijkerbuijk SJ et al. (2010). Molecular causes for BUBR1 dysfunction in the human cancer predisposition syndrome mosaic variegated aneuploidy. *Cancer Res*. PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/)
- Baker DJ et al. (2013). Increased expression of BubR1 protects against aneuploidy and cancer and extends healthy lifespan. *Nat Cell Biol*. PMID [23242215](https://pubmed.ncbi.nlm.nih.gov/23242215/)
- Siemeister G et al. (2019). Inhibition of BUB1 Kinase by BAY 1816032 Sensitizes Tumor Cells toward Taxanes, ATR, and PARP Inhibitors In Vitro and In Vivo. *Clin Cancer Res*. PMID [30429199](https://pubmed.ncbi.nlm.nih.gov/30429199/)
- Huang Y et al. (2019). BubR1 phosphorylates CENP-E as a switch enabling the transition from lateral association to end-on capture of spindle microtubules. *Cell Res*. PMID [31201382](https://pubmed.ncbi.nlm.nih.gov/31201382/)
- Gama Braga L et al. (2020). BUBR1 Pseudokinase Domain Promotes Kinetochore PP2A-B56 Recruitment, Spindle Checkpoint Silencing, and Chromosome Alignment. *Cell Rep*. PMID [33207204](https://pubmed.ncbi.nlm.nih.gov/33207204/)
- El Hafi M et al. (2025). Synthesis and biological assessment of BUB1B inhibitors for the treatment of clear cell renal cell carcinoma. *Eur J Med Chem*. PMID [39818011](https://pubmed.ncbi.nlm.nih.gov/39818011/)
- Song X et al. (2026). Discovery of New OTUB1 Covalent Ligands via Structure-Activity Relationship Studies for Targeted Protein Stabilization. *J Med Chem*. PMID [42083385](https://pubmed.ncbi.nlm.nih.gov/42083385/)
- Braga LG et al. (2019). The BUBR1 pseudokinase domain promotes efficient kinetochore PP2A-B56 recruitment to regulate spindle checkpoint silencing and chromosome alignment. *bioRxiv*. DOI [10.1101/733378](https://doi.org/10.1101/733378)

## Other sources

- Protein Data Bank entries mapping to human BubR1 (queried 2026-10-15): 2WVI, 3SI5, 4GGD, 5JJA, 5K6S, 5SWF, 5LCW, 6TLJ, 5KHU (https://www.rcsb.org/structure/<id>); Drosophila BubR1 kinase domain 6JKK and 6JKM (PMID [31201382](https://pubmed.ncbi.nlm.nih.gov/31201382/)); human BUB1 kinase domain 6F7B (PMID [30429199](https://pubmed.ncbi.nlm.nih.gov/30429199/), Siemeister G et al. 2019).

- AlphaFold DB AF-O60566-F1, model version 6: https://alphafold.ebi.ac.uk/entry/O60566. UniProt O60566: https://www.uniprot.org/uniprotkb/O60566.

- ChEMBL activity record for BUB1B (target CHEMBL4295998: 24 values, 15 molecules, 7 documents; BUB1 paralog, target CHEMBL1772932: 4,123 records, 1,565 distinct molecules, 226 dissociation constants, best 2.1 nM; counts from the ChEMBL REST API) and Open Targets tractability label "High-Quality Ligand" (pChEMBL 5.01; the 5.5 floor is inferred, not documented): Open Targets Platform v26.9.0; ChEMBL 37 (released 2026-05-01), queried 2026-10-24; Open Targets label read [UNVERIFIED: access date of the Open Targets read not recorded]. https://platform.opentargets.org/ and https://www.ebi.ac.uk/chembl/

- The five IC50 values (9.67, 10.36, 13.08, 67.3 µM and one above 100 µM) come from one 2025 paper (PMID [39818011](https://pubmed.ncbi.nlm.nih.gov/39818011/)), recorded in ChEMBL under document CHEMBL6121040.

- Residue atlas (32 regions scored on four axes) and ranking of restoration designs: this report's analysis [UNVERIFIED: scoring table not published with this report].
