# Computational findings

Folding, stability, design and quantitative models were run on the two variants in *BUB1B*, the gene for the spindle-checkpoint protein BubR1, and their results bear on the hypotheses in sections 3 and 4. Every analysis used public sequences, public structures and the two public variant identities, with a positive control for each model; a model that failed its control is reported as unable to detect the effect. Databases and software are listed in [References and tools](06-references-and-tools.md).

## 5.1 Two-allele architecture

The stop-gain variant (p.Leu737Ter, TTA to TGA, a change that creates a stop codon) sits at codon 737 in exon 17 of 23, in a TGA-A context (CCAGAG-TGA-AGTGCC). The stop codon ends 746 nucleotides upstream of the last exon-exon junction (RefSeq NM_001211.6: the codon ends at position 2363 and the junction follows position 3109), which predicts degradation by nonsense-mediated decay (NMD, the pathway that degrades transcripts with premature stop signals). The missense variant (p.Asn1002Lys, a change of one amino acid) sits in the last exon, so its transcript escapes NMD.

Experimental structures resolve every region that a protein stopped at residue 736 would keep. Published patient truncations bracket the product: a 731-residue truncation retained function and a 753-residue truncation was unstable and non-functional (PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/)). In the AlphaFold model, residues 721 to 737 form a helix that docks on the pseudokinase domain; the 731-residue truncation keeps residues 721 to 731 of it and a product stopped at residue 736 keeps residues 721 to 736 (Our inference from a predicted structure). The cell-based test of whether the stop allele escapes NMD is in [5.10](#510-experimental-platform-shared-by-sections-3-and-4).

## 5.2 The missense site is a buried clamp

Nine Protein Data Bank (PDB) entries map to human BubR1. The pseudokinase domain (a kinase-like domain, residues 766 to 1050) that holds residue 1002 is unresolved in all nine, including the three structures of the anaphase-promoting complex/cyclosome (APC/C) bound to the mitotic checkpoint complex (5LCW, 5KHU and 6TLJ). Experimental kinase-domain structures of *Drosophila* BubR1 and human BUB1 show the equivalent asparagine clamping the backbone of the tryptophan that corresponds to residue 978, as the AlphaFold model does.

The table lists the evidence for conservation and contacts at residue 1002.

| Evidence | Result |
|---|---|
| Orthologues | Asparagine at the 1002 position in 99% of 221 vertebrate sequences |
| Family alignment | Asparagine in 95.2% of 3,388 Bub1/Mad3-family domains from 2,355 species after down-weighting near-identical sequences (3,268 sequences, 96.5%, unweighted; BubR1-like 98.5%, Bub1-like 94.7%); 97th conservation percentile in BubR1-like sequences; 12 of 12 structural anchors recovered |
| Surface check | No BubR1-specific conserved surface within 14 Å, so this report reads a shared fold clamp |
| Smallest self-folding unit | Residues 842 to 1041 (200 residues; core root-mean-square deviation (RMSD) 0.45 Å; template-modelling score (TM-score) 0.99) |
| Contacts | The 973 to 978 stretch carries 60% of the heavy-atom contacts of the asparagine side chain (tryptophan 978 alone 35%) |

Sequence windows under about 150 residues lose the fold, and without alignments every window collapses, so later folding runs used the 766 to 1050 construct.

Lysine occurs at this position in one fungal species (a mucoralean fungus) and arginine in rust fungi. Among 28 sequences with a residue other than asparagine (gaps excluded), 14 have a gap at the tryptophan 978 column, against 11 of 3,268 asparagine sequences (odds ratio 296 by Fisher's exact test; a post hoc, lineage-clustered comparison, so inflated).

A pre-specified natural-host test of whether an in-frame deletion of that segment would accommodate lysine failed its control (2 of 4 hosts met the rule, 3 required). The test could not detect whether a deletion would help, so this report gives geometry only.

## 5.3 Folding models show the lost clamp

Four structure predictors folded wild type, the lysine variant, 5 published hypomorphic alleles (alleles with reduced function) used as calibrators, 10 neutral references and 9 synthetic buried-to-aspartate or proline substitutions: Boltz-2, OpenFold3, ESMFold v1 and ESMFold2. The hosted co-folding models returned identical output on repeat runs, so noise floors came from alignment subsampling.

The table gives the four models' result on the lysine variant and on severity ranking. Local pLDDT (predicted local distance difference test) is the model's predicted local confidence in the fold.

| Criterion | Result |
|---|---|
| Agreement of the four models on the lysine variant | All four models agree. Lysine at 1002 loses the three backbone contacts of the asparagine clamp, turns outward and lowers the confidence of the surrounding shell (residues within 8 Å) by 1.6 to 2.4 pLDDT points. In the two Boltz-2 lysine models the side chain is 66 to 68 Å² exposed, with 0 to 2 polar partners and no acid within 8 Å |
| Size of the effect | In Boltz-2 on residues 766 to 1050, the shell moves 0.55 Å (z 2.8 against alignment-subsampling noise) and local pLDDT falls by 2.2 |
| Severity ranking by the models | No model separates calibrators and synthetic controls from neutrals on all pre-specified metrics, and in Boltz-2 8 of 9 synthetic radical substitutions go undetected |

No model passed its calibration, so the agreement on the lysine variant describes the predicted structure only. Severity and protein loss need measurement, and the pre-specified rule for interpreting the variant stays unapplied. Any hypothesis about the missense protein depends on its abundance and activity, which are unmeasured.

## 5.4 Stability methods

Five computational methods estimate the stability effect of the lysine change at residue 1002: frustration scores (Python frustratometer 0.3.2), an evolutionary coupling model (a Potts model of the Bub1/Mad3 family alignment), a protein stability predictor (ThermoMPNN), protein language models (ESM-1v and ESM-2) and a regression model for the abundance of pseudokinase missense proteins. Each ran with a positive control.

The regression model failed its control: it met its pre-registered criteria in 203 of 300 simulated replicates, against a bar of 240. Its prediction for the lysine variant is therefore the mean of 13 published alleles (four with assumed abundance ranges): a median abundance of 0.32 of wild type, with an 80% interval of 0.08 to 1.3. The platform of section 5.10 would measure the abundance and activity of the protein in cells.

## 5.5 Measured missense alleles and variant predictors

Two public screens contain five BubR1 patient alleles: Wei 2014 (PMID [25502805](https://pubmed.ncbi.nlm.nih.gov/25502805/); a green fluorescent protein (GFP) stability assay plus yeast two-hybrid, a test of whether two proteins bind in yeast) and Fragoza 2019 (PMID [31515488](https://pubmed.ncbi.nlm.nih.gov/31515488/); yeast two-hybrid).

The three kinase-region alleles (R727C, L844F, L1012P; residue 727 lies 39 residues before the pseudokinase domain, which starts at residue 766) are unstable and lose the interaction with CDC20 (the activator of the anaphase-promoting complex). The two N-terminal alleles (R36Q, Y155C) are stable and keep it.

Controls on other genes pass: unstable alleles lose the interaction 15 of 15 times, and disease alleles disrupt it 2.8 times as often as population alleles. The chance that all three unstable alleles lose the interaction is 0.0007 at a 9% base rate (0.09³ = 0.00073).

Both screens are assays of single overexpressed variants (GFP fusions in HEK293T cells and yeast two-hybrid in yeast, per the Wei 2014 methods), and three unstable alleles are too few for a rate estimate. Both tables omit the p.Asn1002Lys allele [UNVERIFIED: the five BubR1 rows sit in supplementary tables that were not opened, and the control analysis is not published with this report].

A 2010 study (PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/), full text read) measured kinase-region substitutions: I909T, L1012P, L844F, R814H and R727C are low-abundance disease alleles, and Q921H is a stable polymorphism. Read allele by allele, the residual protein with a null partner (a second allele that makes no protein) is about 5 to 25% of a diploid wild-type amount (fold decreases of 2 to 10 leave 1/10 to 1/2 of one wild-type allele, halved against a diploid reference).

The table gives each variant predictor's call on the five low-abundance hypomorphs and its score for p.Asn1002Lys.

| Predictor | Result on the five low-abundance hypomorphs |
|---|---|
| AlphaMissense | 1 likely pathogenic, 1 ambiguous, 3 likely benign; 0.923 for p.Asn1002Lys (5th of 19 substitutions at the site) |
| REVEL (Rare Exome Variant Ensemble Learner; ≥ 0.5) | 1 of 4; 0.472 for the variant |
| CADD (Combined Annotation Dependent Depletion; ≥ 20) | 4 of 4 |

The predictors under-call destabilised alleles. Details are in the [pathogenicity appendix](appendix/variant-pathogenicity-prediction.md) and the [residue atlas](appendix/residue-atlas.md).

## 5.6 Pseudokinase domain

Residues 766 to 1050 are unresolved in every human experimental model. The ChEMBL activity record (a public bioactivity database) holds 24 activity measurements over 15 molecules, with no dissociation or inhibition constant; the strongest figure is an IC50 (half-maximal inhibitory concentration) of 9.67 µM.

## 5.7 Quantitative models

The table gives the result of each of five quantitative models.

| Model | Result |
|---|---|
| Dose-response of segregation errors | A four-parameter curve fitted to ten published readouts has its half-point (the BubR1 level midway between the curve's floor and ceiling) at 8.6% of normal BubR1. Two of the ten readouts fall outside the posterior predictive range. The curve is anchored on mouse fibroblasts and HeLa cells |
| Limiting functional BubR1 in the child | Product of transcript, translation, folded fraction and specific activity for each allele, sampled 200,000 times. The median is 0.12 of normal (90% interval 0.02 to 0.40) under the patient-line reading (the missense-protein level reported for four patient-derived lines, read per allele) and 0.23 (0.06 to 0.49) under the whole-cell reading (the same level read as a whole-cell value relative to healthy controls). Patient-line reading: the folded fraction of the missense protein (rank correlation 0.59) and the stability of the stop-allele product (0.48) set the result, and the stop-allele transcript fraction hardly matters (0.21). Whole-cell reading: the specific activity of the missense protein (0.56) and the stability of the stop-allele product (0.40) lead, and the folded fraction falls to 0.34 |
| Probability of an error-free division | Median chance that a division segregates all chromosomes correctly: 0.93 (5th to 95th percentile 0.74 to 0.98; range of medians 0.85 to 0.94 under alternative inputs). The fitting method recovered simulated truths (coverage 0.93 against a target band of 0.78 to 0.98). See the [appendix](appendix/error-free-division.md) |
| Fold rescue needed | With a null partner the residual is abundance × specific activity / 2 of a wild-type diploid. A rise of 1.69-fold in young or 2.45-fold in aged wild-type mouse testis (the aged value is recovery of an age-depressed level) after 7 days of nicotinamide mononucleotide (NMN, a precursor of nicotinamide adenine dinucleotide, NAD+), read by eye from Fig. 6E with n = 3 per group (PMID [24825348](https://pubmed.ncbi.nlm.nih.gov/24825348/)), reaches the HeLa near-normal-segregation threshold of 0.13 (13% of wild-type BubR1, the level that gave near-normal segregation in HeLa cells) only if the missense protein keeps an abundance × activity product of at least 2 × 0.13 / fold, which is 0.15 or 0.11. It reaches carrier level (0.5) only if the product is at least 2 × 0.5 / fold, which is 0.59 or 0.41. A turnover-only fix is bounded near 2-fold, the faster turnover measured for two kinase-region alleles (I909T and R727C; PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/)) |
| Readthrough or suppression on an NMD-degraded transcript | The yield calculation indicates that readthrough is unlikely to restore the missing dose unless NMD is inhibited, which would also release the truncated product. Computed full-length product per edited cell: a median 0.04 to 0.10 of one wild-type allele (5th to 95th percentile 0.01 to 0.34) at an assumed readthrough of 0.05 to 0.40 and decay efficiency of 0.5 to 0.95, with three coupling models calibrated on the reported text of PMID [35322228](https://pubmed.ncbi.nlm.nih.gov/35322228/) (figure values not seen) |

The three hypotheses for the missense protein (destabilised fold, interface defect, both) stay unresolved: public data leave all three open for p.Asn1002Lys, and the nearest evidence is analogue alleles, one mouse allele (BubR1 L1002P; PMID [31738183](https://pubmed.ncbi.nlm.nih.gov/31738183/)) and the conserved clamp.

## 5.8 Editor design scan

From the reference sequence alone, the scan enumerated 138 base-editor designs (100 distinct combinations of guide and outcome) and 4,842 geometries of prime-editing guide RNAs (pegRNAs) for the two variant sites.

The table gives the scan's results for base editing at each site, for prime editing and for its controls.

| Finding | Detail |
|---|---|
| Base editing at the stop codon | Every SpCas9 (Cas9 from *Streptococcus pyogenes*) guide with an NGG protospacer-adjacent motif (PAM, the short sequence Cas9 needs beside its target) places the variant base outside the core editing window. An NG-class adenine editor gives leucine to arginine (the reference allele is synonymous), and every guide that could give tryptophan also co-edits the adjacent serine 738 adenine |
| Base editing at the missense site | Glycosylase C-to-G and G-to-Y editors can restore asparagine with only a synonymous bystander at the window edge |
| Allele-exclusive prime editing | Both variants create a PAM site, so allele-exclusive pegRNAs exist, and the reversion destroys the PAM |
| Controls | All 138 designs close at the protein level; an independent regular-expression enumeration is identical; three published guides are reproduced; the directional control of PRIDICT2 (a deep-learning predictor of prime-editing efficiency) passes (Spearman −0.33). The scan covers guide geometry and protein-level outcome |

## 5.9 Findings and the hypotheses they bear on

The table links each computational finding to the cards or sections it bears on.

| Finding | Bears on |
|---|---|
| The missense variant removes a buried clamp; protein abundance and activity are unmeasured | Every card. Stabilising and fold-correcting hypotheses ([NAD+ precursors](03-approved-drugs/nad-precursors.md), [N-acetylcysteine and ascorbate](03-approved-drugs/n-acetylcysteine.md)) depend on the surviving fraction; the abundance prior for an unmeasured pseudokinase missense protein spans 0.08 to 1.3 of wild type (80% interval, [5.4](#54-stability-methods)) |
| Frustration, coupling and language-model scores could not detect effects at clamp sites | The scores could not rank rescue substitutions; a second-site fix is untested |
| Readthrough or suppression on an NMD-degraded transcript yields 0.04 to 0.10 of an allele per edited cell | [Readthrough and decay inhibition](appendix/alternative-approaches-assessed/readthrough-and-nmd-inhibition.md) and [sequence-level rescue routes](appendix/alternative-approaches-assessed/sequence-level-rescue-routes.md) in the appendix |
| Allele-exclusive pegRNAs exist at both sites | [Prime-editing reversion](04-non-approved-therapies/prime-editing-reversion.md) |
| Correction of blood cells addresses a median 0.037 of the documented disease burden, with engraftment probabilities of 0.05 (prime editing) and 0.32 (lentiviral add-back) | [Prime-editing reversion](04-non-approved-therapies/prime-editing-reversion.md) and [lentiviral add-back](04-non-approved-therapies/lentiviral-add-back.md) |
| NMN raised mouse testis BubR1 1.69- to 2.45-fold; reaching the HeLa near-normal-segregation threshold or carrier level needs a missense abundance × activity product of 0.11 to 0.59 | [NAD+ precursors](03-approved-drugs/nad-precursors.md) |

## 5.10 Experimental platform shared by sections 3 and 4

One engineered system would answer most dose questions behind the drug hypotheses. The platform is a design awaiting its first run.

The table lists the four components of the platform, their design and the aim of each.

| Component | Design | Aim |
|---|---|---|
| Isogenic cell system | Near-diploid, non-transformed hTERT-RPE1 cells (human retinal pigment epithelial cells immortalised with telomerase) carrying the natural *BUB1B* gene with a luminescent tag and a switchable degradation tag, so that BubR1 is set from about 5% to above 100% of normal and read in a plate reader. Each division is filmed once. Further lines carry a truncating allele, the missense allele and controls with the same tag | Dose needed per readout; the safe upper limit of BubR1; the role of the interphase pool (BubR1 present between divisions) in setting mitosis length; the effect of truncated-transcript decay on output from the other allele; abundance and per-molecule activity of the missense protein |
| Patient-derived cells | Allele-resolved transcript ratio, with and without a translation inhibitor and with depletion arms for UPF1 (a decay factor) and ILF3 (an RNA-binding protein); level and half-life of the missense protein, with an inhibitor panel | Escape of the stop allele from NMD; protein abundance and activity |
| Approved-drug screen | Approved compounds on the titratable line, with a sign control (which shows whether a compound raises or lowers errors) and safety triage. The screen detects effects that remove about half or more of the missegregation; a null result means every compound fell below that size | Approved compounds that lower missegregation in checkpoint-weak human cells |
| Mouse | Staged study in a BubR1-hypomorph mouse | Effect of a candidate class in a BubR1-weak animal |

A desk check at no cost and a two-week bench control come first. Each hypothesis has confirmation, stopping and intermediate criteria, written before data collection. One stopping criterion applies to every candidate: a rise in segregation errors or micronuclei above the untreated arm ends that candidate.

Rough estimates from itemised cost bands: the dose ladder USD 0.16 to 0.35 million over 9 to 12 months; the full core USD 0.4 to 0.9 million over 15 to 18 months [UNVERIFIED: the bands are the project's own estimates without vendor quotations, and the budget is not published with this report].

The study covers cultured cells and mice. It resolves effects larger than about 10% on the surviving copy, and extending a result to a child's tissues or the early embryo needs separate evidence.

### Stopping measurements by candidate

Each first test has a result that stops its candidate. The first three rows follow the weakest step on the candidate's card, and the fourth applies to every candidate.

| Measurement | Result | Candidate stopped |
|---|---|---|
| Missense-allele protein abundance and half-life | Abundance below about 11% of one wild-type allele, or near normal | NAD+ precursors: a 1.69 to 2.45-fold rise cannot reach the near-normal-segregation threshold, has nothing to raise, or leaves recruitment of the phosphatase PP2A-B56 (protein phosphatase 2A with its B56 subunit) low at equal protein abundance |
| Interleukin-1 and interleukin-6 secretome | Not raised | Anakinra |
| Oxidative stress and kinetochore BubR1 at 3% and 20% oxygen | No oxidative share of the deficit | N-acetylcysteine and ascorbate |
| Segregation errors and micronuclei under any candidate | Any rise | That candidate |

Competitive growth of corrected against mutant blood stem cells decides how well the two gene-level routes engraft. A missing advantage moves both to conditioned engraftment ([section 4](04-non-approved-therapies/README.md)).

## 5.11 Generalisation

Each hypothesis applies to the genotype classes in which its premise holds. A hypothesis that raises the amount of a hypomorphic missense protein applies to patients with a surviving missense allele, and a hypothesis about a stop allele applies to patients with a truncating variant that escapes decay.

The same workflow (gene, mechanism, approved-agent census, safety screen, cell-based test with positive controls) ran on two further genes, both with well-known partners; its performance on an unseen gene is untested. The appraisal protocol for full-text reading and the controls apply to any gene.

## References

- Suijkerbuijk SJ et al. (2010). Molecular causes for BUBR1 dysfunction in the human cancer predisposition syndrome mosaic variegated aneuploidy. *Cancer Res*. PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/)
- North BJ et al. (2014). SIRT2 induces the checkpoint kinase BubR1 to increase lifespan. *EMBO J*. PMID [24825348](https://pubmed.ncbi.nlm.nih.gov/24825348/)
- Wei X et al. (2014). A massively parallel pipeline to clone DNA variants and examine molecular phenotypes of human disease mutations. *PLoS Genet*. PMID [25502805](https://pubmed.ncbi.nlm.nih.gov/25502805/)
- Ioannidis NM et al. (2016). REVEL: An Ensemble Method for Predicting the Pathogenicity of Rare Missense Variants. *Am J Hum Genet*. PMID [27666373](https://pubmed.ncbi.nlm.nih.gov/27666373/)
- Rentzsch P et al. (2019). CADD: predicting the deleteriousness of variants throughout the human genome. *Nucleic Acids Res*. PMID [30371827](https://pubmed.ncbi.nlm.nih.gov/30371827/)
- Fragoza R et al. (2019). Extensive disruption of protein interactions by genetic variants across the allele frequency spectrum in human populations. *Nat Commun*. PMID [31515488](https://pubmed.ncbi.nlm.nih.gov/31515488/)
- Sieben CJ et al. (2020). BubR1 allelic effects drive phenotypic heterogeneity in mosaic-variegated aneuploidy progeria syndrome. *J Clin Invest*. PMID [31738183](https://pubmed.ncbi.nlm.nih.gov/31738183/)
- Wang J et al. (2022). AAV-delivered suppressor tRNA overcomes a nonsense mutation in mice. *Nature*. PMID [35322228](https://pubmed.ncbi.nlm.nih.gov/35322228/)
- Lin Z et al. (2023). Evolutionary-scale prediction of atomic-level protein structure with a language model. *Science*. PMID [36927031](https://pubmed.ncbi.nlm.nih.gov/36927031/)
- Cheng J et al. (2023). Accurate proteome-wide missense variant effect prediction with AlphaMissense. *Science*. PMID [37733863](https://pubmed.ncbi.nlm.nih.gov/37733863/)
- Varadi M et al. (2024). AlphaFold Protein Structure Database in 2024: providing structure coverage for over 214 million protein sequences. *Nucleic Acids Res*. PMID [37933859](https://pubmed.ncbi.nlm.nih.gov/37933859/)
- Dieckhaus H et al. (2024). Transfer learning to leverage larger datasets for improved prediction of protein stability changes. *Proc Natl Acad Sci U S A*. PMID [38285937](https://pubmed.ncbi.nlm.nih.gov/38285937/)
- Mathis N et al. (2025). Machine learning prediction of prime editing efficiency across diverse chromatin contexts. *Nat Biotechnol*. PMID [38907037](https://pubmed.ncbi.nlm.nih.gov/38907037/)

## Other sources

- Protein Data Bank entries mapping to human BubR1 (UniProt O60566), RCSB queries run 2026-10-15 and repeated 2026-10-24 with the same nine entries: 2WVI, 3SI5, 4GGD, 5JJA, 5K6S, 5SWF, 5LCW, 6TLJ, 5KHU, each at https://www.rcsb.org/structure/<id>. Drosophila BubR1 kinase domain: 6JKK and 6JKM (UniProt A1Z6I7). Human BUB1 kinase domain used as paralog control: 6F7B (and 4QPM, 5DMZ, 4R8Q). Yeast Bub3-Mad3: 2I3T. S. pombe checkpoint complex: 4AEZ.

- AlphaFold Protein Structure Database, entry AF-O60566-F1, model version 6 (model created 2025-08-01), https://alphafold.ebi.ac.uk/entry/O60566. Varadi M et al. (2024), PMID [37933859](https://pubmed.ncbi.nlm.nih.gov/37933859/).

- UniProt O60566 (reviewed entry, sequence version 3): https://www.uniprot.org/uniprotkb/O60566. Ensembl gene ENSG00000156970. RefSeq transcript NM_001211.6.

- Boltz-2: Passaro S et al. (2025), preprint DOI [10.1101/2025.06.14.659707](https://doi.org/10.1101/2025.06.14.659707); run through a hosted NVIDIA Inference Microservices (NIM) service [UNVERIFIED: container version not recorded in the sources read].

- ESMFold v1: Lin Z et al. (2023), PMID [36927031](https://pubmed.ncbi.nlm.nih.gov/36927031/). ESMFold2 and OpenFold3 as served by the same hosted service [UNVERIFIED: no citation or version recorded in the sources read].

- ThermoMPNN: Dieckhaus H et al. (2024), PMID [38285937](https://pubmed.ncbi.nlm.nih.gov/38285937/); code fetched from its public GitHub repository [UNVERIFIED: commit not recorded].

- AlphaMissense: Cheng J et al. (2023), PMID [37733863](https://pubmed.ncbi.nlm.nih.gov/37733863/); REVEL: Ioannidis NM et al. (2016), PMID [27666373](https://pubmed.ncbi.nlm.nih.gov/27666373/); CADD: Rentzsch P et al. (2019), PMID [30371827](https://pubmed.ncbi.nlm.nih.gov/30371827/) [UNVERIFIED: CADD version and score table release not recorded].

- PRIDICT2 (prime-editing efficiency predictor): Mathis N et al. (2025), *Nat Biotechnol*, PMID [38907037](https://pubmed.ncbi.nlm.nih.gov/38907037/); code from its public GitHub repository [UNVERIFIED: commit not recorded].

- ChEMBL activity record for BUB1B, target CHEMBL4295998 (24 activity measurements, 15 molecules, 7 documents; strongest value an IC50 of 9.67 µM): ChEMBL 37 (released 2026-05-01), REST API queried 2026-10-24, https://www.ebi.ac.uk/chembl/.

- Bub1/Mad3 family alignment (5.2): UniProt PANTHER family PTHR14030 (6,733 entries fetched 2026-10-20), aligned with pyfamsa 0.7 (FAMSA) and a profile hidden Markov model built with pyhmmer 0.12 (HMMER); Potts model of the EVcouplings type [UNVERIFIED: tool versions and settings recalled from the project notes, and the alignment is not published with this report].

- Frustration scores: Python frustratometer 0.3.2 (AWSEM energy model). Protein language models, public weights run locally: ESM-1v, Meier J et al. (2021), preprint DOI [10.1101/2021.07.09.450648](https://doi.org/10.1101/2021.07.09.450648); ESM-2 650M, Lin Z et al. (2023), PMID [36927031](https://pubmed.ncbi.nlm.nih.gov/36927031/). Regression model of missense abundance (5.4): this report's analysis of 13 published alleles [UNVERIFIED: not published with this report].

- Dose-response and error-free-division model inputs: see the appendix [error-free division](appendix/error-free-division.md).
