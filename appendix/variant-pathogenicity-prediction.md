# Pathogenicity prediction for the missense variant

AlphaMissense (a deep-learning predictor of missense pathogenicity) scores *BUB1B* p.Asn1002Lys (N1002K, a change of one amino acid) at 0.92 (likely pathogenic). The protein level and activity of the allele need a measurement, because the predictor misses 3 of 5 measured destabilised hypomorphs (alleles with reduced function).

## Scores

The table lists the scores of three predictors for N1002K: AlphaMissense, REVEL (Rare Exome Variant Ensemble Learner) and CADD (Combined Annotation Dependent Depletion, phred scale).

| Predictor | N1002K | Reading |
|---|---|---|
| AlphaMissense | 0.92 | Likely pathogenic; 96th percentile among 2,003 reported missense variants in the gene |
| REVEL | 0.47 | Below the usual 0.5 threshold; 90th percentile |
| CADD (phred) | 24.3 to 24.5 | 73rd percentile |

The variant lies in the last exon (c.3006T>G), in the C-terminal lobe of the kinase domain, 10 residues from p.Leu1012Pro and 2 residues from p.Asn1004Ser (ClinVar benign/likely benign). ClinVar (the archive of variant interpretations at the National Center for Biotechnology Information, NCBI; checked 2026-10-24) holds no c.3006T>G record, and gnomAD v4 (Genome Aggregation Database, exome data) lists it once. Its function is unmeasured.

## Calibration against measured alleles

One study (PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/); full text read, methods and figure legends; supplement not available) measured protein abundance for substitutions in or near the kinase region. Its findings:

- Five disease-associated kinase-region substitutions were measured, and all five were 5 to 10 times lower than wild type when expressed as tagged proteins in HeLa and U2OS cells (human cervical cancer and osteosarcoma lines).

- In four patient-derived lines (absent/I909T, 386X/R727C, 753X/R814H and 731X/Y155C, whose Y155C allele is N-terminal and outside the five substitutions above), the text says the full-length missense protein was 2 to 6 times lower "compared to wild-type alleles". The legend of the figure reports band intensity relative to healthy control cells, so the figure may give the whole-cell level, with a per-allele ratio as the alternative reading.

- Overexpression to wild-type level restored function for the two alleles tested this way (I909T and L1012P).

- The authors infer misfolding from a short drug-treatment experiment (inhibition of the chaperone HSP90, heat shock protein 90, and of the proteasome, 5 hours, one representative experiment). Pulse-chase and ubiquitination assays are absent from the study.

- The substitution p.Gln921His lies on the same allele as p.Leu844Phe in the patient report, and matches wild type in abundance and function.

- The two substitutions away from the kinase region (p.Tyr155Cys, p.Arg550Gln) were stable.

The table gives the eight alleles with their measured abundance or function and the scores of the three predictors.

| Measured allele | Abundance or function | AlphaMissense | REVEL | CADD |
|---|---|---|---|---|
| p.Leu1012Pro | Low | 0.87 (likely pathogenic) | 0.50 | 26.7 |
| p.Ile909Thr | Low | 0.45 (ambiguous) | not scored | not scored |
| p.Leu844Phe | Low | 0.29 (likely benign) | 0.39 | 22.1 |
| p.Arg814His | Low | 0.22 (likely benign) | 0.39 | 29.7 |
| p.Arg727Cys | Low | 0.24 (likely benign) | 0.27 | 33.0 |
| p.Gln921His | Stable and functional | 0.49 (ambiguous) | 0.24 | 20.6 |
| p.Arg550Gln | Stable, functional | 0.07 | 0.02 | 0.01 |
| p.Tyr155Cys | Stable; restores chromosome alignment; checkpoint function stays lost | 0.54 (ambiguous) | 0.93 | 29.3 |

AlphaMissense calls 1 of the 5 low-abundance alleles likely pathogenic, 1 ambiguous and 3 likely benign. REVEL reaches 0.5 for 1 of 4 scored. CADD reaches 20 for 4 of 4.

The five alleles were selected because they cause disease. The count therefore applies to disease-associated kinase-region substitutions, and estimating how often a predictor misses a destabilised allele in general takes an unselected set of alleles.

Four of the five destabilised alleles score below 0.5 on AlphaMissense, and three of the four scored alleles score 0.39 or lower on REVEL. Both predictors score the stable, functional p.Arg550Gln low, and p.Tyr155Cys, which keeps chromosome alignment and loses the checkpoint, moderate to high. Neither predictor separates stability from activity.

