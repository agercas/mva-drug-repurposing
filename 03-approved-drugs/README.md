# Approved drugs with mechanistic hypotheses

The searches below found no approved drug with evidence of benefit in mosaic variegated aneuploidy (MVA). The candidates are mechanistic hypotheses for investigation ([disclaimer](../07-disclaimer-and-ai-use.md)), each with an assay that can falsify it. The evidence ranks no candidate above the others ([no lead candidate](../README.md#no-lead-candidate)).

## Searches for existing studies

The searches covered three registries and one literature database. Registry searches cover registered studies; case reports and compassionate use outside registries are out of scope.

- **ClinicalTrials.gov, condition-term search, 2026-10-15:** no study and no expanded-access record (a registered programme giving access to an investigational medicine outside a trial) for MVA, *BUB1B* or BubR1 (the checkpoint protein *BUB1B* encodes).

- **EU Clinical Trials Information System (CTIS), 2026-10-15:** same result.

- **Japan Registry of Clinical Trials (jRCT), 2026-10-15:** same result.

- **ClinicalTrials.gov census, 2026-10-17:** 10 chromosomal-instability syndromes crossed with 16 search-term groups (160 combinations) returned no study for *BUB1B*, MVA or premature chromatid separation (sister chromatids parting before anaphase) in the 48 combinations for those three conditions (3 conditions by 16 term groups). The positive control, Fanconi anaemia, returned 152 studies.

- **Chinese Clinical Trial Registry (ChiCTR):** not searched, because the site returned HTTP 405.

- **Europe PMC (a literature database), title and abstract, 2026-10-24:** 43 records name *BUB1B* together with MVA or premature chromatid separation. Seven of them also contain a treatment term (treatment, therapy, therapeutic, drug, inhibitor or rescue). The seven are single case reports, one family series and mechanistic papers (see [reported research](../02-reported-research.md)); by title and abstract, none is an interventional study of a medicine for MVA. One case report describes infantile spasms refractory to antiepileptics and adrenocorticotropic hormone (PubMed identifier, PMID [23916859](https://pubmed.ncbi.nlm.nih.gov/23916859/)). The treatment-term match reflects shared vocabulary.

## Screening criteria

A candidate enters this section after a seven-gate safety screen written before candidate generation. The screen records its flags on each card and admits the candidate to the laboratory test on that card. The appendix assesses alternative approaches to the candidates in sections 3 and 4.

The criteria are this report's own; the genotoxicity assays follow Organisation for Economic Co-operation and Development (OECD) Test Guidelines 471 (bacterial reverse mutation), 473 (chromosomal aberration) and 487 (micronucleus).

| Gate | Criterion |
|---|---|
| 1 Genotoxicity | Mutagen (alters DNA sequence), clastogen (breaks chromosomes) or other DNA-damaging agent; positive Ames (bacterial mutation), micronucleus or chromosomal-aberration assay |
| 2 Aneugenicity | Spindle poison, mitotic-kinase inhibitor or further weakening of the spindle assembly checkpoint |
| 3 Paediatric exposure | Paediatric label or published paediatric experience |
| 4 Cancer-risk direction | Direction in which the candidate's biology moves tumour risk in a cancer-predisposition syndrome |
| 5 Chronic-use tolerability | Tolerability of long-term use in a child |
| 6 Interaction with existing care | Interaction with drugs a patient may already receive |
| 7 Evidence | Model system, read basis and number of independent groups stated |

Gates 1 and 2 disqualify a candidate in the screen as written. Where a card records a flag at gate 1 or 2 (the N-acetylcysteine card at gate 1; the lentiviral add-back card at gates 1 and 2; the prime-editing card at gate 1, and its ex vivo culture of BubR1-low cells raises the same gate 2 question without a recorded flag), the flag is stated on the card and the candidate is kept as a hypothesis for laboratory test, without an argument that the flag does not apply.

## Check against the child's other genetic findings

Track 1 reported one secondary finding and four further heterozygous carrier-state variants in genes unrelated to *BUB1B*. Each card states the status of the check against the known biology of those genes. The check is open for every card, and a reader with access to the genome data can run it for any candidate.

## Candidate card

Every candidate uses the same nine fields.

| Field | Content |
|---|---|
| Candidate | Name, approval status and indication, route, paediatric exposure |
| Hypothesis | What the candidate does to which step of the mechanism, followed by a table with one row per causal step, its basis label, the system and the source |
| Delivery and exposure | Route, formulation, tissue reach, concentrations achieved in humans or models, constraints |
| Evidence for | Findings with identifier, model system, sample size, read basis |
| Evidence against | Same format, including negative results, findings of the opposite sign and the number of independent research groups behind the mechanism |
| Safety | Adverse effects, cancer-risk direction, check against the other findings |
| Expected effect | What changes if the hypothesis holds, with a model-based range, its assumptions, what would not change, and the unmeasured quantity it depends on (a projection) |
| Test | System, readout, human-achievable exposure, pass and stopping criteria written before the experiment |
| Outcome if confirmed | What the result would establish |

## Basis labels

Each mechanism step and each projected number carries one of four labels.

| Label | Meaning |
|---|---|
| Demonstrated | Shown by experiment in the cited paper, in the system named, with a control |
| Suggested | One method or one research group, an association, or a different system from the child's cells |
| Our inference | Derived by this report from cited facts or a model, with the assumption stated |
| Speculation | No supporting evidence found; stated as a possibility |

A step demonstrated in mouse stays untested in the child's cells, and the card says which.

## Candidate cards

1. [NAD+ precursors](nad-precursors.md): nicotinic acid and nicotinamide riboside, precursors of nicotinamide adenine dinucleotide (NAD+), acting on acetylation-controlled turnover of BubR1.
2. [Interleukin-1 (IL-1) blockade](il1-blockade.md): anakinra, acting on the inflammatory secretome (the signalling proteins a cell releases) of aneuploid cells.
3. [N-acetylcysteine and ascorbate](n-acetylcysteine.md): antioxidants, acting on oxidative stress at the kinetochore (the spindle attachment site on a chromosome).

## Comparison

Expected effects are projections that depend on unmeasured quantities, described on each card.

| Candidate | Hypothesis | Expected effect (projection) | Evidence for | Evidence against | Safety | Test cost and first test |
|---|---|---|---|---|---|---|
| [NAD+ precursors](nad-precursors.md) | Raising NAD+ activates sirtuin 2 (SIRT2), which removes the acetyl mark on lysine 668 (K668) that targets BubR1 for degradation, so the missense protein lasts longer | A 1.69- to 2.45-fold BubR1 rise reaches the level that gave near-normal segregation in HeLa cells (13% of wild type) only if the missense protein keeps about 11 to 15% of one wild-type allele's functional abundance; carrier level needs 41 to 59% and is out of reach for kinase-region alleles that sit 5 to 10 times below wild type | Cell-line data on the acetylation switch; a SIRT2 transgene extended median lifespan of hypomorph mice (mice with partly reduced gene function) by 58% (P = 0.038), mostly in males; a single-arm precursor trial in ataxia telangiectasia raised blood NAD+ | One research group behind the mechanism; no independent report of K668 acetylation, and the acetyl may sit on K667; nicotinamide inhibits the needed enzymes; at equal BubR1 abundance, other lesions in the kinase-like (pseudokinase) domain did not regain recruitment of the phosphatase PP2A-B56; no precursor tested in a hypomorph; possible cancer-direction downside | Supplement-grade record; cancer direction unresolved | Low: cell-based half-life assay, with PP2A-B56 recruitment and micronuclei read at equal BubR1 abundance |
| [Anakinra](il1-blockade.md) | Blocking IL-1 lowers the inflammatory secretome of aneuploid cells | Lower interleukin-6 (IL-6), interleukin-8 (IL-8) and inflammatory markers if the secretome is raised; no change to BubR1 or missegregation; feature-level benefit unknown | Cell-culture mechanism in senescent fibroblasts; anaemia and lung-cancer associations in adult trials of canakinumab, an antibody against IL-1 beta | The IL1B rise in public data lies within perturbation noise and BubR1-hypomorph mouse fibroblasts raised only CCL2 (a chemokine); infection risk, including fatal infections in the canakinumab trial; possible loss of natural-killer clearance | Paediatric label for autoinflammatory disease; injection | Low: cytokine panel in patient cells |
| [N-acetylcysteine and ascorbate](n-acetylcysteine.md) | Lowering oxidative stress preserves kinetochore BubR1 and checkpoint function | Partial restoration of BubR1 function; size unmeasured | Antioxidants lowered segregation errors in Sod1-knockout mouse oocytes at 21% oxygen; BubR1-hypomorph mice die more under an oxidative stressor (no antioxidant arm described) | No antioxidant tested in any BubR1-deficient system; N-acetylcysteine accelerated mouse lung cancer through p53; the oocyte model has normal BubR1 | Injection label bases paediatric use on clinical practice; flags on cancer direction and interactions | Low: reactive-oxygen species and kinetochore BubR1 panel at 3% and 20% oxygen |

### Mechanism basis by candidate

Each card labels every causal step of its mechanism. The table counts the steps per label and names the weakest link, the least supported step.

| Candidate | Steps | Demonstrated | Suggested | Our inference | Speculation | Weakest link |
|---|---|---|---|---|---|---|
| [NAD+ precursors](nad-precursors.md) | 8 | 0 | 4 | 1 | 3 | No paper tests whether the K668 acetylation switch controls turnover of the child's N1002K protein (lysine in place of asparagine 1002); kinase-region data point to a different clearance route, and a higher level may not restore PP2A-B56 function |
| [Anakinra](il1-blockade.md) | 7 | 1 | 2 | 1 | 3 | No IL-1 or IL-6 secretome has been measured in MVA or in human BubR1-deficient cells |
| [N-acetylcysteine and ascorbate](n-acetylcysteine.md) | 9 | 0 | 4 | 2 | 3 | The oxidative share of the BubR1 deficit in the child's cells is unmeasured |

All first tests use the shared cell system in [computational findings](../05-computational-findings.md#510-experimental-platform-shared-by-sections-3-and-4).

## References

- Akasaka N et al. (2013). Refractory infantile spasms associated with mosaic variegated aneuploidy syndrome. *Pediatr Neurol*. PMID [23916859](https://pubmed.ncbi.nlm.nih.gov/23916859/)

## Other sources

- Registry searches, condition terms MVA, *BUB1B*, BubR1 and premature chromatid separation, searched 2026-10-15: ClinicalTrials.gov API v2 (https://clinicaltrials.gov/data-api/api), EU CTIS (https://euclinicaltrials.eu/) and jRCT (https://jrct.mhlw.go.jp/en-top). ClinicalTrials.gov census of 10 syndromes by 16 term groups (160 combinations; positive control Fanconi anaemia 152 studies) run 2026-10-17; query details in the Other sources of [reported research](../02-reported-research.md). ChiCTR (https://www.chictr.org.cn/) was not searched (HTTP 405).

- Europe PMC REST API (https://www.ebi.ac.uk/europepmc/webservices/rest/search), search date 2026-10-24: `(TITLE_ABS:"BUB1B" OR TITLE_ABS:"BUBR1") AND (TITLE_ABS:"mosaic variegated aneuploidy" OR TITLE_ABS:"premature chromatid separation" OR TITLE_ABS:"MVA" OR TITLE_ABS:"PCS syndrome")` returns 43 records. Adding `AND (TITLE_ABS:"treatment" OR TITLE_ABS:"therapy" OR TITLE_ABS:"therapeutic" OR TITLE_ABS:"drug" OR TITLE_ABS:"inhibitor" OR TITLE_ABS:"rescue")` returns 7.

- Safety screen (seven gates): document written for this report before candidate generation [UNVERIFIED: not published with this report; the gate definitions are reproduced in this file]. OECD Test Guidelines 471, 473 and 487 (OECD Guidelines for the Testing of Chemicals).

- Candidate cards link their own sources: [NAD+ precursors](nad-precursors.md), [IL-1 blockade](il1-blockade.md), [N-acetylcysteine and ascorbate](n-acetylcysteine.md).
