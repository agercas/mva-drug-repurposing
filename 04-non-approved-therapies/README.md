# Non-approved therapies with hypotheses

Both candidate routes correct blood stem cells in the child with mosaic variegated aneuploidy (MVA, a syndrome in which cells carry varying chromosome numbers). At published efficiencies neither reaches carrier-level function of BubR1 (the spindle checkpoint protein encoded by *BUB1B*) in most Monte Carlo draws of the model inputs. The evidence does not rank one route above the other ([no lead candidate](../README.md#no-lead-candidate)). Every route is a hypothesis for follow-up; the disclaimer in [section 7](../07-disclaimer-and-ai-use.md) applies.

## Feasibility frame

The child carries two alleles (copies of *BUB1B*): a nonsense allele (L737X, a premature stop codon in place of leucine 737) and a missense allele (N1002K, lysine in place of asparagine 1002). Every route below is measured against three quantities.

### Correction a therapy must reach

A dose-response model (mean division error against BubR1 level, fitted to ten published readouts from mouse fibroblasts, HeLa cells and patient lymphocytes; see [error-free division](../appendix/error-free-division.md)) gives the corrected fraction of dividing cells a therapy must reach. Carrier level is the division error rate of a healthy person with one working *BUB1B* copy. The second column counts cells that each receive one wild-type allele, and the third gives the average number of added wild-type alleles per cell if every cell receives a share.

| Target | Corrected fraction of dividing cells | Added wild-type alleles per cell |
|---|---|---|
| Halve the excess division error | about 0.5 (0.51 to 0.56) | 0.03 to 0.3 |
| Carrier-level error rate | 0.89 to 1.0 | 0.7 to 1.0 |

The fractions depend on the activity of the N1002K protein, which is unmeasured (section 1.7). At 30 percent activity or less, carrier level needs nearly every dividing cell corrected.

The model is extrapolated below 15 percent BubR1. Leave-one-dataset-out validation (refitting the model with one dataset withheld and predicting it) fails in 4 of 6 datasets, so the fractions are indicative.

### Cell compartments

Division flux, the number of cells replaced per day in each tissue, defines where a therapy must act. Sender and Milo 2021 (PubMed identifier, PMID [33432173](https://pubmed.ncbi.nlm.nih.gov/33432173/), abstract read) estimate 0.33 x 10^12 cells replaced per day, close to 90 percent of them blood cells.

The split of replaced cells by lineage (about 82 percent erythroid and neutrophil, about 11 percent gut epithelium, about 1 percent epidermis) is this report's own figure [UNVERIFIED: the paper's tables were not read].

Single-cell detection of *BUB1B* transcripts tracks cycling but sits near the dropout floor (transcripts that single-cell sequencing misses), so it cannot size the need [UNVERIFIED: analysis by this report of public single-cell data; dataset not recorded in the sources read].

### Delivery by division count

A non-integrating vector (a delivered gene copy that stays outside the chromosomes) halves in concentration at each division. Adeno-associated virus (AAV) vectors therefore suit tissues that divide at most about three times: heart and, in childhood, liver (Our inference; the division counts per compartment are assumptions). Marrow, growth plate, gut and skin need integrating or editing routes.

## Basis labels

Each mechanism step and each projected number on a card carries one of four labels:

- **Demonstrated:** shown by experiment in the cited paper, in the system named, with a control.
- **Suggested:** one method or research group, an association, or a different system from the child's cells.
- **Our inference:** derived by this report from cited facts or a model, with the assumption stated.
- **Speculation:** no supporting evidence found.

Each card names the system in which a step was shown. A step demonstrated in mouse remains untested in the child's cells.

## Candidates

Prime editing rewrites a DNA sequence at a chosen site without a double-strand break; ex vivo editing happens outside the body, and the edited cells are returned. Lentiviral add-back delivers a working copy of the gene with a lentivirus, a virus whose copy integrates into the chromosomes and passes to daughter cells.

| Route | Protein made | Projected ceiling | Card |
|---|---|---|---|
| Ex vivo prime-editing reversion in haematopoietic stem cells | wild-type BubR1 (leucine at position 737) from the edited allele | 15 to 24 percent cut in mean error at published efficiencies | [prime-editing-reversion.md](prime-editing-reversion.md) |
| Ex vivo lentiviral add-back in haematopoietic stem cells | wild-type BubR1 from the added copy, whichever allele the cell carries | 0.32 probability of reaching the needed engrafted fraction, against 0.05 for prime editing; blood cells only | [lentiviral-add-back.md](lentiviral-add-back.md) |

## Comparison

Expected effects are projections that depend on the unmeasured activity of the missense protein, described on each card. In the table, CD34+ cells are blood stem and progenitor cells, and K562 is a human leukaemia cell line.

| Route | Hypothesis | Expected effect (projection) | Evidence for | Evidence against | Safety | Test cost and first test |
|---|---|---|---|---|---|---|
| [Prime-editing reversion](prime-editing-reversion.md) | Reverting the stop to leucine in edited blood stem cells restores one wild-type allele | At the published median edit, the mean error halves with probability 0.04 (0.33 with the calibrated advantage); carrier level 0.001, assuming 0.1 missense activity | 23% median allele edit in published haematopoietic stem and progenitor cells; engraftment retention 0.74 to 1.05 | No stop-gain reversion in haematopoietic cells found; 0.17 to 0.25 of cells corrected (0.23 × 0.75 to 0.23 × 1.10) against 0.89 to 1.0 needed for carrier level | Conditioning; p53 and interferon response to prime editing | K562 knock-in and healthy CD34+ cell editing, weeks |
| [Lentiviral add-back](lentiviral-add-back.md) | An added wild-type *BUB1B* copy in autologous blood stem cells restores BubR1 whichever allele the cell carries | Engrafted fraction needed to remove 90 percent of the excess error reached with probability 0.32; blood correction addresses a median 0.037 of the documented disease burden | Integrating vector copies persist through division in Fanconi anaemia gene therapy; added BubR1 restores checkpoint function in cell lines | No BubR1 data in CD34+ cells; corrected-cell advantage is a calibration made for this report, 1 to 3 percent per division; one mouse source | Conditioning; boxed malignancy warnings on two approved lentiviral products; the one reported MVA transplant failed | Competitive growth of corrected and mutant CD34+ cells, weeks to months |

### Mechanism basis by candidate

The table counts each card's causal steps per label and names the weakest link, the least supported step.

| Route | Steps | Demonstrated | Suggested | Our inference | Speculation | Weakest link |
|---|---|---|---|---|---|---|
| [Prime-editing reversion](prime-editing-reversion.md) | 8 | 1 | 1 | 4 | 2 | No reversion of a stop codon in blood cells has been reported; the corrected-cell advantage is a calibration made for this report, and the probability of halving the mean error moves from 0.04 to 0.33 on that assumption |
| [Lentiviral add-back](lentiviral-add-back.md) | 7 | 1 | 2 | 1 | 3 | Whether corrected cells out-compete uncorrected ones in the child's marrow |

All routes in this section act through blood stem cells. A perfect correction of blood alone addresses a median 0.037 of the documented burden of biallelic *BUB1B* disease (range 0.016 to 0.098), and 0.17 of the mortality-linked features, in an accounting model built for this report on published case reports (see Other sources).

## Conditioning, transplant and malignancy precedents

- **Conditioning.** Autologous haematopoietic editing (editing of the patient's own blood stem cells) needs the native stem cells cleared, usually with busulfan (an alkylating drug, one that damages DNA). Engraftment, the settling and growth of the infused cells in the marrow, is the limiting constraint for an edited autologous product. Model estimates of the probability of reaching the engrafted fraction that removes 90 percent of the excess error are 0.05 for prime editing with busulfan and 0.32 for lentiviral add-back (a working gene copy delivered by a lentivirus) with busulfan.

- **Transplant in biallelic *BUB1B* disease.** A title and abstract search of Europe PMC (a literature database) on 2026-10-24 found one published transplant in a patient with biallelic *BUB1B* variants (variants on both gene copies): an 11-year-old with myelodysplasia (abnormal blood-cell production in the marrow). The matched unrelated donor graft followed treosulfan, fludarabine and thymoglobulin. The graft engrafted and was rejected on day 47. Aplasia (marrow failure) followed, and the patient died of infection on day 156 (PMID [31053147](https://pubmed.ncbi.nlm.nih.gov/31053147/), full text read).

- **Interpretation by the authors.** The authors discuss reduced-intensity conditioning, anti-human leukocyte antigen (HLA) antibodies and T-cell depletion of the graft as causes of rejection, and a contribution of defective *BUB1B*-mutant precursors.

- **Allogeneic transplant as reference.** Transplant of donor blood stem cells is the approved way to replace the marrow, and it needs no vector or edit. A donor graft acts on blood only, so it addresses the same median 0.037 of the documented burden as both routes. Donor, conditioning and timing are decisions for the treating team.

- **Donor-graft engraftment estimate.** The model behind the estimates of 0.05 and 0.32 gives 0.74 to 0.93 for a donor graft reaching the same need across three conditioning regimens, and the remaining probability is graft failure, as in the reported case (*Our inference from a model*). The donor-graft inputs are prior values from other diseases, and one of five leave-one-trial-out checks fails [UNVERIFIED: the model is not published with this report].

- **Malignancy warnings.** Approved haematopoietic gene therapies for adrenoleukodystrophy (Skysona) and sickle-cell disease (Lyfgenia) carry boxed warnings (the most prominent warning on a US label) for haematological malignancy (US Food and Drug Administration, FDA, labelling). MVA predisposes to cancer, and the one reported transplant recipient with biallelic *BUB1B* variants had a monosomy 7 clone (loss of one copy of chromosome 7) before transplant (PMID [31053147](https://pubmed.ncbi.nlm.nih.gov/31053147/)).

### Precedent products

AAV gene therapy (Zolgensma) carries a boxed warning for serious liver injury and acute liver failure with fatal outcomes (FDA label, read 2026-10-24).

The haematopoietic gene-therapy precedents read for this section fall into treated cohorts (with cohort size) and safety failures (with the finding).

| Kind | Condition | Product | Finding | Source |
|---|---|---|---|---|
| Treated cohort | Adenosine deaminase severe combined immunodeficiency (ADA-SCID) | Lentiviral gene therapy | 50 patients | PMID [33974366](https://pubmed.ncbi.nlm.nih.gov/33974366/), abstract read |
| Treated cohort | Metachromatic leukodystrophy | Haematopoietic gene therapy | 29 treated children | PMID [35065785](https://pubmed.ncbi.nlm.nih.gov/35065785/), abstract read |
| Treated cohort | Wiskott-Aldrich syndrome | Haematopoietic gene therapy | 8 treated children | PMID [30981783](https://pubmed.ncbi.nlm.nih.gov/30981783/), abstract read |
| Treated cohort | Fanconi anaemia, without conditioning | Haematopoietic gene therapy | 8 evaluable patients | PMID [39642902](https://pubmed.ncbi.nlm.nih.gov/39642902/), abstract read |
| Safety failure | Wiskott-Aldrich syndrome | Gammaretroviral gene therapy | Acute leukaemia in 7 of 10 patients | PMID [24622513](https://pubmed.ncbi.nlm.nih.gov/24622513/), abstract only |
| Safety failure | X-linked severe combined immunodeficiency | Haematopoietic gene therapy | Clonal T-cell proliferation tied to an *LMO2* insertion in the two youngest patients | PMID [14564000](https://pubmed.ncbi.nlm.nih.gov/14564000/), abstract only |
| Safety failure | X-linked chronic granulomatous disease | Haematopoietic gene therapy | Three- to four-fold expansion of gene-corrected myelopoiesis driven by oncogene insertions in two adults | PMID [16582916](https://pubmed.ncbi.nlm.nih.gov/16582916/), abstract only |

None of the precedents read combines a dividing target, a cell-autonomous protein, no demonstrated advantage of a corrected cell and cancer predisposition.

A Europe PMC title and abstract search of 2026-10-24 (BUB1B or BUBR1, with busulfan, alkylating, radiation, irradiation, radiosensitivity or chemosensitivity) found no study of the sensitivity of patient-derived or non-transformed *BUB1B*-deficient cells to alkylating drugs or radiation. One study in a paediatric glioblastoma cell line found that BubR1 knockdown with small interfering RNA sensitised the cells to gamma irradiation and, with temozolomide (also an alkylating drug), increased apoptosis (PMID [23728478](https://pubmed.ncbi.nlm.nih.gov/23728478/); abstract read).

## References

- Hacein-Bey-Abina S et al. (2003). LMO2-associated clonal T cell proliferation in two patients after gene therapy for SCID-X1. *Science*. PMID [14564000](https://pubmed.ncbi.nlm.nih.gov/14564000/)
- Ott MG et al. (2006). Correction of X-linked chronic granulomatous disease by gene therapy, augmented by insertional activation of MDS1-EVI1, PRDM16 or SETBP1. *Nat Med*. PMID [16582916](https://pubmed.ncbi.nlm.nih.gov/16582916/)
- Morales AG et al. (2013). BUB1 and BUBR1 inhibition decreases proliferation and colony formation, and enhances radiation sensitivity in pediatric glioblastoma cells. *Childs Nerv Syst*. PMID [23728478](https://pubmed.ncbi.nlm.nih.gov/23728478/)
- Braun CJ et al. (2014). Gene therapy for Wiskott-Aldrich syndrome--long-term efficacy and genotoxicity. *Sci Transl Med*. PMID [24622513](https://pubmed.ncbi.nlm.nih.gov/24622513/)
- Ferrua F et al. (2019). Lentiviral haemopoietic stem/progenitor cell gene therapy for treatment of Wiskott-Aldrich syndrome: interim results of a non-randomised, open-label, phase 1/2 clinical study. *Lancet Haematol*. PMID [30981783](https://pubmed.ncbi.nlm.nih.gov/30981783/)
- Laberko A et al. (2019). Hematopoietic stem cell transplantation in a patient with type 1 mosaic variegated aneuploidy syndrome. *Orphanet J Rare Dis*. PMID [31053147](https://pubmed.ncbi.nlm.nih.gov/31053147/)
- Sender R et al. (2021). The distribution of cellular turnover in the human body. *Nat Med*. PMID [33432173](https://pubmed.ncbi.nlm.nih.gov/33432173/)
- Kohn DB et al. (2021). Autologous Ex Vivo Lentiviral Gene Therapy for Adenosine Deaminase Deficiency. *N Engl J Med*. PMID [33974366](https://pubmed.ncbi.nlm.nih.gov/33974366/)
- Fumagalli F et al. (2022). Lentiviral haematopoietic stem-cell gene therapy for early-onset metachromatic leukodystrophy: long-term results from a non-randomised, open-label, phase 1/2 trial and expanded access. *Lancet*. PMID [35065785](https://pubmed.ncbi.nlm.nih.gov/35065785/)
- Río P et al. (2025). Haematopoietic gene therapy of non-conditioned patients with Fanconi anaemia-A: results from open-label phase 1/2 (FANCOLEN-1) and long-term clinical trials. *Lancet*. PMID [39642902](https://pubmed.ncbi.nlm.nih.gov/39642902/)

## Other sources

- SKYSONA (elivaldogene autotemcel), DailyMed set id f189502b-dc44-4289-99a6-cfba36918329 (Initial U.S. Approval 2022): boxed warning hematologic malignancy. Read 2026-10-24: https://dailymed.nlm.nih.gov/dailymed/lookup.cfm?setid=f189502b-dc44-4289-99a6-cfba36918329
- LYFGENIA (lovotibeglogene autotemcel), DailyMed set id 0d1b475e-5781-2bd1-e063-6294a90a7311 (Initial U.S. Approval 2023): boxed warning hematologic malignancy. Read 2026-10-24: https://dailymed.nlm.nih.gov/dailymed/lookup.cfm?setid=0d1b475e-5781-2bd1-e063-6294a90a7311
- ZOLGENSMA (onasemnogene abeparvovec-xioi), DailyMed set id 68cd4f06-70e1-40d8-bedb-609ec0afa471 (Initial U.S. Approval 2019): boxed warning serious liver injury and acute liver failure. Read 2026-10-24: https://dailymed.nlm.nih.gov/dailymed/lookup.cfm?setid=68cd4f06-70e1-40d8-bedb-609ec0afa471
- Model estimates (engraftment 0.05, 0.32 and 0.74 to 0.93; corrected-cell-fraction ranges): Monte Carlo models described on the prime-editing and lentiviral add-back cards of this section [UNVERIFIED: the models are not published with this report].
- Blood share of the documented burden (0.037, range 0.016 to 0.098; 0.17 for mortality-linked features): accounting model built for this report on a table of published biallelic *BUB1B* case reports [UNVERIFIED: the case table and the model are not published with this report].
