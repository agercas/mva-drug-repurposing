# IL-1 blockade with anakinra

## Candidate

Anakinra is a recombinant interleukin-1 (IL-1) receptor antagonist given by daily subcutaneous injection. It is approved for rheumatoid arthritis (adults) and for the autoinflammatory diseases neonatal-onset multisystem inflammatory disease (NOMID) and deficiency of the interleukin-1 receptor antagonist (DIRA). The label reports a NOMID study with 36 paediatric patients (13 under 2 years) and a DIRA study with 9 patients aged 1 month to 9 years (Kineret label). Use in mosaic variegated aneuploidy (MVA) would be off-label (outside the approved indications).

## Hypothesis

Aneuploid cells in a senescence-like state (a lasting growth arrest controlled by p53, a tumour-suppressor protein) secrete interleukin-6 (IL-6) and interleukin-8 (IL-8); in senescent fibroblasts, IL-1 alpha acts upstream of that secretion, through nuclear factor kappa B (NF-kB). This inflammatory secretome (the signalling proteins the cells release) may contribute to features of the syndrome; no inflammatory feature of MVA is established. Blocking IL-1 would lower the secretome and leave senescent cells alive and interferon signalling unchanged.

Each row of the table is one causal step, with a basis label defined in the [section 3 README](README.md#basis-labels): Demonstrated, Suggested, Our inference or Speculation.

| # | Step | Basis | System | Source |
|---|---|---|---|---|
| 1 | Subcutaneous anakinra blocks IL-1 receptor signalling in children at labelled exposure | Demonstrated | Human, approved paediatric indications (NOMID, DIRA); pharmacokinetics in the label | Kineret label |
| 2 | Cells with abnormal karyotypes arrest and acquire a senescence-like inflammatory programme | Suggested | Human RPE1 cells (a retinal pigment epithelial line) with drug-induced missegregation of each chromosome in 6 to 8% of mitoses, 47 to 63 times the 0.127% that the [error-free division](../appendix/error-free-division.md) model gives for the child's median BubR1 level (6 / 0.127 and 8 / 0.127); arrested cells with complex karyotypes secreted more IL-6, IL-8 and CCL2 (a chemokine). The authors report that missegregation rarely activates p53 and that DNA damage drives the p53 arrest. Full text read for PubMed identifier (PMID) 28633018, abstract for PMID 34105235 here and full text in the earlier appraisal of section 2.4.14 | PMID [28633018](https://pubmed.ncbi.nlm.nih.gov/28633018/); PMID [34105235](https://pubmed.ncbi.nlm.nih.gov/34105235/) |
| 3 | BubR1-deficient or MVA cells carry this IL-1 programme | Speculation | None; the secretome is unmeasured in MVA. Early-passage Bub1b hypomorph mouse fibroblasts raised CCL2 and no other cytokine tested, and the mild IL1B rise in public BUB1B-depleted RPE1 data lies within perturbation noise | PMID [28633018](https://pubmed.ncbi.nlm.nih.gov/28633018/) (Figure 7C) |
| 4 | IL-1 alpha is the upstream switch of the IL-6 and IL-8 secretome | Suggested | Senescent human fibroblasts in culture; antagonist, neutralising antibody and knockdown each lowered IL-6 and IL-8; abstract read | PMID [19805069](https://pubmed.ncbi.nlm.nih.gov/19805069/) |
| 5 | Blocking IL-1 lowers IL-6 and IL-8 in the child's cells | Our inference | Extrapolates step 4 from fibroblasts, assuming step 3 holds | PMID [19805069](https://pubmed.ncbi.nlm.nih.gov/19805069/) |
| 6 | Lower IL-6 and IL-8 improve a syndrome feature driven by that signalling (none is established in MVA) | Speculation | None in MVA; adult canakinumab trials give an anaemia association in a clonal-haematopoiesis subset and an exploratory lung-cancer signal | PMID [37934948](https://pubmed.ncbi.nlm.nih.gov/37934948/); PMID [28855077](https://pubmed.ncbi.nlm.nih.gov/28855077/) |
| 7 | IL-1 blockade leaves immune clearance of aneuploid cells intact | Speculation | Untested; the natural-killer clearance paper tests NF-kB and reports no IL-1 blockade or other IL-1 manipulation; IL1B mRNA is among the NF-kB targets it finds raised in the arrested aneuploid cells (Figure 4; full text read) | PMID [34105235](https://pubmed.ncbi.nlm.nih.gov/34105235/) |

Basis: 1 step Demonstrated, 2 Suggested, 1 Our inference, 3 Speculation.

## Delivery and exposure

- **Pharmacokinetics (Demonstrated: human pharmacokinetics in the label):** anakinra is a protein given subcutaneously with 95% bioavailability. Plasma concentration peaks 3 to 7 hours after a dose, and the terminal half-life is 4 to 6 hours.

- **Paediatric exposure:** in 16 NOMID patients on a median 3 mg/kg once daily for 3.5 years, steady-state peak serum concentration had a median of 3,628 ng/mL (range 655 to 8,511) and the 24-hour trough 203 ng/mL (range 53 to 1,979) (Kineret label, section 12.3).

- **Tissue reach:** the label reports serum concentrations only, so tissue levels are unreported (Speculation).

- **Clearance and formulation:** the kidney clears the agent, and the label adjusts the dosing interval in severe renal insufficiency. The label states that the prefilled syringe has a 20 mg minimum dose, a delivery limit in small children.

- **Deciding constraint:** the presence of an IL-1 programme in the child's cells decides usefulness, and it is unmeasured (Speculation, step 3).

## Evidence for

- Cell-surface IL-1 alpha is the upstream switch of the senescence secretome: an IL-1 receptor antagonist, neutralising IL-1 alpha antibodies or IL-1 alpha knockdown each reduced IL-6 and IL-8 secretion by senescent human fibroblasts, whatever the cause of senescence (PMID [19805069](https://pubmed.ncbi.nlm.nih.gov/19805069/); abstract read; cultured cells).

- In a randomised, double-blind trial of canakinumab (anti-IL-1 beta) in 10,061 adults with prior myocardial infarction and raised C-reactive protein (the Canakinumab Anti-inflammatory Thrombosis Outcomes Study, CANTOS), incident lung cancer was less frequent at 150 mg (hazard ratio 0.61, 95% CI 0.39 to 0.97) and 300 mg (0.33, 0.18 to 0.59). The authors call this an exploratory, hypothesis-generating analysis, and Novartis funded the trial (PMID [28855077](https://pubmed.ncbi.nlm.nih.gov/28855077/); abstract read).

- In a proteogenomic analysis of 4,595 CANTOS participants, canakinumab was associated with a larger haemoglobin increment in patients with clonal haematopoiesis mutations (blood cells descended from one mutated stem cell) and anaemia (PMID [37934948](https://pubmed.ncbi.nlm.nih.gov/37934948/); abstract read; association in a subset of the trial).

- Public data from BUB1B-depleted RPE1 cells show a mild rise in *IL1B* (+0.39), *CXCL8* (+0.55), *CDKN1A* (+0.93) and *IGFBP7* (+0.91) on a z-scale with a median per-gene standard deviation of 0.19 across perturbations. *IL1B* itself has a standard deviation of 0.78 (see Evidence against).

## Evidence against

- The IL-1 and IL-6 secretome is unmeasured in MVA. The IL1B rise in the public RPE1 data sits at the 73rd percentile of its own perturbation distribution, where the standard deviation across all perturbations is 0.78, so it is indistinguishable from perturbation noise. A hypomorph primary cell may differ from a p53-intact knockdown line.

- In early-passage fibroblasts from Bub1b hypomorph mice, secretion of CCL2 was slightly raised (PMID [28633018](https://pubmed.ncbi.nlm.nih.gov/28633018/); full text read, Figure 7C; mouse cells). The figure reports CCL2 only, and the text states that other cytokines were not raised. This counts against step 3 for mouse cells.

- Independence: the IL-1 alpha switch comes from one group (PMID [19805069](https://pubmed.ncbi.nlm.nih.gov/19805069/)), and the two aneuploid-cell papers share two authors (PMIDs [28633018](https://pubmed.ncbi.nlm.nih.gov/28633018/), [34105235](https://pubmed.ncbi.nlm.nih.gov/34105235/)). No paper tests the chain from aneuploidy to IL-1 to IL-6 and IL-8.

- The CANTOS lung-cancer result was hypothesis-generating. Fatal infections and sepsis were more frequent, and all-cause mortality was unchanged (PMID [28855077](https://pubmed.ncbi.nlm.nih.gov/28855077/)).

- A systematic review of five canakinumab trials in non-small cell lung cancer (adjuvant, first-line and second-line combinations and neoadjuvant therapy; 88 to 1,382 patients per trial) found no significant improvement in response rate, progression-free survival, overall survival or major pathologic response in any setting (PMID [42486074](https://pubmed.ncbi.nlm.nih.gov/42486074/); abstract read). The treatment trials in established disease were negative; the adult prevention signal came from an exploratory analysis.

- In an in vitro natural-killer cell killing system, untransformed cells with abnormal karyotypes were cleared mainly through non-cell-autonomous mechanisms that depend on NF-kB signalling (PMID [34105235](https://pubmed.ncbi.nlm.nih.gov/34105235/); abstract read here, full text in the earlier appraisal of section 2.4.14; cell culture). The paper tests NF-kB. A requirement for IL-1 in that clearance is untested, so blockade could weaken immune surveillance.

- IL-1 blockade carries infection risk. The label advises against live vaccines and active infection and cautions against combination with tumour necrosis factor (TNF) blockers. It reports neutropenia (0.4% of rheumatoid arthritis patients in placebo-controlled studies; 2 of 43 NOMID patients) and states that the effect on malignancy "is not known" (Kineret label).

- The chain from secretome to clinical features of the syndrome rests on data from outside MVA, from two research areas: senescent fibroblast culture and adult cardiovascular trials.

- NAD+ (nicotinamide adenine dinucleotide) metabolism raises the same secretome in senescent fibroblasts (PMID [30778219](https://pubmed.ncbi.nlm.nih.gov/30778219/)), and NMN supplementation enhanced it in oncogene-induced senescent fibroblasts and raised IL1B, IL6 and IL8 mRNA in one mouse model (same paper), so in those systems this candidate and the [NAD+ precursors](nad-precursors.md) pull in opposite directions; neither has been tested in MVA cells.

## Safety

The gates are defined in [Screening criteria](README.md#screening-criteria).

- Gates 1 and 2 pass on mechanism: a receptor antagonist protein with no genotoxic or mitotic action (Our inference; the label reports no long-term carcinogenicity studies, section 13.1).

- Gate 3 passes through paediatric autoinflammatory studies.

- Gate 4 is a flag: a different IL-1 agent, canakinumab, reduced lung cancer incidence in an exploratory analysis in adults, canakinumab treatment trials in established lung cancer were negative, and the anakinra label states that the effect on malignancy is not known.

- Gates 5 and 6 are flags: daily injection, infection risk, renal clearance, and neutropenia reported on the label, in a child with a chromosome-instability syndrome.

- Check against the child's other genetic findings (the secondary finding and the four carrier-state variants, [section 1.6](../01-disease-and-case.md)): pending, gene by gene ([section 3 README](README.md#check-against-the-childs-other-genetic-findings)).

## Expected effect

The magnitude of this projection is unmodelled, because the secretome is unmeasured in MVA (Our inference throughout).

- **Expected change:** if a raised IL-1 programme is present (Speculation), blockade is expected (Our inference from step 4) to lower IL-6 and IL-8 and the downstream inflammatory markers (C-reactive protein, hepcidin-linked anaemia as in PMID [37934948](https://pubmed.ncbi.nlm.nih.gov/37934948/)). The same inference expects the p53 arrest, the number of senescent cells and interferon signalling to stay unchanged.

- **Expected to stay unchanged:** aneuploid cells, BubR1 level and the rate of chromosome missegregation (Our inference: its pharmacology acts outside chromosome segregation).

- **Size of benefit:** any feature-level benefit is of unknown size (Speculation). The human effect sizes found are anaemia and lung-cancer incidence in adult trials of a different IL-1 agent (Suggested: association and exploratory analysis).

- **Dependence:** the projection depends on one unmeasured quantity, the IL-1 alpha and beta, IL-6 and IL-8 level in the child's cells or plasma against age-matched controls.

**Weakest link:** step 3, because no IL-1 or IL-6 secretome has been measured in MVA or in human BubR1-deficient cells.

## Test

- **System:** patient-derived cells and isogenic cell lines; plasma or conditioned medium from the child and age-matched controls.

- **Readout:** IL-1 alpha and beta, IL-6 and IL-8 by immunoassay; ULBP and MICA (surface ligands that natural-killer cells recognise) expression and natural-killer killing in co-culture with and without anakinra.

- **Exposure:** anakinra at concentrations within the steady-state serum range reported in paediatric NOMID patients (peak 655 to 8,511 ng/mL; Kineret label).

- **Pass criterion (fixed before the experiment):** IL-1 alpha or beta, IL-6 and IL-8 exceed the upper range of age-matched controls and anakinra lowers them without reducing natural-killer killing.

- **Stopping criterion:** cytokines within control range, or anakinra reduces ULBP or MICA expression or natural-killer killing in co-culture.

## Outcome if confirmed

A measured inflammatory secretome in MVA and a response of that secretome to an approved paediatric IL-1 antagonist. A negative first measurement removes the target after one cytokine panel.

Shared cell systems: [computational findings](../05-computational-findings.md). Disclaimer: [disclaimer and AI-use disclosure](../07-disclaimer-and-ai-use.md).

## References

- Izadpanah K et al. (2026). Efficacy and Safety of Canakinumab Compared With Standard Therapy for the Treatment of Non-Small Cell Lung Cancer (NSCLC): A Systematic Review. *Cancer Rep (Hoboken)*. PMID [42486074](https://pubmed.ncbi.nlm.nih.gov/42486074/)
- Nacarelli T et al. (2019). NAD+ metabolism governs the proinflammatory senescence-associated secretome. *Nat Cell Biol*. PMID [30778219](https://pubmed.ncbi.nlm.nih.gov/30778219/)
- Orjalo AV et al. (2009). Cell surface-bound IL-1alpha is an upstream regulator of the senescence-associated IL-6/IL-8 cytokine network. *Proc Natl Acad Sci U S A*. PMID [19805069](https://pubmed.ncbi.nlm.nih.gov/19805069/)
- Replogle JM et al. (2022). Mapping information-rich genotype-phenotype landscapes with genome-scale Perturb-seq. *Cell*. PMID [35688146](https://pubmed.ncbi.nlm.nih.gov/35688146/)
- Ridker PM et al. (2017). Effect of interleukin-1β inhibition with canakinumab on incident lung cancer in patients with atherosclerosis: exploratory results from a randomised, double-blind, placebo-controlled trial. *Lancet*. PMID [28855077](https://pubmed.ncbi.nlm.nih.gov/28855077/)
- Santaguida S et al. (2017). Chromosome Mis-segregation Generates Cell-Cycle-Arrested Cells with Complex Karyotypes that Are Eliminated by the Immune System. *Dev Cell*. PMID [28633018](https://pubmed.ncbi.nlm.nih.gov/28633018/)
- Wang RW et al. (2021). Aneuploid senescent cells activate NF-κB to promote their immune clearance by NK cells. *EMBO Rep*. PMID [34105235](https://pubmed.ncbi.nlm.nih.gov/34105235/)
- Woo J et al. (2023). Effects of IL-1β inhibition on anemia and clonal hematopoiesis in the randomized CANTOS trial. *Blood Adv*. PMID [37934948](https://pubmed.ncbi.nlm.nih.gov/37934948/)

## Other sources

- Kineret (anakinra), prescribing information, openFDA drug label API, search `openfda.brand_name:Kineret`, effective 2026-04-03, read 2026-10-24: https://api.fda.gov/drug/label.json?search=openfda.brand_name:Kineret

- Public perturbation data (RPE1 BUB1B CRISPRi pseudobulk): z-scale values as reported in the repository analysis; the public genome-scale RPE1 Perturb-seq set is Replogle et al. 2022, PMID [35688146](https://pubmed.ncbi.nlm.nih.gov/35688146/) [UNVERIFIED: the exact table used was not recorded in the sources read].
