# Ex vivo lentiviral add-back of BUB1B

A lentiviral vector (a modified virus whose gene copy integrates into the chromosomes) can carry the 3,153-nucleotide *BUB1B* coding sequence into the patient's own (autologous) CD34+ blood stem and progenitor cells (identified by the surface protein CD34), which are transduced (given the vector) ex vivo (outside the body) and reinfused after conditioning (chemotherapy that clears native marrow cells). The added copy works with either of the child's two alleles.

Its reach is blood: haematopoietic correction addresses a median 0.037 of the documented disease burden (0.17 for mortality-linked features). A corrected cell gains an estimated 1 to 3 percent per division over an uncorrected one (0.7 to 3.4 across the modelled range of missense activity), so most models need conditioning to reach a useful corrected fraction. Two approved lentiviral stem-cell products carry boxed warnings for haematological malignancy, and the one reported transplant in a patient with biallelic *BUB1B* variants was rejected on day 47.

## Candidate

| Field | Content |
|---|---|
| Candidate | A self-inactivating lentiviral vector carrying the full-length *BUB1B* coding sequence (3,153 nucleotides, no introns) under a moderate promoter, applied ex vivo to autologous mobilised CD34+ cells |
| Status | Investigational. No *BUB1B* product exists. Lentiviral stem-cell products exist for other diseases; elivaldogene autotemcel (SKYSONA) and lovotibeglogene autotemcel (LYFGENIA) carry boxed warnings for haematological malignancy (US Food and Drug Administration, FDA, labels) |
| Route | Cell product reinfused after conditioning. The Fanconi anaemia-A trial reinfused without cytotoxic conditioning (PubMed identifier, PMID [39642902](https://pubmed.ncbi.nlm.nih.gov/39642902/)) |

## Hypothesis

A working copy of *BUB1B* in blood stem cells gives each transduced cell and its progeny BubR1 (the spindle checkpoint protein encoded by *BUB1B*) whichever alleles the child carries, and lowers their segregation error rate toward the carrier level.

*Speculation:* transduced cells engraft, outcompete uncorrected cells and lower aneuploidy in the blood lineage. The competitive advantage of a corrected cell is unmeasured in human cells and in the child's genotype.

Basis labels are defined in the [section 4 README](README.md#basis-labels): Demonstrated, Suggested, Our inference and Speculation.

| Step | Basis | System | Source |
|---|---|---|---|
| 1. An integrating lentiviral vector delivers a transgene to human blood stem cells and the copies persist through division | Demonstrated | Autologous FANCA-transduced CD34+ cells in 8 evaluable patients with Fanconi anaemia-A, infused without cytotoxic conditioning; at least 0.1 vector copies per nucleated cell at year 2 in 5 of 8 (median 0.18 in marrow); follow-up up to 7 years; a different disease, sponsor-funded; abstract read | PMID [39642902](https://pubmed.ncbi.nlm.nih.gov/39642902/) |
| 2. Added BubR1 restores checkpoint function in BubR1-deficient cells | Suggested | Fibroblast lines derived from patients with biallelic *BUB1B* mutations; transient plasmid expression of tagged BubR1 doubled the response to nocodazole, and in one patient line checkpoint activity returned almost to the parental level (Figure 1D, mean of 5 experiments); one research group; full text read. Section 1.4 records the same paper's overexpression experiments in HeLa and U2OS cells | PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/) |
| 3. A reachable expression level lies inside the useful window | Suggested | HeLa titration: about 13 percent of normal BubR1 gave near-normal segregation and about 6 percent gave errors in most cells. Mouse transgene lines at about 5-fold did not protect and at about 10-fold reduced tumours, with no rise in aneuploidy in fibroblasts and splenocytes; constitutive random-integration transgenes | PMIDs [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/), [23242215](https://pubmed.ncbi.nlm.nih.gov/23242215/) |
| 4. Added BubR1 lowers segregation errors in human CD34+ progenitors | Speculation | None; no BubR1 measurement in these cells | None |
| 5. A corrected cell gains about 1 to 3 percent per division over an uncorrected cell | Our inference | Lineage model calibrated on one mouse paper (3.4 percent at missense activity 0.1, 0.7 percent at 0.3); in that paper *Bub1b* hypomorph stem cells showed no defect in primary reconstitution and exhausted on serial transplantation | PMID [27313317](https://pubmed.ncbi.nlm.nih.gov/27313317/) |
| 6. The advantage exists in the child's genotype and permits engraftment with little or no conditioning | Speculation | None; Fanconi anaemia-A cells engrafted without conditioning (PMID [39642902](https://pubmed.ncbi.nlm.nih.gov/39642902/)), and that setting differs because those cells are sensitive to DNA crosslinks [UNVERIFIED: background knowledge, not a cited finding] | None |
| 7. Correcting blood benefits the child | Speculation | None; haematopoietic correction addresses a median 0.037 of documented disease burden (0.17 for mortality-linked features) | None |

Basis: 1 step Demonstrated (human, a different disease), 2 Suggested, 1 Our inference, 3 Speculation.

## Delivery and exposure

- **Vector fit** (*Our inference, computed from the reference sequence*). The coding sequence is 3,153 nucleotides and has no introns, so the vector carries it with room for a promoter, and the added copy escapes nonsense-mediated decay (the cell's degradation of messenger RNAs with premature stop codons), which acts on the stop allele.

- **Culture** (*Our inference*). Transduction needs several days of cytokine culture, which makes quiescent stem cells divide. A BubR1-low cell divides with more errors, and aneuploid stem cells compete poorly in vivo (relative fitness 0.08 for trisomy 16; PMID [27313317](https://pubmed.ncbi.nlm.nih.gov/27313317/)), so the infused product may be depleted of its best cells.

- **Conditioning** (*Our inference from a model; the Fanconi anaemia trial is Demonstrated*). The model probability that the achieved engrafted fraction meets the need for removing 90 percent of the excess error is in the table under Expected effect (0.32 with busulfan; the prime-editing card gives 0.05 with busulfan). The needed fraction is a median 0.72 to 0.78 of stem cells fully corrected for 90 percent and 0.35 to 0.38 for half.

- **Conditioning in Fanconi anaemia** (*Demonstrated*). The trial reinfused cells without cytotoxic conditioning; the limits on efficacy are under Evidence against.

- **Expression control** (*design options, all untested for BubR1*). Overexpression of the checkpoint proteins Mad2 and Bub1 caused tumours in mice (PMIDs [17189715](https://pubmed.ncbi.nlm.nih.gov/17189715/), [21646403](https://pubmed.ncbi.nlm.nih.gov/21646403/)), and the safe ceiling for BubR1 is unmeasured. Three designs would control the dose.

  - A dose-limited cassette: a 352-base-pair fragment of the *BUB1B* promoter with a truncated 5' untranslated region, tested against promoters of rising strength (PGK, EFS, high-EF1a) so a cell assay reads the window from 0.5 to 10 times one allele. Computed from the reference sequence; a packaging control failed for one of the vectors in our design check [UNVERIFIED: the check is not published with this report].

  - A cell-cycle-gated promoter: the *BUB1B* promoter needs a CDE-CHR element (a cell-cycle-dependent promoter element) for G2/M-specific transcription (PMID [17478512](https://pubmed.ncbi.nlm.nih.gov/17478512/); abstract read; a 464-bp fragment was tested), CHR elements bind the MYBL2- and FOXM1-containing complexes (PMID [25106871](https://pubmed.ncbi.nlm.nih.gov/25106871/); abstract read). Public single-cell data show *BUB1B* tracking a G2/M index [UNVERIFIED: dataset not recorded in the sources read]. A payload under it would express in cycling cells, which are the cells that need BubR1. The prediction of at least ten-fold higher expression in cycling than quiescent cells is untested.

  - A drug-gated degron (a protein segment that targets its protein for degradation): the *Escherichia coli* dihydrofolate reductase (DHFR) destabilising domain fused to BubR1 makes the protein depend on trimethoprim. The domain was reported in rodent brain with another protein [UNVERIFIED: primary paper not re-read]. Trimethoprim is a folate antagonist, and an 18-kilodalton fusion on a protein that carries degrons is untested.

- **Transplant in the disease** (*Demonstrated for one allogeneic case*). The only transplant reported in a patient with biallelic *BUB1B* variants was an unrelated-donor graft that was rejected on day 47; the patient died of infection on day 156 (PMID [31053147](https://pubmed.ncbi.nlm.nih.gov/31053147/), full text read; details in the [section 4 README](README.md#conditioning-transplant-and-malignancy-precedents)).

## Evidence for

- Added BubR1 restored checkpoint activity in fibroblast lines from patients with biallelic *BUB1B* mutations, and the authors conclude that BubR1 dysfunction causes the segregation errors (PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/); full text read). The expression was transient and from a plasmid, a weaker test of a stable lentiviral copy.

- Lentiviral add-back kept the vector in human blood stem cells for years. In the Fanconi anaemia-A trial, 5 of 8 evaluable patients reached at least 0.1 vector copies per nucleated cell at year 2 without conditioning, and no genotoxic event related to the therapy appeared in follow-up of up to 7 years (PMID [39642902](https://pubmed.ncbi.nlm.nih.gov/39642902/); abstract read; sponsor-funded). A systematic review of seven studies found stable polyclonal patterns and no clonal dominance (PMID [41991439](https://pubmed.ncbi.nlm.nih.gov/41991439/); abstract read, high risk of bias).

- Raising BubR1 to about 10 times normal reduced tumours and extended lifespan in mice, with no rise in aneuploidy in fibroblasts and splenocytes (3 samples per genotype; PMID [23242215](https://pubmed.ncbi.nlm.nih.gov/23242215/); full text read; one research group).

- Aneuploid stem cells lose competitive fitness, and hypomorph stem cells exhausted on serial transplantation, with the authors stating that repeated challenge is needed to reveal the defect (PMID [27313317](https://pubmed.ncbi.nlm.nih.gov/27313317/); full text read). This predicts an advantage for corrected cells under replicative stress (Our inference).

- The added copy functions independently of both variants (*Our inference*), so the route works with either allele and with any activity of the missense protein.

## Evidence against

- No *BUB1B* add-back has been tested in blood stem cells, and the effect of added BubR1 on their segregation error rate is unmeasured (step 4).

- The calibrated advantage is small and rests on one mouse paper. A model puts the 5-to-50-percent takeover of the stem-cell pool at 56 years at missense activity 0.1 and 283 years at 0.3 (*Our inference*). In the same paper hypomorph stem cells competed normally in primary reconstitution (PMID [27313317](https://pubmed.ncbi.nlm.nih.gov/27313317/)). The Fanconi anaemia-A result belongs to a disease where the corrected cell resists DNA crosslinks, a different advantage.

- Haematopoietic correction addresses a median 0.037 of documented disease burden (range 0.016 to 0.098; 0.17 for mortality-linked features). A decision model that weighs benefit against conditioning harm reaches break-even only if blood carries 0.80 to 0.90 of the benefit (*Our inference*).

- The mouse dose data come from random-integration transgenes. The line at about 5-fold did not protect. Bone-marrow and small-intestine aneuploidy was unchanged at 10-fold, and spontaneous tumours lost transgene expression (PMID [23242215](https://pubmed.ncbi.nlm.nih.gov/23242215/)). A physiological promoter may not reach the protective range.

- Efficacy in Fanconi anaemia was greater in younger patients and in those without advanced marrow failure (PMID [41991439](https://pubmed.ncbi.nlm.nih.gov/41991439/)).

- The sensitivity of patient-derived or non-transformed *BUB1B*-deficient cells to alkylators or radiation has no study in Europe PMC (searched 2026-10-24), so conditioning toxicity in this host is unmeasured. The one study found, BubR1 knockdown in a paediatric glioblastoma cell line, reports sensitisation to irradiation and, with temozolomide, more apoptosis (PMID [23728478](https://pubmed.ncbi.nlm.nih.gov/23728478/); abstract read).

- No independent research group has tested *BUB1B* add-back in blood stem cells, and one group produced the BubR1 dose papers.

## Safety

- Insertional oncogenesis (cancer triggered by vector integration into the genome) is on the labels of approved lentiviral stem-cell products; SKYSONA and LYFGENIA carry boxed warnings for haematological malignancy (FDA labels). The host is cancer-predisposed with a checkpoint-weak marrow (Gate 4 strained).

- Conditioning with an alkylating drug damages DNA in a host whose sensitivity is unmeasured, and BubR1 knockdown sensitised a glioblastoma cell line to irradiation (Gate 1 strained). Culture forces a checkpoint-weak progenitor through divisions (Gate 2 strained).

- Lentiviral stem-cell products are approved in children, and no *BUB1B* product exists (Gate 3). No long-term data exist for a one-time infusion of a *BUB1B* product.

- Overshoot: BubR1 at about 10 times normal was tumour-protective in mice, while overexpression of Mad2 and Bub1 was oncogenic; the human ceiling is unmeasured.

- Check against the child's other genetic findings: pending, gene by gene ([section 3 README](../03-approved-drugs/README.md#check-against-the-childs-other-genetic-findings)).

## Expected effect

*Every figure is Our inference: a model projection that rests on the activity of the missense protein, which is unmeasured, and on the blood share of the burden.*

| Conditioning | Probability that engraftment meets the need for 90 percent of the excess error removed |
|---|---|
| Busulfan | 0.32 |
| Antibody-based | 0.10 |
| None | 0.04 |

- A transduced cell carries one added copy at a dose set by the promoter. The test window for the dose is 0.5 to 2 times a normal allele (a design choice, Speculation).

- Tissues outside the blood lineage, the two variant alleles and tumour risk in non-haematopoietic tissue stay unchanged. The blood share of the burden is under Evidence against.

- **Weakest link.** Step 6: whether a corrected cell outcompetes an uncorrected one in the child's marrow. Without conditioning the probability of reaching the need is 0.04 (table above).

## Test

| Stage | Measurement | Pass criterion | Stopping criterion |
|---|---|---|---|
| 0 | Cassette arms (native fragment, PGK, EFS, high-EF1a) in the titratable *BUB1B*-tagged cell line: BubR1 level and segregation errors | An arm gives 0.5 to 2 times normal BubR1 with errors at carrier level | Errors above the untreated arm at any dose |
| 1 | Competitive growth of vector-carrying against uncorrected BubR1-depleted healthy-donor CD34+ cells, 14 days | Corrected share rises at least 1.3-fold over 10 divisions (about 3 percent per division) | Rise of 1.1-fold or less (about 1 percent per division) |
| 2 | Vector copy number and BubR1 level in transduced CD34+ cells | 1 to 3 copies per cell; BubR1 0.5 to 2 times control | Below 0.3 or above 4 times control |
| 3 | Segregation errors and micronuclei in transduced CD34+ progeny by live imaging | At carrier level or lower | Any rise above untransduced cells |
| 4 | Engrafted transduced cells in immunodeficient mice at 16 weeks against input | Retention at least 0.7 | Below 0.5 |

All thresholds are proposals fixed before any experiment. Stage 1 measures the advantage that the Expected effect table assumes, and stage 3 applies the stopping criterion for any rise in aneuploidy or micronuclei. The shared cell system is in [computational findings](../05-computational-findings.md#510-experimental-platform-shared-by-sections-3-and-4).

## Outcome if confirmed

A pass at stages 1 to 3 would show that added BubR1 corrects blood stem cells and that corrected cells hold an advantage. The share of the disease burden that lives in blood (Evidence against) then limits the benefit the route can give.

## References

- Myslinski E et al. (2007). Transcription of the human cell cycle regulated BUB1B gene requires hStaf/ZNF143. *Nucleic Acids Res*. PMID [17478512](https://pubmed.ncbi.nlm.nih.gov/17478512/)
- Sotillo R et al. (2007). Mad2 overexpression promotes aneuploidy and tumorigenesis in mice. *Cancer Cell*. PMID [17189715](https://pubmed.ncbi.nlm.nih.gov/17189715/)
- Suijkerbuijk SJ et al. (2010). Molecular causes for BUBR1 dysfunction in the human cancer predisposition syndrome mosaic variegated aneuploidy. *Cancer Res*. PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/)
- Ricke RM et al. (2011). Bub1 overexpression induces aneuploidy and tumor formation through Aurora B kinase hyperactivation. *J Cell Biol*. PMID [21646403](https://pubmed.ncbi.nlm.nih.gov/21646403/)
- Morales AG et al. (2013). BUB1 and BUBR1 inhibition decreases proliferation and colony formation, and enhances radiation sensitivity in pediatric glioblastoma cells. *Childs Nerv Syst*. PMID [23728478](https://pubmed.ncbi.nlm.nih.gov/23728478/)
- Baker DJ et al. (2013). Increased expression of BubR1 protects against aneuploidy and cancer and extends healthy lifespan. *Nat Cell Biol*. PMID [23242215](https://pubmed.ncbi.nlm.nih.gov/23242215/)
- Müller GA et al. (2014). The CHR site: definition and genome-wide identification of a cell cycle transcriptional element. *Nucleic Acids Res*. PMID [25106871](https://pubmed.ncbi.nlm.nih.gov/25106871/)
- Pfau SJ et al. (2016). Aneuploidy impairs hematopoietic stem cell fitness and is selected against in regenerating tissues in vivo. *Genes Dev*. PMID [27313317](https://pubmed.ncbi.nlm.nih.gov/27313317/)
- Laberko A et al. (2019). Hematopoietic stem cell transplantation in a patient with type 1 mosaic variegated aneuploidy syndrome. *Orphanet J Rare Dis*. PMID [31053147](https://pubmed.ncbi.nlm.nih.gov/31053147/)
- Río P et al. (2025). Haematopoietic gene therapy of non-conditioned patients with Fanconi anaemia-A: results from open-label phase 1/2 (FANCOLEN-1) and long-term clinical trials. *Lancet*. PMID [39642902](https://pubmed.ncbi.nlm.nih.gov/39642902/)
- Cano Reyes SE et al. (2026). Efficacy and safety of gene therapy in pediatric patients with Fanconi anemia: a systematic review. *An Pediatr (Engl Ed)*. PMID [41991439](https://pubmed.ncbi.nlm.nih.gov/41991439/)

## Other sources

- SKYSONA (elivaldogene autotemcel), DailyMed set id f189502b-dc44-4289-99a6-cfba36918329: boxed warning, haematological malignancy. https://dailymed.nlm.nih.gov/dailymed/lookup.cfm?setid=f189502b-dc44-4289-99a6-cfba36918329

- LYFGENIA (lovotibeglogene autotemcel), DailyMed set id 0d1b475e-5781-2bd1-e063-6294a90a7311: boxed warning, haematological malignancy. https://dailymed.nlm.nih.gov/dailymed/lookup.cfm?setid=0d1b475e-5781-2bd1-e063-6294a90a7311

- Coding sequence length (3,153 nucleotides, 1,050 residues, 23 exons in the genomic transcript) and absence of introns in the coding sequence: Ensembl canonical transcript ENST00000287598, queried through Ensembl REST on 2026-10-24.

- Engraftment probabilities (0.32, 0.10, 0.04), the needed fractions, the per-division advantage and the takeover times: Monte Carlo models of conditioning, engraftment and competition whose inputs are the cited trials and one mouse paper [UNVERIFIED: the models are not published with this report].

- Blood share of the documented burden (0.037; 0.17 for mortality-linked features): estimate by this report from a case table dominated by kidney tumours [UNVERIFIED: the table and the accounting model are not published with this report].
