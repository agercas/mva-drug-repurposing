# Probability of an error-free division

The probability of an error-free mitosis (a cell division that segregates all 46 chromosomes correctly) is about 0.93 for a cell carrying the child's estimated amount of working BubR1. BubR1 is the spindle-checkpoint protein encoded by *BUB1B*. The model's 5th to 95th percentile is 0.74 to 0.98, and the median varies from 0.85 to 0.94 under alternative inputs.

The figure is a model estimate, and the error rate in the child's cells is unmeasured.

## Calculation

The probability of an error-free mitosis is (1 − μ)^46, where μ is the probability that one chromosome missegregates in one division. Two steps set μ.

1. **Working BubR1 level.** The two alleles are the stop-gain p.Leu737Ter (a change that creates a premature stop codon) and the missense p.Asn1002Lys (a change of one amino acid). The level combines the two alleles from four factors per allele, each relative to one wild-type allele: transcript remaining after nonsense-mediated decay (NMD, the degradation of transcripts that carry a premature stop codon), translation, folded fraction and specific activity (activity per protein molecule).

   The limiting level is the lower of the checkpoint function and the attachment-stabilisation function. The median is 0.23 of a normal cell (90% interval 0.06 to 0.49).

2. **Dose curve.** Per-chromosome missegregation probability is a four-parameter sigmoid of BubR1 level, fitted to ten published readouts in three groups.

   - **Patient lymphocytes (three readouts).**
     - Two readouts come from patients in seven families with monoallelic *BUB1B* variants (one gene copy affected; PMID [16411201](https://pubmed.ncbi.nlm.nih.gov/16411201/); abstract read; BubR1 expression reduced by more than half).
     - The third readout pairs an aneuploid share, the median of 13 patients (this report's calculation from Table I of PMID [18548531](https://pubmed.ncbi.nlm.nih.gov/18548531/), a compilation of case reports), with a protein level from a different cohort.
     - The level comes from PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/) (full text read: a 2- to 6-fold decrease in four patient lines, taken as the geometric mean level of 0.29 of normal, √(1/2 × 1/6)). The two sources describe different patients.

   - **Mouse embryonic fibroblasts (five readouts).** Five genotypes with graded BubR1 levels (PMID [15208629](https://pubmed.ncbi.nlm.nih.gov/15208629/); full text read in an earlier project appraisal, see [section 2.4.2](../02-reported-research.md#242-baker-2004-bubr1-hypomorph-mouse)). The level and aneuploid-share values come from the extraction of the paper's tables and figure made in that earlier appraisal.

   - **HeLa cells, a human cervical cancer line (two readouts).** Doxycycline titration of BubR1 (PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/)). The paper states "virtually no impact" at about 13% of normal and missegregation "in the majority of cells" at about 6%. The numeric shares used in the fit (0.20 and 0.60) are the model's translation of those words.
     - A lagging-kinetochore floor of 0.17 comes from a different HeLa study (PMID [20016069](https://pubmed.ncbi.nlm.nih.gov/20016069/); 17% of anaphases with wild-type BubR1, read by eye from a figure; the abstract gives no value).

   The fitted half-point (the BubR1 level at which the curve lies midway between its floor and its ceiling) is 8.6% of normal level (90% interval 3.6% to 13.3%).

Combining both steps over 1.5 million joint draws gives a probability of an error-free mitosis with median 0.934 and mean 0.907. At the posterior-median parameters, μ = 1.27 × 10⁻³ per chromosome at level 0.23.

## Inputs by evidence quality

The table gives the status of each input to the model.

| Input | Status |
|---|---|
| Transcript fraction of the stop allele (median 0.54) | Measured for the class of 1,184 internal-exon stop-gains in the Genotype-Tissue Expression project (GTEx); the allele itself is unmeasured |
| Folded fraction and activity of the stop product | Mixture of two analogue alleles; the mixture weight (35% stable, 65% unstable) is assumed |
| Folded fraction of the missense product (median 0.58) | Inferred from one figure legend that pools four patient lines with other missense alleles |
| Specific activity of the missense product | Assumed; unmeasured for every variant at this position |
| Dose curve | Fitted to mouse, HeLa and patient-lymphocyte data of mixed quality; transfer to human cells is assumed; the HeLa values are the model's reading of text |
| Cell counts for five of ten readouts (three patient readouts, two HeLa readouts) | Assumed (100 cells each) |

## Sensitivity

The table gives the median and 90% interval of the probability of an error-free mitosis when one input is changed.

| Input varied | Median (90% interval) |
|---|---|
| Base case (no input varied) | 0.934 (0.744 to 0.977) |
| Missense folded fraction from kinase-region patient lines only | 0.914 (0.703 to 0.974) |
| Stop product unstable | 0.920 (0.714 to 0.975) |
| Both missense defects (stability and activity) | 0.904 (0.705 to 0.973) |
| Per-allele reading of the patient-line figure | 0.855 (0.623 to 0.971) |
| Prior only, no readouts | 0.84 (0.23 to 0.99) |
| Plug-in at the posterior-median curve parameters, (1 − 1.27 × 10⁻³)⁴⁶ (a different summary, so no interval) | 0.943 |

The plug-in value sets the upper end and the per-allele reading the lower end of the range of medians (0.94 to 0.85). The 5th percentile ranges from 0.62 to 0.74 across the sensitivity analyses of the derivation, excluding the prior-only row. The interval holds the priors, assumed counts and the mouse-to-human transfer fixed, so the real uncertainty is larger.

## Checks

- **Calibration on simulated data:** 60 simulated truths; coverage 0.93 against a pre-specified band of 0.78 to 0.98.

- **Reproduction:** a re-run with a new curve seed gave 0.932.

- **Posterior predictive check:** two of ten readouts fall outside the predicted interval (the first patient readout is over-predicted, and the HeLa readout at level 0.06 is under-predicted).

- **Baseline error:** the model's baseline of 6.2 × 10⁻⁴ per chromosome is 2.5 times the value measured in untreated RPE-1 (retinal pigment epithelial) and HCT116 (colon cancer) cells, about 2.5 × 10⁻⁴ per chromosome (PMID [18283116](https://pubmed.ncbi.nlm.nih.gov/18283116/); full text read, results text).

  - The authors state that their interphase FISH (fluorescence in situ hybridisation) method underestimates the true rate because single chromosomes in micronuclei are missed, and it scores a subset of chromosomes.

  - Conditioning the posterior on a baseline at or below 3.5 × 10⁻⁴ gives an estimate of 0.931.

- **Readout dependence:** the half-point is about 7% to 9% of normal for aneuploid-cell percentage and about 40% for premature chromatid separation, so the curve depends on which readout defines an error.

- **Hold-out control for the patient readouts failed** (Spearman rank correlation 0.61, exact two-sided p = 0.17, n = 7), so those readouts add little beyond a scaling factor.

## Use of the estimate

Over n divisions of one lineage the chance of no error is the single-division probability raised to the power n: 0.71 after 5 divisions, 0.51 after 10 and 0.26 after 20 at the median (0.934⁵ = 0.711, 0.934¹⁰ = 0.505, 0.934²⁰ = 0.255).

The estimate covers one division of a single dividing cell at the estimated BubR1 level, where a typical division is likely to be error-free. A direct measurement of missegregation in the child's own dividing cells would replace most of the model.

## References

- Baker DJ et al. (2004). BubR1 insufficiency causes early onset of aging-associated phenotypes and infertility in mice. *Nat Genet*. PMID [15208629](https://pubmed.ncbi.nlm.nih.gov/15208629/)
- Matsuura S et al. (2006). Monoallelic BUB1B mutations and defective mitotic-spindle checkpoint in seven families with premature chromatid separation (PCS) syndrome. *Am J Med Genet A*. PMID [16411201](https://pubmed.ncbi.nlm.nih.gov/16411201/)
- Thompson SL et al. (2008). Examining the link between chromosomal instability and aneuploidy in human cells. *J Cell Biol*. PMID [18283116](https://pubmed.ncbi.nlm.nih.gov/18283116/)
- García-Castillo H et al. (2008). Clinical and genetic heterogeneity in patients with mosaic variegated aneuploidy: delineation of clinical subtypes. *Am J Med Genet A*. PMID [18548531](https://pubmed.ncbi.nlm.nih.gov/18548531/)
- Elowe S et al. (2010). Uncoupling of the spindle-checkpoint and chromosome-congression functions of BubR1. *J Cell Sci*. PMID [20016069](https://pubmed.ncbi.nlm.nih.gov/20016069/)
- Suijkerbuijk SJ et al. (2010). Molecular causes for BUBR1 dysfunction in the human cancer predisposition syndrome mosaic variegated aneuploidy. *Cancer Res*. PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/)
- GTEx Consortium et al. (2017). Genetic effects on gene expression across human tissues. *Nature*. PMID [29022597](https://pubmed.ncbi.nlm.nih.gov/29022597/)

## Other sources

- GTEx v8 (https://gtexportal.org): transcript fraction for 1,184 internal-exon stop-gain variants; GTEx Consortium (2017), PMID [29022597](https://pubmed.ncbi.nlm.nih.gov/29022597/) [UNVERIFIED: the per-variant selection and the median of 0.54 come from a project analysis not published with this report].
- Dose-response readouts (ten published measurements), anchor cell lines (mouse fibroblasts, HeLa) and the posterior sample of 1.5 million joint draws: project model [UNVERIFIED: code and sample not published with this report].
