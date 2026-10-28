# Removal or replacement of aneuploid cells

A strategy that finds cells with the wrong chromosome number (aneuploid cells) and destroys them is unlikely to work for random aneuploidy at the detection accuracy now achievable. At a 1% aneuploid fraction, an agent that destroys every detected cell needs a false-positive rate near 1.4 × 10⁻⁵ per chromosome-arm test; the allowed rate rises steeply with the aneuploid fraction, and the one published control rate found is above the budget at every fraction up to about 42%, which covers the 13.6% in the patient cited here and the more than 25% that the [disease overview](../01-disease-and-case.md), citing a mouse-model paper, describes as typical for MVA. Every detector built or modelled here falls short on sensitivity and specificity at once. Replacement of cells works without per-cell discrimination and remains open.

## Trisomy-field tools

Every dosage correction built for trisomy 21 (a third copy of chromosome 21) assumes one known extra chromosome. In mosaic variegated aneuploidy (MVA) each cell has its own karyotype (set of chromosomes), regenerated at each division. The table lists six approaches from trisomy 21 research, the evidence for each and how far each transfers to random mosaic aneuploidy.

| Approach | Evidence | Transfer to random mosaic aneuploidy |
|---|---|---|
| *XIST* (the X-inactivation gene) transgene silencing a chromosome | PMID [23863942](https://pubmed.ncbi.nlm.nih.gov/23863942/), full text read; trisomy-21 pluripotent stem cells, transgene inserted into *DYRK1A* on one chromosome 21 | Needs the chromosome's identity and a targeted insertion into that copy in every cell; genes on the edited copy were silenced in about 100% of XIST-expressing cells after 20 days of doxycycline, and clones with XIST on two or three copies lost XIST expression |
| Nuclease-driven chromosome elimination | PMID [29178945](https://pubmed.ncbi.nlm.nih.gov/29178945/), full text available, abstract read; mouse and human cells, including trisomy-21 induced pluripotent stem cells | Multi-site guides match every copy, so a mosaic tissue's normal cells would be cut and made monosomic (left with one copy; this report's inference) |
| Interferon-receptor copy-number correction | PMID [37277650](https://pubmed.ncbi.nlm.nih.gov/37277650/), abstract read; copy number of the interferon-receptor locus corrected by genome editing in a Down syndrome mouse model; blood transcriptomes from people with Down syndrome | Acts on the interferon pathway only |
| Janus kinase (JAK) inhibition (tofacitinib) | PMID [39737640](https://pubmed.ncbi.nlm.nih.gov/39737640/), full text read; single-site open-label phase 2 interim analysis, first 10 participants to finish 16 weeks, people with Down syndrome and an immune skin condition (skin pathology fell in alopecia areata, psoriasis and atopic dermatitis); no serious adverse events | Chromosome-agnostic; the population differs from MVA |
| Senolytic clearance of senescent cells (fisetin) | PMID [37491366](https://pubmed.ncbi.nlm.nih.gov/37491366/), abstract and methods read; Ts65Dn mouse model of trisomy 21, fisetin in the diet (500 ppm) from 3 to 6 months of age reduced cortical oligodendrocyte-precursor senescence, restored precursor proliferation and improved contextual fear memory | Chromosome-agnostic; one laboratory; a dietary flavonoid with multiple effects |
| Aneuploidy-selective cytotoxics | PMID [21315436](https://pubmed.ncbi.nlm.nih.gov/21315436/), abstract only; AICAR (5-aminoimidazole-4-carboxamide ribonucleoside) killed mouse fibroblasts with a third copy of chromosome 1, 13, 16 or 19 by p53-mediated apoptosis, and 17-AAG (17-allylamino-17-demethoxygeldanamycin) and chloroquine also showed aneuploidy-selective effects | AICAR selectivity depends on p53; where a p53-dependent arrest protects cells in this disease (this report's inference), the selectivity would not act as intended |

## Detection arithmetic

1. **Signal.** In this report's unpublished analysis of public Cancer Dependency Map (DepMap) 24Q4 data (cancer cell lines with matched copy number), a whole-arm gain transfers 0.526 of the expected dosage change to mRNA (0.49 after lineage and offset adjustment). Of the genes on the gained arm, 45% respond at under half of full dosage and 9.3% move in the wrong direction.

   An independent published analysis reports that arm gain raises mean transcript by 22% and protein by 12% in 367 cancer cell lines, and by 22% and 8% in 168 ovarian tumours (PMID [35701073](https://pubmed.ncbi.nlm.nih.gov/35701073/); full text read).

2. **Budget.** For 9 in 10 destroyed cells to be aneuploid at a 1% aneuploid fraction and 50% sensitivity, the false-positive rate must stay below 5.6 × 10⁻⁴ per cell, which solves 0.5 × 0.01 / (0.5 × 0.01 + rate × 0.99) = 0.9 for the rate. 

   A detector blind to the changed chromosome tests 22 autosomes (non-sex chromosomes) or 39 chromosome arms (17 two-armed autosomes and 5 acrocentric ones with one testable arm), so the budget becomes 2.5 × 10⁻⁵ per autosome test or 1.4 × 10⁻⁵ per arm test (5.6 × 10⁻⁴ divided by 22 or by 39). Treating the tests as independent gives an upper bound on the penalty.

3. **Reference point.** A published analysis of blood single-cell RNA data labelled 4.0% of control cells "clean aneuploid" under stringent thresholds, against 13.6% in a patient with biallelic *MAD1L1* variants (a damaging change on both gene copies; PMID [36322655](https://pubmed.ncbi.nlm.nih.gov/36322655/); full text read, Methods). 

   The calls come from inferCNV, a program that infers copy-number changes from RNA expression. At f = 1% the 4.0% is 71 times the per-cell budget (0.040 / 5.6 × 10⁻⁴). Spread over 39 arm tests it is about 1.0 × 10⁻³ per test, also about 70 times the per-test budget at that fraction. As a false-positive rate it is an upper bound, because some control cells may be truly aneuploid.

4. **Chromosome-agnostic stress signatures** (this report's analysis of public data, with decoy signatures as controls) performed near chance across the same panel (area under the curve of 0.5 is chance): 0.522 for integrated stress, 0.531 for heat shock, 0.522 for type-I interferon and 0.539 for a mitotic-instability proxy, each inside its decoy distribution. The p53 signature scores below chance (0.377).

5. **Tissue model** (this report's simulation under an assumed noise model). At six buildable operating points, the ratio of the removal rate of healthy cells to that of aneuploid cells is 0.17, 0.18, 1.06, 1.08, 1.10 and 1.43. Four remove healthy cells at least as fast as aneuploid cells. The two below 1 reach true-positive rates of 0.060 and 0.056 against 0.5 required. An imperfect detector enriches tissue for the cells it was built to remove.

The 1.4 × 10⁻⁵ per-arm bound is the value at a 1% aneuploid fraction, 50% sensitivity and 90% precision. The allowed rate scales with f / (1 − f), where f is the aneuploid fraction: it is 0.5 × f × (1/0.9 − 1) / (1 − f) per cell, which is 6.2 × 10⁻³ per cell (1.6 × 10⁻⁴ per arm test) at f = 10% and 8.7 × 10⁻³ per cell (2.2 × 10⁻⁴ per arm test) at f = 13.6%, the called fraction in the *MAD1L1* patient of item 3 (called by inferCNV; if the 4.0% called in controls were all false positives and every truly aneuploid cell were called, the true fraction would be about 10%). At f = 13.6% the 4.0% control rate is about 4.6 times the per-cell budget, not 71 times. At f = 25% the budget is 1.9 × 10⁻² per cell (4.8 × 10⁻⁴ per arm test) and the 4.0% rate is about 2.2 times it; the two are equal at f of about 42%. The bound can be applied before a detector is built, with the aneuploid fraction of the disease in question.

## Antibodies

The spindle assembly checkpoint, the dosage imbalance and every effector sit inside the cell. The best extracellular candidate is a roughly twofold rise in the surface ligands MICA and MICB (MHC class I chain-related proteins A and B, where MHC is the major histocompatibility complex) of the natural killer cell receptor NKG2D on arrested cells with complex karyotypes. The finding comes from one author group (PMID [28633018](https://pubmed.ncbi.nlm.nih.gov/28633018/); full text read, results on Fig. 7D and 7G), in cells that are also arrested and senescence-like.

In the same figure, euploid cells (normal chromosome number) given doxorubicin are the positive control for two other ligands (CD155 and ULBP2). The surface markers considered here failed an evidence bar this report set before the analysis [UNVERIFIED: the bar and its results are not published with this report].

## Replacement

Supplying competent cells works without per-cell discrimination under two conditions:

- The enabling conditioning step acts on cells that already missegregate (distribute chromosomes unequally at division), and the radiosensitivity of the disease is open.
- A donor-derived cell population outcompetes the recipient's mosaic lineages.

## Limits

- Cell-level figures are calculated under an assumed noise model.
- Two of five pre-registered controls failed.
- The tissue model is exploratory.

## Verification

An independent AI verifier (a separate Claude session) rederived the detection numbers from the public source files and reread the primary papers behind every transfer claim. AI agents also reviewed thirty hypotheses from the project's own idea set in a blind review [UNVERIFIED: the count comes from the project's review log and was not recomputed].

## References

- Tang YC et al. (2011). Identification of aneuploidy-selective antiproliferation compounds. *Cell*. PMID [21315436](https://pubmed.ncbi.nlm.nih.gov/21315436/)
- Jiang J et al. (2013). Translating dosage compensation to trisomy 21. *Nature*. PMID [23863942](https://pubmed.ncbi.nlm.nih.gov/23863942/)
- Santaguida S et al. (2017). Chromosome Mis-segregation Generates Cell-Cycle-Arrested Cells with Complex Karyotypes that Are Eliminated by the Immune System. *Dev Cell*. PMID [28633018](https://pubmed.ncbi.nlm.nih.gov/28633018/)
- Zuo E et al. (2017). CRISPR/Cas9-mediated targeted chromosome elimination. *Genome Biol*. PMID [29178945](https://pubmed.ncbi.nlm.nih.gov/29178945/)
- Schukken KM et al. (2022). Extensive protein dosage compensation in aneuploid human cancers. *Genome Res*. PMID [35701073](https://pubmed.ncbi.nlm.nih.gov/35701073/)
- Villarroya-Beltri C et al. (2022). Biallelic germline mutations in MAD1L1 induce a syndrome of aneuploidy with high tumor susceptibility. *Sci Adv*. PMID [36322655](https://pubmed.ncbi.nlm.nih.gov/36322655/)
- Waugh KA et al. (2023). Triplication of the interferon receptor locus contributes to hallmarks of Down syndrome in a mouse model. *Nat Genet*. PMID [37277650](https://pubmed.ncbi.nlm.nih.gov/37277650/)
- Rusu B et al. (2023). Single-Nucleus Profiling Identifies Accelerated Oligodendrocyte Precursor Cell Senescence in a Mouse Model of Down Syndrome. *eNeuro*. PMID [37491366](https://pubmed.ncbi.nlm.nih.gov/37491366/)
- Rachubinski AL et al. (2024). JAK inhibition decreases the autoimmune burden in Down syndrome. *Elife*. PMID [39737640](https://pubmed.ncbi.nlm.nih.gov/39737640/)

## Other sources

- Single-cell copy-number calls labelling 4.0% of control cells aneuploid (reference point, item 3 of Detection arithmetic): inferCNV (https://github.com/broadinstitute/infercnv), run with the settings of PMID [36322655](https://pubmed.ncbi.nlm.nih.gov/36322655/) Methods [UNVERIFIED: inferCNV version not recorded].
- Detection arithmetic (per-cell and per-arm error budgets, 5.6e-4 per cell and 1.4e-5 per arm test): this report's calculation, given in full in item 2 of Detection arithmetic and rechecked by hand on 2026-10-24.

- Arm-gain transfer to mRNA (0.526; 0.49 adjusted), the stress-signature areas under the curve and the tissue-model ratios: this report's analysis of DepMap 24Q4 (https://depmap.org) and public single-cell data [UNVERIFIED: the analyses are not published with this report].
- Antibody and tissue-model screens: public tissue-expression atlases [UNVERIFIED: the atlases, releases and access dates are not recorded in the sources read].
