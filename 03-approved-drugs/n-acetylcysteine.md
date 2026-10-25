# N-acetylcysteine and ascorbate

## Candidate

N-acetylcysteine (NAC) is an approved antidote for paracetamol overdose (Acetadote label) and a mucolytic (a medicine that thins mucus; PubMed identifier, PMID [41312188](https://pubmed.ncbi.nlm.nih.gov/41312188/)). The injection label bases paediatric use on clinical practice, and oral use in children is documented in a narrative review (same PMID).

Ascorbic acid (vitamin C) has an injectable product (Ascor) approved by the US Food and Drug Administration (FDA). It is a short-term (up to one week) intravenous treatment for scurvy (vitamin C deficiency) in patients aged 5 months and older (openFDA label).

This card covers oral NAC and ascorbate as two antioxidants that act on one mechanism. Use in mosaic variegated aneuploidy (MVA, a syndrome in which cells carry varying chromosome numbers) would be off-label (outside the approved indications).

## Hypothesis

Oxidative stress (an excess of reactive oxygen species, ROS, over antioxidant defences) lowers the recruitment of BubR1, the protein encoded by *BUB1B*, to kinetochores (the sites on chromosomes where spindle fibres attach). It also weakens the spindle assembly checkpoint (the control that delays chromosome separation until every chromosome is attached to the spindle), the checkpoint that the two *BUB1B* variants weaken as well.

A cell with a small BubR1 reserve tolerates a second insult poorly, so reducing oxidative stress could preserve the checkpoint function that remains.

Each row of the table is one causal step, with a basis label defined in the [section 3 README](README.md#basis-labels): Demonstrated, Suggested, Our inference or Speculation.

| Step | Basis | System | Source |
|---|---|---|---|
| 1. NAC or ascorbate raises antioxidant capacity in dividing tissues (marrow, growth plate) | Our inference | Derived from the glutathione-precursor pharmacology of NAC (glutathione is the main small-molecule antioxidant in cells); tissue exposure of either agent is unmeasured; oral ascorbate absorption saturates | Acetadote label (glutathione); PMID [8623000](https://pubmed.ncbi.nlm.nih.gov/8623000/) (ascorbate absorption); PMID [41312188](https://pubmed.ncbi.nlm.nih.gov/41312188/) (paediatric use only) |
| 2. Oxidative stress lowers BubR1 at kinetochores | Suggested | Sod1-knockout mouse oocytes (lacking the antioxidant enzyme superoxide dismutase 1) matured in vitro at 21% oxygen, meiosis I (the first division of egg maturation), normal *Bub1b*; full text read | PMID [39845481](https://pubmed.ncbi.nlm.nih.gov/39845481/) |
| 3. Ascorbate or NAC lowers segregation errors in that setting | Suggested | Same oocyte model; ascorbate in room-air medium can itself generate peroxide, so a culture artefact is possible | PMID [39845481](https://pubmed.ncbi.nlm.nih.gov/39845481/); PMID [24923566](https://pubmed.ncbi.nlm.nih.gov/24923566/) |
| 4. Oxidative stress harms a BubR1-deficient animal | Suggested | Mice with 20% of normal BubR1 given potassium bromate alone; higher death rate than wild type; abstract read | PMID [27815460](https://pubmed.ncbi.nlm.nih.gov/27815460/) |
| 5. Oxidative stress lowers BubR1 and weakens mitotic arrest in somatic cells | Suggested | Human umbilical-cord mesenchymal stem cells from three donors, hydrogen peroxide and late passage as the only exposures, normal BubR1 genotype; full text partly read | PMID [37094517](https://pubmed.ncbi.nlm.nih.gov/37094517/) |
| 6. A measurable oxidative share of the BubR1 deficit exists in the child's cells | Speculation | Unmeasured in MVA and in BubR1-deficient human cells | None |
| 7. Missegregation falls as BubR1 rises from the estimated 0.23 of normal, by at most 51% per chromosome in the model, so restoring BubR1 could lower the error rate | Our inference | Dose-response model fitted to ten published readouts (appendix); model estimate | [Error-free division](../appendix/error-free-division.md) |
| 8. An antioxidant restores checkpoint function in BubR1-deficient cells | Speculation | No antioxidant tested in any BubR1-deficient system | None |
| 9. The antioxidant leaves intact the tumour barrier formed by p53 (a tumour-suppressor protein) | Speculation | NAC and vitamin E accelerated BRAF- and KRAS-driven lung cancer in mice by lowering p53 signalling (a contrary finding, Suggested; abstract read) | PMID [24477002](https://pubmed.ncbi.nlm.nih.gov/24477002/) |

Basis: 0 steps Demonstrated, 4 Suggested, 2 Our inference, 3 Speculation. Weakest link: step 6, because every supporting experiment used cells with normal BubR1 or contained no antioxidant.

## Delivery and exposure

NAC is given orally or intravenously and acts systemically as a cysteine donor for glutathione synthesis (Acetadote label, sections 12.1 and 12.3).

Oral NAC has documented paediatric use in respiratory disease (Suggested: narrative review, abstract read). A 2025 narrative review reports that most trial participants were older than 9 years and that evidence on dosing in younger children is lacking (PMID [41312188](https://pubmed.ncbi.nlm.nih.gov/41312188/)).

Intracellular exposure in marrow, growth plate or other mitotic tissues is unmeasured for either agent [no basis for tissue reach: Speculation]. Ascorbate absorption from the gut saturates: in seven healthy volunteers plasma concentration saturated at 1,000 mg daily and bioavailability fell at single doses of 500 mg and above (PMID [8623000](https://pubmed.ncbi.nlm.nih.gov/8623000/); abstract read). The labelled product is intravenous (openFDA label, see Other sources).

The effect depends on a local oxidative burden, which is unmeasured in MVA, so tissue reach matters more than plasma level.

The oocyte rescue used 500 µM ascorbate or 500 µM NAC in the culture medium (PMID [39845481](https://pubmed.ncbi.nlm.nih.gov/39845481/); full text read). A single intravenous ascorbate dose of 1,000 mg, five times the largest labelled single dose, gave a mean peak of 436.2 µM in eight healthy adults (Ascor label), so the assay concentration is 1.15 times that peak (500 / 436.2; Our inference).

## Evidence for

- Sod1-knockout mouse oocytes matured in vitro at 21% oxygen show more chromosome misalignment and segregation errors and less BubR1 recruited to kinetochores in meiosis I; adding ascorbate or NAC lowered the segregation-error frequency (PMID [39845481](https://pubmed.ncbi.nlm.nih.gov/39845481/); full text read).
  - The full text is narrower than the abstract. With the antioxidants (50 Sod1-knockout oocytes untreated, 39 with ascorbate, 52 with NAC), the share of oocytes with the normal 20 chromosomes rose and premature separation of sister chromatids fell. The shares with 19 or fewer or 21 or more chromosomes did not differ (Figure 7B).
  - Kinetochore BubR1 was not measured under the antioxidants.
  - The oocytes carry normal *Bub1b*, so the model tests an oxidative insult in cells with normal BubR1. Meiosis I differs from somatic mitosis (the division of body cells).
- Mice expressing 20% of normal BubR1 (hypomorphs: animals with reduced gene function) died at a higher rate than wild-type mice under an oxidative stressor (potassium bromate, 2 g/l in drinking water for 16 weeks; p = 0.0082), and the authors suggest splenic neoplasms as the cause (PMID [27815460](https://pubmed.ncbi.nlm.nih.gov/27815460/); abstract read; animal numbers not in the abstract). The abstract describes a stressor-only comparison, so the study shows that oxidative stress harms the hypomorph; the effect of an antioxidant is untested there.
- In primary human umbilical-cord mesenchymal stem cells (cultures from three donors), young cells exposed to hydrogen peroxide and late-passage cells failed to hold mitotic arrest in the presence of spindle poisons. BubR1 first rose and then fell through autophagy-dependent degradation (autophagy is the cell's recycling of its own components) (PMID [37094517](https://pubmed.ncbi.nlm.nih.gov/37094517/); full text partly read). The model system is senescence (permanent arrest of cell division) and ageing in cells with normal BubR1 genotype; the only exposures were oxidant and late passage.
- In a 12-week randomised trial of low-dose antioxidants (alpha-tocopherol 100 mg, beta-carotene 6 mg, vitamin C 100 mg, selenium 50 microgram daily) in middle-aged men, lymphocyte micronuclei (small extra nuclei, a marker of chromosome loss or breakage) rose in the placebo group (P = 0.04) and not in the supplemented group. In the 28 myocardial-infarction survivors who completed the study, micronucleus frequency fell, with the largest fall at normal folate (P = 0.015) (PMID [15548759](https://pubmed.ncbi.nlm.nih.gov/15548759/); abstract read). The trial was small, used a multi-ingredient mix without NAC and enrolled middle-aged men with cardiovascular risk.

## Evidence against

- No antioxidant drug has been tested in any BubR1-deficient system. The only drug-level rescue is the oocyte result at 21% oxygen. Ascorbate and other antioxidants added to culture medium can themselves generate hydrogen peroxide and degradation products, which have produced artefacts in published cell studies (PMID [24923566](https://pubmed.ncbi.nlm.nih.gov/24923566/); abstract read), so the rescue may be a culture artefact.
- Independence: the oocyte rescue (PMID [39845481](https://pubmed.ncbi.nlm.nih.gov/39845481/)), the hypomorph mouse stressor study (PMID [27815460](https://pubmed.ncbi.nlm.nih.gov/27815460/)) and the senescence study (PMID [37094517](https://pubmed.ncbi.nlm.nih.gov/37094517/)) come from three groups with separate author lists, and each group tested one step of the chain. No study tests the whole chain, and no paper reports an MVA patient or cell line.
- In a *Drosophila* model of MVA microcephaly, overexpressing the ROS scavengers Sod2 and GTPx-1 partly restored the number of aneuploid (abnormal chromosome number) neural stem cells and fully restored brain size (PMID [41820377](https://pubmed.ncbi.nlm.nih.gov/41820377/); full text read). The depleted checkpoint genes were *bub3* or *rod*, and the antioxidant intervention was genetic overexpression. Blocking apoptosis (programmed cell death) with p35 also restored brain size completely without restoring stem-cell numbers.
- The fly result supports tolerance of aneuploid cells; protection of BubR1 is outside what it tests. Sod2 acts in mitochondria, whereas NAC and ascorbate act mainly in cytosol and plasma.
- NAC and vitamin E accelerated BRAF- and KRAS-driven lung cancer in mice by lowering ROS, DNA damage and p53 expression (PMID [24477002](https://pubmed.ncbi.nlm.nih.gov/24477002/); abstract read; somatic lung model). Human RPE1 cells (a retinal pigment epithelial line) that missegregate chromosomes arrest through p53, activated by DNA damage (PMID [28633018](https://pubmed.ncbi.nlm.nih.gov/28633018/); full text read). An antioxidant that lowers DNA damage and p53 signalling may therefore weaken that arrest and a tumour barrier (Our inference from two papers; the lung study did not involve *BUB1B*).
- The fly study also partly rescued the number of aneuploid neuroblasts (fly neural stem cells) by depleting TOR (target of rapamycin) or treating with rapamycin, while brain size stayed small (PMID [41820377](https://pubmed.ncbi.nlm.nih.gov/41820377/)). Rapamycin induces autophagy, and autophagy-dependent BubR1 degradation (PMID [37094517](https://pubmed.ncbi.nlm.nih.gov/37094517/)) suggests it could lower BubR1 (Our inference from two papers).

## Safety

Gate numbers follow the seven-gate screen in [Screening criteria](README.md#screening-criteria).

- Gate 1 (genotoxicity) flag: the NAC injection label (Acetadote) reports negative results in the Ames test (a bacterial mutation assay) and the in vivo mouse micronucleus test, and a positive result in the in vitro mouse lymphoma forward-mutation test (openFDA label, see Other sources). The ascorbate label was not re-read.
- Gate 2 (aneugenicity) passes; the hypothesis under test is that the candidate protects checkpoint function (step 8, Speculation).
- Gate 3 (paediatric exposure) passes with a caveat. The NAC injection label bases use in patients of 5 kg and above on clinical practice. A 2025 narrative review reports oral NAC as generally effective and well tolerated in children, with most participants older than 9 years (PMID [41312188](https://pubmed.ncbi.nlm.nih.gov/41312188/)). The FDA-approved ascorbate product (Ascor) is a short-term intravenous scurvy treatment with an oxalate-nephropathy warning (kidney injury from oxalate crystals; openFDA label).
- Gate 4 (cancer direction) flag, unresolved. A 2026 narrative review argues that oral vitamin C, NAC and other supplements can act as tumour suppressors or promoters depending on dose, route and disease stage (PMID [42510540](https://pubmed.ncbi.nlm.nih.gov/42510540/); abstract read). The mouse lung result above is the specific mechanism of concern, and the BubR1-insufficient mouse result points toward benefit.
- Gate 5 (chronic-use tolerability): the oral NAC review reports good tolerability in children for the doses and durations studied (PMID [41312188](https://pubmed.ncbi.nlm.nih.gov/41312188/); abstract read). The ascorbate label limits use to one week and warns of oxalate nephropathy after prolonged high-dose infusion (Ascor label).
- Gate 6 (interactions) flag: in 1,134 patients with breast cancer in a prospective cohort ancillary to a chemotherapy trial, use of any antioxidant supplement (vitamins A, C and E, carotenoids, coenzyme Q10) before and during chemotherapy was associated with an adjusted hazard ratio of 1.41 for recurrence (95% CI 0.98 to 2.04; P = 0.06, so not significant). The study was observational, and its list of supplements excludes NAC (PMID [31855498](https://pubmed.ncbi.nlm.nih.gov/31855498/); abstract read).
  - A 2026 narrative review proposes NAC as a redox-modulating adjunct in paediatric acute lymphoblastic leukaemia, concludes that NAC can reduce treatment toxicity without consistently compromising antitumour efficacy, and states that evidence is limited (PMID [42199526](https://pubmed.ncbi.nlm.nih.gov/42199526/); abstract read).
- Check against the child's other genetic findings (the secondary finding and the four unnamed carrier-state variants): pending, gene by gene ([section 3 README](README.md#check-against-the-childs-other-genetic-findings)).

## Expected effect

If oxidative stress removes part of the kinetochore BubR1 that the two alleles supply, an antioxidant would restore some of it and lower the per-chromosome missegregation probability [projection, Speculation: step 8]. The size of the gain is bounded by the share of the BubR1 deficit that is oxidative. That share is unmeasured, so no numeric range is supported [Speculation].

In the [error-free division](../appendix/error-free-division.md) model the child's estimated missegregation rate at 0.23 of normal BubR1 is 1.27 × 10⁻³ per chromosome, and the baseline at normal BubR1 is 6.2 × 10⁻⁴. Complete restoration would therefore lower the rate by at most 51% (1 − 6.2 / 12.7), and the unmeasured oxidative share decides how much of that is reached [Our inference: step 7].

The candidate would be expected to leave unchanged the BubR1 level that the genotype sets, aneuploidy that has already occurred and any tissue it does not reach [Our inference].

If antioxidants also lower p53 signalling, errors could fall while the tumour barrier weakens [Speculation: step 9; stopping criterion below].

## Test

- **System:** patient-derived cells and isogenic cell lines (lines that differ only in the BubR1 variant) with a BubR1 hypomorph and carrier controls, each cultured at 3% and 20% oxygen.
- **Readout:** mitochondrial ROS (MitoSOX, a mitochondrial superoxide dye) and cytosolic ROS (H2DCF, a general ROS dye), kinetochore BubR1 by immunofluorescence, expression of p21 (a cell-cycle inhibitor switched on by p53) and other p53 targets, premature chromatid separation rate (sister chromatids parting before anaphase) and micronucleus frequency, each with and without NAC or ascorbate.
- **Exposure:** concentrations within plasma exposure at the labelled paediatric regimen [UNVERIFIED: the value is not yet sourced here].
- **Pass criterion (fixed before the experiment):** raised ROS or lowered kinetochore BubR1 in patient cells relative to carrier controls at 3% oxygen, and a drug-induced fall in segregation errors at both oxygen tensions with p21 unchanged or higher.
- **Stopping criterion:** normal ROS and kinetochore BubR1 against carrier controls at 3% oxygen; no effect at 3% oxygen; or errors fall together with a proportional fall in p21, which would signal a loss of the p53 barrier.

## Outcome if confirmed

A measured oxidative component in BubR1-deficient cells and an approved, paediatric-labelled agent with a defined cancer-direction test. A negative first measurement removes the target after one ROS and kinetochore panel.

Shared cell systems: [computational findings](../05-computational-findings.md). Disclaimer: [disclaimer and AI-use disclosure](../07-disclaimer-and-ai-use.md).

## References

- Levine M et al. (1996). Vitamin C pharmacokinetics in healthy volunteers: evidence for a recommended dietary allowance. *Proc Natl Acad Sci U S A*. PMID [8623000](https://pubmed.ncbi.nlm.nih.gov/8623000/)
- Smolková B et al. (2004). Folate levels determine effect of antioxidant supplementation on micronuclei in subjects with cardiovascular risk. *Mutagenesis*. PMID [15548759](https://pubmed.ncbi.nlm.nih.gov/15548759/)
- Sayin VI et al. (2014). Antioxidants accelerate lung cancer progression in mice. *Sci Transl Med*. PMID [24477002](https://pubmed.ncbi.nlm.nih.gov/24477002/)
- Halliwell B (2014). Cell culture, oxidative stress, and antioxidants: avoiding pitfalls. *Biomed J*. PMID [24923566](https://pubmed.ncbi.nlm.nih.gov/24923566/)
- Matsuda D et al. (2016). BUBR1 Insufficiency in Mice Increases their Sensitivity to Oxidative Stress. *In Vivo*. PMID [27815460](https://pubmed.ncbi.nlm.nih.gov/27815460/)
- Santaguida S et al. (2017). Chromosome Mis-segregation Generates Cell-Cycle-Arrested Cells with Complex Karyotypes that Are Eliminated by the Immune System. *Dev Cell*. PMID [28633018](https://pubmed.ncbi.nlm.nih.gov/28633018/)
- Ambrosone CB et al. (2020). Dietary Supplement Use During Chemotherapy and Survival Outcomes of Patients With Breast Cancer Enrolled in a Cooperative Group Clinical Trial (SWOG S0221). *J Clin Oncol*. PMID [31855498](https://pubmed.ncbi.nlm.nih.gov/31855498/)
- Goutas A et al. (2023). The establishment of mitotic errors-driven senescence depends on autophagy. *Redox Biol*. PMID [37094517](https://pubmed.ncbi.nlm.nih.gov/37094517/)
- Nago M et al. (2025). Sod1 deficiency in mouse oocytes during in vitro maturation increases chromosome segregation errors with a reduced BUBR1 at kinetochore. *Reprod Med Biol*. PMID [39845481](https://pubmed.ncbi.nlm.nih.gov/39845481/)
- Benedetti F et al. (2025). N-acetylcysteine in paediatrics: a review of efficacy, safety and dosing strategies in respiratory care. *Drugs Context*. PMID [41312188](https://pubmed.ncbi.nlm.nih.gov/41312188/)
- González-Blanco A et al. (2026). Proteostasis failure and mitochondrial dysfunction contribute to chromosomal instability-induced microcephaly. *Nat Commun*. PMID [41820377](https://pubmed.ncbi.nlm.nih.gov/41820377/)
- Soetadji RS et al. (2026). Chemotherapy-induced oxidative injury in pediatric acute lymphoblastic leukemia: The role of N-acetylcysteine (Review). *Biomed Rep*. PMID [42199526](https://pubmed.ncbi.nlm.nih.gov/42199526/)
- Martinez P et al. (2026). The Redox Paradox of Natural Supplements in Cancer: A Narrative Review to Guide Clinical Practice. *Antioxidants (Basel)*. PMID [42510540](https://pubmed.ncbi.nlm.nih.gov/42510540/)

## Other sources

- Acetylcysteine injection (Acetadote), prescribing information, openFDA drug label API, effective 2025-04-30, set id 472f158a-5ab9-4308-8e49-1116e6ea3d39, read 2026-10-24: section 13.1 genotoxicity statements and the paediatric-use sentence for patients of 5 kg and above. https://api.fda.gov/drug/label.json?search=openfda.brand_name:Acetadote
- Ascorbic acid injection (Ascor), prescribing information, openFDA drug label API, effective 2026-05-29, set id 388aad52-fc01-4784-9791-1dbc80c69306, read 2026-10-24: indication (short-term treatment of scurvy from age 5 months) and the oxalate nephropathy warning. https://api.fda.gov/drug/label.json?search=openfda.brand_name:Ascor
