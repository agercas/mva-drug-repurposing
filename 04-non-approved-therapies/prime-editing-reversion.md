# Ex vivo prime-editing reversion of the stop allele

Prime editing writes a chosen sequence at a single-strand DNA nick, directed by a prime editing guide RNA (pegRNA) and a Cas9 nickase (a CRISPR enzyme that cuts one DNA strand). It can revert the L737X stop codon (TGA) to leucine (TTA). The patient's own (autologous) CD34+ blood stem and progenitor cells (identified by the surface protein CD34) would be edited ex vivo (outside the body). Reversion would turn the compound heterozygote (a different damaging change on each *BUB1B* copy) into the genotype of a healthy heterozygous carrier.

At the published median edit of 0.23 and a retention of 0.75 to 1.10 after engraftment, 0.17 to 0.25 of cells would carry the reversion (0.23 × 0.75 and 0.23 × 1.10). Halving the excess division error needs 0.51 to 0.56 of cells and carrier level needs 0.89 to 1.0 ([correction a therapy must reach](README.md#correction-a-therapy-must-reach)).

## Candidate

| Field | Content |
|---|---|
| Candidate | Prime editor with a pegRNA specific to the stop allele, applied ex vivo to autologous CD34+ haematopoietic stem and progenitor cells |
| Status | Investigational. A prime-edited autologous CD34+ product (PM359) has first-in-human data in p47-phox chronic granulomatous disease (an inherited immune disorder in which neutrophils cannot kill microbes): 2 adult participants (aged 18 and 57), 4 to 6 months of follow-up, sponsor-funded, study later terminated by the sponsor (PubMed identifier, PMID [41358590](https://pubmed.ncbi.nlm.nih.gov/41358590/), full text read) |
| Route | Cell product reinfused after conditioning (chemotherapy that clears native marrow cells); no paediatric prime-editing exposure is reported |

## Hypothesis

Reversion of TGA to TTA at codon 737 in CD34+ cells restores one wild-type allele in the edited cell and lowers its mean division error to the carrier level for that cell.

*Speculation:* edited cells engraft and divide as normal cells, so the corrected pool lowers blood-lineage aneuploidy. The competitive advantage of a corrected cell over an uncorrected one is unmeasured.

Basis labels are defined in the [section 4 README](README.md#basis-labels): Demonstrated, Suggested, Our inference and Speculation.

| Step | Basis | System | Source |
|---|---|---|---|
| 1. Prime editing makes single-nucleotide changes in human CD34+ stem and progenitor cells | Demonstrated | Human CD34+ cells ex vivo, healthy and sickle-cell donors, at loci optimised by the authors (13 to 41 percent allele edit) | PMIDs [37069266](https://pubmed.ncbi.nlm.nih.gov/37069266/), [37679541](https://pubmed.ncbi.nlm.nih.gov/37679541/), [39640014](https://pubmed.ncbi.nlm.nih.gov/39640014/) |
| 2. A pegRNA for the stop-to-leucine reversion at codon 737 reaches a useful edit level | Speculation | None: no stop-gain reversion by prime editing in blood cells was found; a predictor scores the best NGG pegRNA 6.4 in K562 cells against 64.3 in HEK293T | PMID [38907037](https://pubmed.ncbi.nlm.nih.gov/38907037/) (predictor only) [UNVERIFIED predictor version] |
| 3. Edited cells engraft and keep their edit | Suggested | Human cells in immunodeficient mice at three loci (retention 0.74 to 1.05, ratios calculated by this report); two adults with an edited autologous product, 4 to 6 months of follow-up | PMIDs [37069266](https://pubmed.ncbi.nlm.nih.gov/37069266/), [39640014](https://pubmed.ncbi.nlm.nih.gov/39640014/), [37679541](https://pubmed.ncbi.nlm.nih.gov/37679541/), [41358590](https://pubmed.ncbi.nlm.nih.gov/41358590/) |
| 4. A BubR1-low autologous product survives manufacture and conditioning | Our inference | Model projection of 21 to 36 percent loss of viable euploid cells over two divisions at missense activity 0.1 to 0.05; the one transplant in a patient with biallelic *BUB1B* variants was rejected on day 47 and ended in death on day 156 (allogeneic, a different intervention) | PMID [31053147](https://pubmed.ncbi.nlm.nih.gov/31053147/) |
| 5. One restored wild-type allele with the N1002K allele in trans gives carrier-level function | Our inference | Healthy heterozygous carriers of one loss-of-function allele are the reference; the activity of the N1002K protein is unmeasured | Section 1.7 |
| 6. A corrected cell outcompetes an uncorrected one by about 1 to 3 percent per division | Our inference | Calibration made for this report; the cited mouse hypomorph paper reports no per-division advantage (relative fitness 1.06, 10 H/H and 6 control mice, one research group) | PMID [27313317](https://pubmed.ncbi.nlm.nih.gov/27313317/) |
| 7. The corrected cell halves the mean division error | Our inference | Monte Carlo model of the BubR1 dose-response, depending on the activity of the N1002K protein relative to wild type (alpha; 0.1 in the table below) | Section 5 |
| 8. A lower blood-lineage error rate gives a benefit to the child | Speculation | None; haematopoietic correction addresses a median 0.037 of documented disease burden (0.17 for mortality-linked features) | None |

Basis: 1 step Demonstrated (human CD34+ cells, other loci), 1 Suggested, 4 Our inference, 2 Speculation.

## Delivery and exposure

- **Format** (*Demonstrated at other loci in human CD34+ cells*). Prime-editor mRNA with a synthetic pegRNA and a nicking guide (a second guide that nicks the unedited strand) is electroporated (delivered by electric pulse) into mobilised-blood CD34+ cells (stem cells moved from marrow to blood by a drug) and edited over a 3-day culture. Three published studies used prime editor versions (PE2, PE3, PEmax) at other loci:

  - HBB (the beta-globin gene): PEmax mRNA, an engineered pegRNA and one nicking guide, with the components electroporated twice (2xPE3max; PMID [37069266](https://pubmed.ncbi.nlm.nih.gov/37069266/)).

  - B2M (the beta-2 microglobulin gene): PE3 and day-3 culture (PMID [37679541](https://pubmed.ncbi.nlm.nih.gov/37679541/)).

  - HBA2 (the alpha-globin gene), haemoglobin Constant Spring: PE2 mRNA, a synthetic pegRNA and one nicking guide (PMID [39640014](https://pubmed.ncbi.nlm.nih.gov/39640014/)).

- **Efficiency in the product** (*Demonstrated at other loci; the median across ten values is a compilation made for this report, Our inference*). Allele-level edits of 13 to 41 percent at loci that the authors had optimised (median 23 percent, 5th to 95th percentile 10 to 52 across ten published values compiled for the model). Four sources are cited here and the other six are not listed in this report [UNVERIFIED]. A new locus without optimisation is expected to start lower.

  - Day-3 editing at HBB was 26 +/- 10 percent in cells from four sickle-cell donors, 15 to 41 percent per donor in the abstract (PMID [37069266](https://pubmed.ncbi.nlm.nih.gov/37069266/)).

  - In the PM359 product for p47-phox chronic granulomatous disease, bulk sequencing reads gave 13 and 23 percent, with at least one corrected allele in 68 and 91 percent of colonies (PMID [41358590](https://pubmed.ncbi.nlm.nih.gov/41358590/)).

  - The colony figure overstates the allele fraction by up to twofold in a two-allele cell, and this stop is one target allele per cell.

- **Retention after engraftment** (*Suggested: mouse xenotransplants; the ratios are calculated by this report from figure values, Our inference*). Retention is the engrafted edit divided by the input edit. All three loci were tested as xenotransplants (human cells in immunodeficient mice):

  - HBB, 0.90 (range 0.80 to 1.10; PMID [37069266](https://pubmed.ncbi.nlm.nih.gov/37069266/)): busulfan-treated NBSGW mice (an immunodeficient strain) at 17 weeks, with cells from four sickle-cell donors. The authors report edits maintained and one donor higher than input.

  - HBA2, 0.74 (PMID [39640014](https://pubmed.ncbi.nlm.nih.gov/39640014/)): two healthy-donor products edited to create the Hb Constant Spring variant (a stop-loss variant of HBA2), read at 16 weeks. Patient-cell correction (21 percent) was not transplanted.

  - B2M, 1.05 (PMID [37679541](https://pubmed.ncbi.nlm.nih.gov/37679541/)): healthy-donor mobilised-blood cells with primary and secondary recipients.

  - Our leave-one-locus-out check (predicting each locus from the other two) was within a factor of 1.31 for every locus, so a planning range of 0.75 to 1.10 applies.

- **Conditioning** (*Demonstrated in two adults for busulfan; for BUB1B, one allogeneic case report*).

  - Engraftment of the p47-phox product followed single-agent, pharmacokinetically adjusted busulfan (dose set from measured drug levels), with neutrophil engraftment on day +14 and +16 and no serious adverse event after infusion (PMID [41358590](https://pubmed.ncbi.nlm.nih.gov/41358590/)).

  - The only transplant report in a patient with biallelic *BUB1B* variants found in a title and abstract search of Europe PMC (a literature database) on 2026-10-24 (PMID [31053147](https://pubmed.ncbi.nlm.nih.gov/31053147/), full text read) describes an 11-year-old with myelodysplasia (abnormal blood-cell production in the marrow) and monosomy 7 (loss of one copy of chromosome 7). The child received an unrelated-donor graft (9.4 x 10^6 CD34+ cells per kg) after treosulfan, fludarabine and thymoglobulin.

  - The graft engrafted and was rejected on day +47. Marrow aplasia (failure to make blood cells) followed, and the patient died of infection (sepsis) on day +156. The authors' interpretation is in the [section 4 README](README.md#conditioning-transplant-and-malignancy-precedents).

- **In vivo route** (*no evidence*). No in vivo (inside the body) haematopoietic stem cell prime-editing efficiency was found in the 2023 to 2026 literature searched. Targeted lipid nanoparticle base editing in humanised mice exists in reviews only.

- **Constraint specific to this product** (*viability loss: Our inference from a model; p53 and interferon response: Demonstrated in healthy-donor CD34+ cells*).

  - A BubR1-low (reduced BubR1) CD34+ culture loses a median 21 to 36 percent of its viable euploid cells (cells with the normal chromosome number) over two divisions at missense activity 0.1 to 0.05 (model projection, see Expected effect).

  - In healthy-donor mobilised-blood CD34+ cells, prime editing at B2M induced p53 target genes, interferon genes and a pro-apoptotic TP73 isoform at 24 hours, to a lower extent than Cas9 for the p53 and interferon genes (PMID [37679541](https://pubmed.ncbi.nlm.nih.gov/37679541/), full text read, n = 5 to 6 donors).

- **Weakest link.** Step 2: no reversion of a stop codon by prime editing in blood cells has been reported, and every efficiency figure comes from a different locus.

## Evidence for

- Prime editing in human haematopoietic stem and progenitor cells gave a median 23 percent allele-level edit across ten published values, at loci optimised by the authors. All targets are single-nucleotide or small edits; none reverts a premature stop codon.

- Editing reached up to 41 percent at the sickle-cell locus in patient cells (PMID [37069266](https://pubmed.ncbi.nlm.nih.gov/37069266/), full text read; the authors hold prime-editing patents and consult for Prime Medicine). The average precise outcome was 40 percent at B2M in six healthy donors (PMID [37679541](https://pubmed.ncbi.nlm.nih.gov/37679541/), full text read).

- Edited human cells engrafted immunodeficient mice with edit levels maintained at three loci (PMIDs [37069266](https://pubmed.ncbi.nlm.nih.gov/37069266/), [39640014](https://pubmed.ncbi.nlm.nih.gov/39640014/), [37679541](https://pubmed.ncbi.nlm.nih.gov/37679541/); full texts read). The retention ratios of 0.74 to 1.05 are our calculations from figure values. The leave-one-locus-out control passed (borderline at HBA2).

- A prime-edited autologous product (PM359) reached neutrophil engraftment on day +14 and +16 in two adults with p47-phox chronic granulomatous disease after busulfan conditioning. NADPH oxidase activity in neutrophils was maintained at 6 and 4 months, and no serious adverse event followed infusion (PMID [41358590](https://pubmed.ncbi.nlm.nih.gov/41358590/), full text read). The follow-up is short, the trial was sponsor-funded and the sponsor terminated it.

- Editing reached up to 70 percent at a seven-nucleotide deletion (c.956_962del) in *GATA2*, a blood-cell transcription factor gene, in patient-derived CD34+ cells, raising functional *GATA2* alleles from 50 to 77 percent, and short prestimulation mitigated p53 activation (PMID [42814803](https://pubmed.ncbi.nlm.nih.gov/42814803/), abstract only; carries no weight in conclusions).

- At HBB, adding a silent edit that destroys the protospacer-adjacent motif (PAM; the short sequence Cas9 needs next to its target, NGG for *Streptococcus pyogenes* Cas9, SpCas9) after editing raised editing efficiency (PMID [37069266](https://pubmed.ncbi.nlm.nih.gov/37069266/)). The allele-exclusive design below destroys a PAM on reversion; this related design is untested.

## Evidence against

- A 2022 to 2026 search found no stop-gain reversion by prime editing in haematopoietic cells. The nearest examples are point substitutions, a two-nucleotide repair and, at HBA2, a stop-loss variant (a stop codon changed to a sense codon). Its creation matches the direction of this reversion and reached 27 percent in healthy-donor haematopoietic cells, while its correction installs a stop codon, the opposite direction, in 21 percent of patient-cell alleles (PMID [39640014](https://pubmed.ncbi.nlm.nih.gov/39640014/); abstract and full text read; searches of Europe PMC, dated 2026-10-20).

- Efficiency is locus-specific: only one of a panel of B2M pegRNAs worked in K562 cells, a human leukaemia cell line (PMID [37679541](https://pubmed.ncbi.nlm.nih.gov/37679541/)).

- A pegRNA-efficiency predictor (PRIDICT2) scores the best stop-reversion NGG pegRNA 6.4 in K562 cells against 64.3 in HEK293T cells, a human embryonic kidney cell line (our run of the predictor, version not recorded [UNVERIFIED]). That pegRNA is not allele-exclusive. The predictor's scope covers NGG guides in cell lines; the allele-exclusive NG and NGA guides and haematopoietic cells fall outside it.

- Manufacturing a BubR1-low CD34+ product differs from manufacturing healthy-donor products. Prime editing triggers p53, interferon and TP73 responses in normal cells (PMID [37679541](https://pubmed.ncbi.nlm.nih.gov/37679541/)). The transplant recipient with biallelic *BUB1B* variants had a monosomy 7 clone and hypoplastic marrow (marrow with reduced cell production), and died after graft rejection (PMID [31053147](https://pubmed.ncbi.nlm.nih.gov/31053147/)). That was an allogeneic graft (from a donor), a different intervention from an autologous edited product.

- Engraftment limits every autologous route. The model probability that the achieved engrafted fraction meets the need is 0.05 with busulfan.

- Haematopoietic correction addresses a median 0.037 of documented disease burden (range 0.016 to 0.098; 0.17 for mortality-linked features; defined in [section 4](README.md#mechanism-basis-by-candidate)). Only 1 of 13 tumour-bearing patients in this report's case table had a haematopoietic first tumour. The estimate rests on that table, which is dominated by kidney tumours [UNVERIFIED: the table is not published with this report].

- The selective advantage of a corrected cell (about 1 to 3 percent per division) is a calibration made for this report [UNVERIFIED model input].

- The mouse paper behind this calibration (PMID [27313317](https://pubmed.ncbi.nlm.nih.gov/27313317/), full text read, one research group) found that *Bub1b* hypomorph (H/H) stem cells competed normally in primary reconstitution (relative fitness 1.06 against 0.08 for trisomy 16; 10 H/H and 6 control recipients).

  - Single-cell sequencing of one recipient at 16 weeks found 7 of 18 donor-derived blood cells (about 39 percent) aneuploid, while 0 of 19 sequenced H/H stem cells from fetal liver and 0 of 19 from bone marrow were. H/H stem cells exhausted on serial transplantation.

  - The paper's system is a hypomorphic mouse with random aneuploidy, a different comparison from a corrected against an uncorrected human cell.

- No independent research group has reported *BUB1B* stop reversion; the five editing papers cited come from four to five groups working at other loci, and two of the papers are linked to one company.

## Safety

- Gate 4 (cancer-risk direction) for the edit: unassessed. Prime editing introduces fewer double-strand breaks than Cas9 nuclease, yet about 140 colonies from edited healthy-donor cells still showed large deletions at the target in the B2M study, fewer than after Cas9 (PMID [37679541](https://pubmed.ncbi.nlm.nih.gov/37679541/)). Its p53 activation in BubR1-low cells is untested.

- Gate 1 (genotoxicity) is strained by conditioning: busulfan is an alkylating drug (it damages DNA). The sensitivity of patient-derived or non-transformed *BUB1B*-deficient cells to alkylators has no study in Europe PMC (searched 2026-10-24). The one related study, in a paediatric glioblastoma cell line (PMID [23728478](https://pubmed.ncbi.nlm.nih.gov/23728478/); abstract read), is summarised in the [section 4 README](README.md#precedent-products).

- Gate 3 (paediatric exposure): the reported exposure to prime-edited autologous products is the two PM359 participants, adults aged 18 and 57 (PMID [41358590](https://pubmed.ncbi.nlm.nih.gov/41358590/)). No paediatric exposure is reported.

- Check against the child's other genetic findings: pending for the secondary finding and the four unnamed carrier-state variants ([section 3 README](../03-approved-drugs/README.md#check-against-the-childs-other-genetic-findings)).

## Expected effect

*Every figure below is Our inference: a projection from a pre-registered Monte Carlo model that draws its inputs at random (the published edit levels above [Suggested, other loci], retention 0.75 to 1.10 [Suggested] and a division-error model of the BubR1 dose). The projection depends on the activity of the missense protein relative to wild type (alpha), which is unmeasured; the figures assume alpha = 0.1.*

| Scenario | Corrected cells at 50 percent or more of mature blood cells | Error halved in the mean | Carrier-level error | Basis |
|---|---|---|---|---|
| Edit as published (median 0.23), no selective advantage | 0.04 | 0.04 | 0.001 | Our inference from Suggested inputs |
| Same, with the selective advantage calibrated on the mouse hypomorph data | 0.35 | 0.33 | 0.001 | Our inference; advantage is a calibration made for this report |
| Same, with the unconstrained selective-advantage model | 0.73 | 0.71 | 0.13 | Speculation: advantage not constrained by data |
| Best-case GATA2 edit level (abstract only), no advantage | 0.51 | 0.46 | 0 | Our inference from an abstract-only input |

- The day-3 edit needed to halve the mean error with probability 0.8 is 0.63 to 0.66 without selection and 0.29 to 0.60 with the calibrated advantage. The published median is 0.23, so halving the error needs more editing than has been achieved at every alpha except under the unconstrained advantage model at alpha 0.05 (0.16).

- If the missense protein is weaker (alpha 0.05), a calibrated advantage raises the probability of halving the error to 0.66. At alpha 0.3 it falls to 0.05.

- Expected to stay unchanged: the unedited N1002K allele, tissues outside the blood lineage and tumour risk in non-haematopoietic tissue.

- **Weakest link.** Step 6, the selective advantage of a corrected cell: this report calibrated it, and the probability of halving the mean error moves from 0.04 to 0.33 in the table on that one assumption.

## Test

| Stage | Measurement | Pass criterion | Stopping criterion |
|---|---|---|---|
| 0 | Stop reversion in a K562 knock-in, best of three pegRNAs | at least 25 percent precise, indels at most 5 percent | below 10 percent for all |
| 1 | Forward edit at the same locus in healthy CD34+ cells, day 3 | at least 20 percent | below 8 percent |
| 2 | Viability and colony output of BubR1-low CD34+ cells after editing versus mock | at least 0.7 | below 0.4 |
| 3 | Engrafted edit in immunodeficient mice at 16 to 17 weeks versus input | at least 0.7 | below 0.5 |
| 4 | Day-3 allele fraction in the product | at least 0.41 (calibrated selection) or 0.63 (no selection) | below 0.29 |

A 14-day competitive growth assay of *BUB1B*-depleted versus rescued CD34+ cells runs before stage 0. It measures the selective advantage and moves the stage 4 threshold from 0.63 to between 0.16 and 0.41. All thresholds are written before any experiment.

## Outcome if confirmed

A reversion product that passes stages 0 to 4 would reach the halved-error target and fall short of the carrier-level target. The activity of the N1002K protein ([section 1.7](../01-disease-and-case.md#17-unmeasured-quantities-that-bear-on-every-candidate)) and the share of disease burden in blood (Evidence against) determine whether the halved error gives the child a benefit.

## Allele-exclusive guides

At each variant site the substituted base creates a PAM on the variant allele only, so a pegRNA can nick the variant chromosome and leave the reference copy intact. The reversion restores the original base and destroys the PAM, which protects the edited allele from a second nick.

- **Stop site (L737X).** The site needs an NG or NGA PAM (spacer `TACTGAAGTCCCTACCAGAG`, nick 5 nucleotides from the edit).

- **Missense site (N1002K).** The site has an SpCas9 NGG guide (`ATTCTTTGTGCGGATTCTGA`, PAM AGG). The pegRNA design begins its template with a cytosine, which design guidance disfavours. A second missense design with an NGC PAM finds that PAM on the reference allele too, so the design lacks allele selectivity.

- **Scope of exclusivity.** Exclusivity holds for the NG, NGA and NGG PAM classes and fails for SpRY (a Cas9 variant that accepts nearly any PAM).

- **Remaining risk and test.** Allele-exclusive nicking spares the other chromosome copy; the genome-wide off-target risk remains. An independent enumeration reproduced the sequence geometry, and editing efficiency is unmeasured. A reference-allele reporter tests exclusivity: nick and edit signals at background level on the reference allele confirm it.

## References

- Morales AG et al. (2013). BUB1 and BUBR1 inhibition decreases proliferation and colony formation, and enhances radiation sensitivity in pediatric glioblastoma cells. *Childs Nerv Syst*. PMID [23728478](https://pubmed.ncbi.nlm.nih.gov/23728478/)
- Pfau SJ et al. (2016). Aneuploidy impairs hematopoietic stem cell fitness and is selected against in regenerating tissues in vivo. *Genes Dev*. PMID [27313317](https://pubmed.ncbi.nlm.nih.gov/27313317/)
- Laberko A et al. (2019). Hematopoietic stem cell transplantation in a patient with type 1 mosaic variegated aneuploidy syndrome. *Orphanet J Rare Dis*. PMID [31053147](https://pubmed.ncbi.nlm.nih.gov/31053147/)
- Everette KA et al. (2023). Ex vivo prime editing of patient haematopoietic stem cells rescues sickle-cell disease phenotypes after engraftment in mice. *Nat Biomed Eng*. PMID [37069266](https://pubmed.ncbi.nlm.nih.gov/37069266/)
- Fiumara M et al. (2024). Genotoxic effects of base and prime editing in human hematopoietic stem cells. *Nat Biotechnol*. PMID [37679541](https://pubmed.ncbi.nlm.nih.gov/37679541/)
- Shao C et al. (2024). Efficient and in situ correction of hemoglobin Constant Spring mutation by prime editing in human hematopoietic cells. *Mol Ther Nucleic Acids*. PMID [39640014](https://pubmed.ncbi.nlm.nih.gov/39640014/)
- Mathis N et al. (2025). Machine learning prediction of prime editing efficiency across diverse chromatin contexts. *Nat Biotechnol*. PMID [38907037](https://pubmed.ncbi.nlm.nih.gov/38907037/)
- Gori JL et al. (2026). Prime Editing for p47phox-Deficient Chronic Granulomatous Disease. *N Engl J Med*. PMID [41358590](https://pubmed.ncbi.nlm.nih.gov/41358590/)
- Wolff JH et al. (2026). Prime editing of human hematopoietic stem cells for correction of GATA2 deficiency. *Sci Transl Med*. PMID [42814803](https://pubmed.ncbi.nlm.nih.gov/42814803/)

## Other sources

- Spacer, PAM and pegRNA geometry: computed from the GRCh38 reference sequence around *BUB1B* c.2210 and c.3006 (Ensembl REST, regions 15:40209671-40209731 and 15:40220582-40220642, re-read 2026-10-24). Efficiency scores: PRIDICT2.0, PMID [38907037](https://pubmed.ncbi.nlm.nih.gov/38907037/) (DOI 10.1038/s41587-024-02268-2) [UNVERIFIED: the version used in the project run is not recorded].
- Monte Carlo projection: a pre-registered model whose inputs are the cited papers [UNVERIFIED: the model, its pre-registration and its code are not published with this report].