## Interpretation

1. N1002K scores above all five measured low-abundance alleles on AlphaMissense. This agrees with a damaging classification and with the position-based expectation that the allele belongs with its nearest measured neighbours, whose abundance is low.

2. The scores of N1002K lie within the range of the measured hypomorphs on REVEL (0.47 against 0.27 to 0.50 for the four scored) and on CADD (24.3 to 24.5 against 22.1 to 33.0), so the two scores leave the severity of N1002K unranked.

3. With a null partner (a second allele that makes no functional protein), the residual function of a compound heterozygote (a different change on each gene copy) equals the missense protein's abundance times its specific activity (activity per protein molecule), divided by two (the wild-type diploid cell is 1).

   - Taking the paper's fold ranges literally per allele, and assuming normal specific activity and a fully null partner, gives about 5% to 25% of diploid wild type.

   - If the 2 to 6 fold values are whole-cell levels relative to healthy controls, as the figure legend suggests, the residual is higher.

   - The range comes from abundance alone and from a mix of tagged-protein and patient-line measurements, none of them for N1002K.

   - It overlaps the HeLa window in which about 13% of normal BubR1 had virtually no effect on segregation and about 6% caused errors in most cells (PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/), Fig. 4D, one cell line).

   - The position of N1002K relative to that window is unmeasured.

Only a measurement of N1002K protein abundance, half-life and checkpoint activity in a matched system settles the question.

## References

- Suijkerbuijk SJ et al. (2010). Molecular causes for BUBR1 dysfunction in the human cancer predisposition syndrome mosaic variegated aneuploidy. *Cancer Res*. PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/)
- Ioannidis NM et al. (2016). REVEL: An Ensemble Method for Predicting the Pathogenicity of Rare Missense Variants. *Am J Hum Genet*. PMID [27666373](https://pubmed.ncbi.nlm.nih.gov/27666373/)
- Rentzsch P et al. (2019). CADD: predicting the deleteriousness of variants throughout the human genome. *Nucleic Acids Res*. PMID [30371827](https://pubmed.ncbi.nlm.nih.gov/30371827/)
- Cheng J et al. (2023). Accurate proteome-wide missense variant effect prediction with AlphaMissense. *Science*. PMID [37733863](https://pubmed.ncbi.nlm.nih.gov/37733863/)
- Chen S et al. (2024). A genomic mutational constraint map using variation in 76,156 human genomes. *Nature*. PMID [38057664](https://pubmed.ncbi.nlm.nih.gov/38057664/)

## Other sources

- AlphaMissense: Cheng J et al. (2023), PMID [37733863](https://pubmed.ncbi.nlm.nih.gov/37733863/); scores for p.Asn1002Lys (0.9229, 5th highest of the 19 substitutions at residue 1002) and the eight measured alleles re-read on 2026-10-24 from the AlphaFold DB file AF-O60566-F1-aa-substitutions.csv (model version 6), and found to match the table to two decimals.

- REVEL: Ioannidis NM et al. (2016), PMID [27666373](https://pubmed.ncbi.nlm.nih.gov/27666373/). CADD: Rentzsch P et al. (2019), PMID [30371827](https://pubmed.ncbi.nlm.nih.gov/30371827/); the table reports 24.3 to 24.5 [UNVERIFIED: CADD release numbers and the reason for two values are not recorded].

- ClinVar, read through the NCBI E-utilities on 2026-10-24: no record for c.3006T>G; the neighbouring record VCV004600147.1 is c.3006T>A (uncertain significance): https://www.ncbi.nlm.nih.gov/clinvar/variation/4600147/. p.Asn1004Ser (c.3011A>G) is VCV000133772, benign/likely benign, criteria provided, multiple submitters, no conflicts, last evaluated 2026-03-01: https://www.ncbi.nlm.nih.gov/clinvar/variation/133772/

- gnomAD v4 (GraphQL API, dataset `gnomad_r4`, queried 2026-10-24): Chen S et al. (2024), PMID [38057664](https://pubmed.ncbi.nlm.nih.gov/38057664/); 15-40220612-T-G seen once in 1,461,878 exome alleles.

- The 2,003 reported missense rows and the five measured low-abundance kinase-region alleles: Suijkerbuijk SJ et al. (2010), PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/), with the BUB1B variant table of this project [UNVERIFIED: table not published with this report].
