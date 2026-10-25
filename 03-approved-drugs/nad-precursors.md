# NAD+ precursors

## Candidate

Nicotinic acid (niacin) is approved for lipid disorders; its label states that safety and effectiveness in children and adolescents have not been established (Niacor label). Nicotinamide riboside is sold as a dietary supplement [UNVERIFIED: no regulatory source recorded].

Both raise cellular NAD+ (nicotinamide adenine dinucleotide, a coenzyme of cellular metabolism) by different routes. Nicotinic acid needs the enzyme nicotinate phosphoribosyltransferase (NAPRT; PubMed identifier, PMID [42017774](https://pubmed.ncbi.nlm.nih.gov/42017774/)), and nicotinamide riboside enters through nicotinamide riboside kinases (PMID [15137942](https://pubmed.ncbi.nlm.nih.gov/15137942/)).

Nicotinamide, the vitamin form, inhibits sirtuins (NAD+-dependent deacetylase enzymes: yeast Sir2 and human SIRT1 in vitro, PMID [12297502](https://pubmed.ncbi.nlm.nih.gov/12297502/); SIRT2 acting on BubR1 in vitro, PMID [24825348](https://pubmed.ncbi.nlm.nih.gov/24825348/)) and is excluded as a candidate. Use in mosaic variegated aneuploidy (MVA, a syndrome in which cells carry varying chromosome numbers) would be off-label (outside the approved indications).

## Hypothesis

Raising NAD+ activates the deacetylase sirtuin 2 (SIRT2), an enzyme that removes acetyl groups. SIRT2 removes the acetyl mark at lysine 668 (K668) of BubR1, the protein encoded by *BUB1B*, and that mark targets BubR1 for degradation. A longer BubR1 half-life would raise the level of the missense protein (the child's protein with one amino acid replaced).

Each row of the table is one causal step, with a basis label defined in the [section 3 README](README.md#basis-labels): Demonstrated, Suggested, Our inference or Speculation.

| # | Step | Basis | System | Source |
|---|---|---|---|---|
| 1 | An oral precursor raises NAD+ in blood | Suggested | Human blood, single-arm open-label studies in ataxia telangiectasia (an inherited DNA-repair disorder) | PMID [42449929](https://pubmed.ncbi.nlm.nih.gov/42449929/) |
| 2 | The precursor raises NAD+ in the cells that carry the defect (dividing marrow, growth plate, muscle) | Speculation | None; tissue reach is unmeasured | No source found |
| 3 | Higher NAD+ increases SIRT2 activity on BubR1 | Suggested | HeLa cells (a human cervical cancer line) and mouse embryonic fibroblasts with sirtuin inhibitors, SIRT2 knockdown and overexpression; mouse testis after nicotinamide mononucleotide (NMN) (n = 3, one tissue); NMN raised BubR1 in wild-type mouse embryonic fibroblasts and almost not in Sirt2-knockout ones. A second group found no change in total BubR1 after SIRT2 knockdown in HCT116 cells (a human colon cancer line) | PMID [24825348](https://pubmed.ncbi.nlm.nih.gov/24825348/); PMID [25285631](https://pubmed.ncbi.nlm.nih.gov/25285631/) |
| 4 | SIRT2 removes the K668 acetyl mark that targets BubR1 for degradation | Suggested | HEK293T cells (a human embryonic kidney line) with overexpression and acetyl-mimic mutants; one group; a second group reports the opposite effect for K250 acetylation; the acetyl may sit on K667 (Evidence against) | PMID [24825348](https://pubmed.ncbi.nlm.nih.gov/24825348/); PMID [19407811](https://pubmed.ncbi.nlm.nih.gov/19407811/) |
| 5 | Loss of the K668 mark lengthens BubR1 half-life and raises its level | Suggested | Cell lines; a SIRT2 transgene raised BubR1 in hypomorph (reduced-function) mouse tissue without reaching wild-type level | PMID [24825348](https://pubmed.ncbi.nlm.nih.gov/24825348/) |
| 6 | The same switch controls turnover of the child's N1002K protein | Speculation | None; N1002K (asparagine to lysine at position 1002) is untested, and kinase-region missense proteins were cleared by turnover that depends on heat shock protein 90 (HSP90) and the proteasome in cell lines | PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/) (context only) |
| 7 | A 1.69- to 2.45-fold rise in the missense protein reaches the threshold of 0.13 (13% of wild-type BubR1, the level that gave near-normal segregation) | Our inference | Dose-response model; assumes the missense protein keeps about 11 to 15% of one wild-type allele's functional abundance; the threshold comes from one titration in HeLa cells | PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/); section [5.7](../05-computational-findings.md) |
| 8 | Reaching the threshold improves the child's marrow, growth or other clinical features | Speculation | None in MVA; the lifespan gain in hypomorph mice came from a SIRT2 transgene, and the precursor was given to wild-type mice | PMID [24825348](https://pubmed.ncbi.nlm.nih.gov/24825348/) |

Basis: 0 steps Demonstrated, 4 Suggested, 1 Our inference, 3 Speculation.

## Delivery and exposure

Both agents are oral. Nicotinamide riboside raised NAD+ in peripheral blood in two open-label studies in ataxia telangiectasia, as summarised in PMID [42449929](https://pubmed.ncbi.nlm.nih.gov/42449929/) (Suggested: human blood, open label).

Tissue reach into dividing marrow or growth-plate cells is unmeasured [UNVERIFIED: no source found] (Speculation).

The mouse result used 500 mg/kg/day intraperitoneally for 7 days (PMID [24825348](https://pubmed.ncbi.nlm.nih.gov/24825348/)). The oral human exposure that corresponds to that dose is unsourced [UNVERIFIED: no dose conversion sourced] (Speculation).

The only human trial found in a related syndrome is a single-arm, open-label study of nicotinamide riboside in ataxia telangiectasia, with participants of all ages (PMID [37899683](https://pubmed.ncbi.nlm.nih.gov/37899683/); abstract read). Ten participants received 2 x 250 mg/day by mouth, and the analysis measured blood cells only (PMID [42449929](https://pubmed.ncbi.nlm.nih.gov/42449929/); full text read). The participants' ages are unreported in the papers read.

Nicotinic acid causes flushing, gastrointestinal effects and raised uric acid at lipid-lowering exposure (US Food and Drug Administration label, Niacor).

The usefulness of the precursor depends on its conversion to NAD+ inside cells that carry the missense allele; that conversion is unmeasured (Our inference).

## Evidence for

- A genetic SIRT2 gain and a short NMN course raised BubR1 in mice (PMID [24825348](https://pubmed.ncbi.nlm.nih.gov/24825348/); main text, legends and methods read; supplementary figures not opened).
  - Acetylation at K668 by the acetyltransferase CREB-binding protein (CBP) lowered BubR1 stability and SIRT2 reversed it, shown mainly in HEK293T overexpression and mouse embryonic fibroblasts.
  - NMN at 500 mg/kg/day intraperitoneally for 7 days raised NAD+ and restored testis BubR1 in aged wild-type mice to the young level (three mice per group, one tissue).
  - A SIRT2 transgene raised BubR1 in BubR1 hypomorph (H/H) mouse tissues without restoring wild-type levels and extended median lifespan by 58% (n = 31 versus 33; log-rank P = 0.038; maximum lifespan +21%). The lifespan result came from the transgene; the precursor was given to wild-type mice.
- In a single-arm, open-label study of nicotinamide riboside in ataxia telangiectasia, blood transcriptomes of 10 patients at baseline, 6 and 12 months showed suppressed interferon-response genes (PMID [42449929](https://pubmed.ncbi.nlm.nih.gov/42449929/); full text read). The authors state the study was too small and too short to assess malignancy risk. The interferon effect is a different mechanism from the BubR1 hypothesis.
- A narrative review reports improved DNA repair and mitochondrial function from NAD supplementation in models and early human studies of premature-ageing and repair disorders, relates benefit to low baseline NAD+, and notes that some studies show no benefit (PMID [41436848](https://pubmed.ncbi.nlm.nih.gov/41436848/); abstract read; no new data).

## Evidence against

- One research network produced the mechanism and the mouse papers behind it. The senior author of PMID [24825348](https://pubmed.ncbi.nlm.nih.gov/24825348/) discloses consulting and patents licensed to companies working on NAD+ and sirtuin modulation.
- The male-only lifespan effect (+123%, n = 16 versus 17; no effect in females, n = 15 versus 16) is a sex subgroup that the authors reported as a surprise, and the overall result is borderline (P = 0.038).
- Independent data on aneuploidy in hypomorph tissues exist (PMID [27313317](https://pubmed.ncbi.nlm.nih.gov/27313317/)) but do not test the NAD+ mechanism. No independent replication of it was found in the papers read.
- SIRT2 overexpression in wild-type mice did not change health or lifespan in either sex on standard chow, or in males on a high-fat diet (PMID [38009412](https://pubmed.ncbi.nlm.nih.gov/38009412/); full text read). That study shares authors with the 2014 paper, including its senior author, so the two reports come from one network. The result fits a benefit limited to a BubR1 deficit.
- A second group found SIRT2 deacetylates lysine 250 of BubR1, a different site, and that SIRT2 knockdown in HCT116 cells left total BubR1 and mitotic timing unchanged (PMID [25285631](https://pubmed.ncbi.nlm.nih.gov/25285631/); full text read).
- The K668 acetylation has no independent primary report. A scan of 747 papers by this report (607 open full texts, 2014 to 2026) found K668 named in at least 11, each a review, a citation, an unrelated site or a paper sharing an author with the 2014 report [UNVERIFIED: the scan is not published with this report]. The one independent human-cell result on SIRT2 and BubR1 level is a null result: SIRT2 knockdown in G361 melanoma cells left BUB3, BUB1 and BubR1 unchanged on immunoblots, and SIRT1 knockdown lowered all three (PMID [24743044](https://pubmed.ncbi.nlm.nih.gov/24743044/); full text read; no quantification stated).
- The acetylated residue may be K667. The 2014 report assigned the acetyl to K668 from a tandem mass spectrum of overexpressed BubR1 and an antibody (PMID [24825348](https://pubmed.ncbi.nlm.nih.gov/24825348/); supplement not opened). In the public PRIDE/PTMeXchange proteomics records returned by the European Bioinformatics Institute (EBI) Proteins application programming interface (API) on 2026-10-24, the acetyl on the peptide spanning residues 648 to 668 sits on K667 (project PXD005252), and ubiquitin sits on K667 in two projects and on K668 in one. Processed records carry no localisation probability and raw spectra were not reviewed, so the site is unresolved (Our inference).
- A mouse oocyte study ties the Sirt2 effect to K243, the K250 equivalent (PMID [29067790](https://pubmed.ncbi.nlm.nih.gov/29067790/); abstract read). A summary kept by this report records no effect of mutating K657, the K668 equivalent [UNVERIFIED: the abstract does not report K657].
- K668 lies in the binding motif for PP2A-B56 (protein phosphatase 2A with its B56 subunit, which BubR1 recruits to kinetochores, the spindle attachment sites on chromosomes), residues 668 to 675, and is one of four motif residues reported to contact B56 (PMID [33892776](https://pubmed.ncbi.nlm.nih.gov/33892776/); review from the laboratory that reported the K668 mark; full text read). The review suggests the mark may act in mitosis and in error correction as well as in turnover. No paper has tested that.
- K668 lies outside the pseudokinase region (a kinase-like domain) that carries N1002K.
  - Kinase-region missense proteins were 5- to 10-fold less abundant than wild type when expressed in HeLa and U2OS cells (a human bone cancer line), and the authors attribute this to faster turnover that depends on HSP90 and the proteasome (PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/); main text and legends read).
  - The turnover data come from 5-hour drug treatments, a roughly two-fold faster loss in patient-derived lymphoblastoid cells (3 experiments) and a single representative HSP90 and proteasome experiment in U2OS cells. N1002K itself was not measured.
  - A kinase-proximal missense product may therefore be cleared by protein quality control (the cell's removal of misfolded proteins), a route separate from acetylation. No paper connects the SIRT2 switch to that route.
- Raising BubR1 level may restore the checkpoint response without restoring PP2A-B56 function. Overexpressing the kinase-region variants I909T and L1012P to near-wild-type level restored the response to nocodazole (a spindle poison) in one representative experiment (PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/)). A later study equalised kinetochore BubR1 level in HeLa cells and tested three pseudokinase-domain lesions (a truncation at residue 731 and two kinase-dead point mutants). None restored B56 recruitment or mitotic-exit timing, and the truncation and the double kinase-dead mutant had lower phosphorylation of the B56-binding motif per unit BubR1 (PMID [33207204](https://pubmed.ncbi.nlm.nih.gov/33207204/); preprint full text read, published version abstract only; Suggested). N1002K lies in this domain. In the papers read, no patient missense allele was measured on this function at equal BubR1 abundance, and the dose-response model under Expected effect carries that gap as the unmeasured specific activity.
- If BubR1 level rises but PP2A-B56 function does not recover, a cell could regain an adequate checkpoint and stay weak at error correction. That state predicts lagging chromosomes and micronuclei (small extra nuclei, a marker of chromosome loss or breakage) rising while the nocodazole arrest improves and mitosis lengthens (Our inference; the net sign is unknown). The papers disagree on the 731-residue truncation: it retained segregation function in one (PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/)) and failed to restore B56 recruitment in the other (PMID [33207204](https://pubmed.ncbi.nlm.nih.gov/33207204/)). The two results remain in conflict.
- The hypomorph lifespan effect came from a transgene, was concentrated in males and left kyphosis, cataract and small size unchanged (PMID [24825348](https://pubmed.ncbi.nlm.nih.gov/24825348/)). The authors link the gain to improved cardiac repolarisation.
- Acetylation at K250 has the opposite reported effect: acetylation by the acetyltransferase p300/CBP-associated factor (PCAF) protects BubR1 from degradation, whereas K668 acetylation promotes it (PMID [19407811](https://pubmed.ncbi.nlm.nih.gov/19407811/); HeLa cells with overexpression and acetyl-mimetic mutants; one group). How the two marks combine in vivo is unresolved.
- Nicotinamide, the product of NAD+ consumption, inhibits sirtuins, so a precursor that raises nicotinamide could cancel the effect.
- NAD+ metabolism drives the pro-inflammatory secretome (the set of proteins a cell secretes) of senescent cells (cells in permanent growth arrest): nicotinamide phosphoribosyltransferase (NAMPT), the rate-limiting NAD+ salvage enzyme, promoted interleukin (IL)-1 beta, IL-6 and IL-8 expression in senescent human fibroblasts, and the authors conclude that NAD+ augmentation should be administered with precision (PMID [30778219](https://pubmed.ncbi.nlm.nih.gov/30778219/); full text read).
  - In KRAS-driven pancreas mice (8 weeks old, n = 10 per group), NMN at 500 mg/kg/day intraperitoneally for 13 days reduced normal acinar area and raised inflammatory cytokine mRNA and immune infiltration. Tumour burden, lesion grade and survival were not measured, so the pro-tumour reading rests on those proxies.
  - [Anakinra](il1-blockade.md) targets the same IL-1 signal, so the two candidates pull in opposite directions on one secretome.
- Paediatric rhabdomyosarcoma depends on NAD+ synthesis: NAPRT-deficient tumour cells (30% to 40% of 109 primary tumours lacked NAPRT protein) were sensitive to NAMPT inhibitors through NAD+ depletion, and nicotinic acid did not rescue them (PMID [42017774](https://pubmed.ncbi.nlm.nih.gov/42017774/); abstract read). The study tested NAD+ depletion and shows tumour dependence on NAD+. The tumour-risk direction of raising NAD+ remains open.

## Safety

Gate numbers follow the seven-gate screen in [Screening criteria](README.md#screening-criteria).

- Gate 1 (genotoxicity): nicotinic acid was negative in the Ames test (a bacterial mutation assay) and not carcinogenic in lifelong mouse exposure (Niacor label). No genotoxicity source was found for nicotinamide riboside [UNVERIFIED].
- Gate 2 (aneugenicity) passes on direct mechanism: no mitotic mechanism is known for either precursor [no source recorded]. The hazard that a higher BubR1 level leaves error correction weak (Evidence against) has a stopping criterion in the Test.
- Gate 3 (paediatric exposure) is open: the nicotinic acid label states that safety and effectiveness in children are not established, and the one nicotinamide riboside trial found is in ataxia telangiectasia participants of all ages, with no age breakdown in the abstract read.
- Gate 4 is a flag: the tumour and inflammation findings above point both ways and are untested in MVA.
- Gate 5 (chronic-use tolerability) is a flag for nicotinic acid: the label warns of severe hepatic toxicity when a sustained-release product replaces an immediate-release one, and of raised uric acid and impaired glucose tolerance. The 2-year nicotinamide riboside trial reports good tolerability in most participants (PMID [37899683](https://pubmed.ncbi.nlm.nih.gov/37899683/); abstract read).
- Gate 6 (interactions): the label lists interactions with HMG-CoA reductase inhibitors (statins), antihypertensives and aspirin. The check against the child's own medicines is outside this report.
- Check against the child's other genetic findings (the secondary finding and the four unnamed carrier-state variants): pending, gene by gene ([section 3 README](README.md#check-against-the-childs-other-genetic-findings)).

## Expected effect

Basis: Our inference throughout, from the dose-response model (section [5.7](../05-computational-findings.md)) applied to Suggested inputs from cell lines and mouse. The projection depends on the unmeasured abundance and specific activity of the missense protein; their product, as a fraction of one wild-type allele, is its functional abundance. The partner allele makes no protein, so the child's residual functional BubR1, as a fraction of a wild-type cell, equals half the functional abundance. The table sets two target levels against the fold increase each would need at example residuals.

| Target | Level of functional BubR1 | Fold needed at the child's residual | Reachable with the measured fold (1.69 to 2.45 in mouse) |
|---|---|---|---|
| Threshold for near-normal segregation in a human cell titration (doxycycline-titrated HeLa cells: 13% BubR1 gave near-normal segregation, 6% gave errors in most cells; one titration series, PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/)) | 0.13 of wild type | 6.5-fold at 0.02, 1.3-fold at 0.10, none at 0.15 | Only if the missense protein keeps about 11 to 15% of one wild-type allele's functional abundance |
| Carrier level | 0.5 of wild type | 25-fold at 0.02, 5-fold at 0.10, 2-fold at 0.25 | Only if functional abundance is at least 0.41 to 0.59 |

Measured folds (Suggested; this report estimated them from blot quantification in the original figures, which adds an Our inference step): 1.69 in young wild-type mouse testes and 2.45 as recovery of an age-depressed level (PMID [24825348](https://pubmed.ncbi.nlm.nih.gov/24825348/), three mice per group, one tissue); 2.2 in hypomorph testes from the SIRT2 transgene (same paper).

A change in turnover alone is bounded near 2-fold (Our inference) by the roughly two-fold faster turnover of two kinase-region missense proteins. The turnover was measured by cycloheximide chase (blocking new protein synthesis to follow decay) in cell lines (PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/), n = 3 experiments).

Five of five measured disease-associated kinase-region substitutions are low in abundance, 5 to 10 times below wild type when expressed in HeLa and U2OS cells (PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/); Suggested), which gives a functional abundance of at most 0.1 to 0.2 if specific activity is normal (1/10 and 1/5). That range lies below the 0.41 to 0.59 that carrier level needs, so the projection favours the near-normal-segregation threshold over carrier level as the target (Our inference).

The projection assumes that function tracks abundance. The equal-abundance comparisons under Evidence against do not support that for other pseudokinase lesions, so functional abundance may overstate function (Our inference).

The candidate would be expected (Our inference) to leave unchanged aneuploidy that has already occurred, a stop-gain allele (a variant that creates a premature stop codon), tissues the precursor does not reach and PP2A-B56 function, which a higher level may not repair.

The 0.13 threshold rests on a titration series in HeLa cells, which carry a high level of aneuploidy (PMID [23550136](https://pubmed.ncbi.nlm.nih.gov/23550136/); abstract read; Suggested). A second HeLa series with short hairpin RNA (shRNA) used one hairpin per residual level (8.5% to 77%) and reported aneuploidy at every level below 50%, which includes 14%, a level that the titration series scores as near-normal (PMID [18932004](https://pubmed.ncbi.nlm.nih.gov/18932004/); the levels and the aneuploidy result are from the abstract). Its readout was DNA content above 4N (four genome copies) after nocodazole, which measures checkpoint strength and polyploidisation more than chromosome gain or loss. The 0.13 threshold is therefore the more permissive reading (Our inference).

**Weakest link:** step 6, because no paper tests whether the K668 switch controls turnover of N1002K, the kinase-region data point to a different clearance route, and a higher level may not restore PP2A-B56 function.

## Test

- **System:** isogenic cell lines (lines that differ only in the BubR1 variant) carrying the missense allele, and patient-derived cycling cells.
- **Readout:** BubR1 level and half-life by cycloheximide chase at equal protein abundance, with intracellular NAD+ and acetylation at K667 and K668 (synthetic acetyl-peptide standards) measured in the same cells. At equal kinetochore BubR1 level, PP2A-B56 recruitment and phosphorylation of the B56-binding motif per unit BubR1, lagging chromosomes, micronuclei, mitotic duration and the nocodazole response. Positive control: wild-type BubR1 half-life. Negative control: a SIRT2 inhibitor arm.
- **Exposure:** precursor concentrations that raise intracellular NAD+ by no more than the rise reported in adults after oral supplementation [UNVERIFIED: the adult value is not yet sourced].
- **Pass criterion (fixed before the experiment):** half-life rises beyond the 95% interval of the untreated arm and the SIRT2 inhibitor abolishes the rise.
- **Stopping criterion:** half-life stays within control range, proteasome inhibition shows the protein is cleared by quality control, nicotinamide accumulation cancels the effect, PP2A-B56 recruitment or motif phosphorylation per unit BubR1 stays below the wild-type range at equal BubR1 abundance, or lagging chromosomes or micronuclei rise while the nocodazole arrest improves.

## Outcome if confirmed

A replication of the NAD+ mechanism outside its originating network, and a measured fold to place in the projection (Expected effect). A negative result closes the hypothesis for the missense allele and leaves it open only for under-expressed wild-type protein.

## References

- Bieganowski P, Brenner C (2004). Discoveries of nicotinamide riboside as a nutrient and conserved NRK genes establish a Preiss-Handler independent route to NAD+ in fungi and humans. *Cell*. PMID [15137942](https://pubmed.ncbi.nlm.nih.gov/15137942/)
- Bitterman KJ et al. (2002). Inhibition of silencing and accelerated aging by nicotinamide, a putative negative regulator of yeast sir2 and human SIRT1. *J Biol Chem*. PMID [12297502](https://pubmed.ncbi.nlm.nih.gov/12297502/)
- Bloom CR, North BJ (2021). Physiological relevance of post-translational regulation of the spindle assembly checkpoint protein BubR1. *Cell Biosci*. PMID [33892776](https://pubmed.ncbi.nlm.nih.gov/33892776/)
- Bohers E et al. (2008). Gradual reduction of BUBR1 protein levels results in premature sister-chromatid separation then in aneuploidy. *Hum Genet*. PMID [18932004](https://pubmed.ncbi.nlm.nih.gov/18932004/)
- Bohr VA (2026). Promising Results With NAD Supplementation in Rare Diseases With Premature Aging and DNA Damage. *Aging Cell*. PMID [41436848](https://pubmed.ncbi.nlm.nih.gov/41436848/)
- Choi E et al. (2009). BubR1 acetylation at prometaphase is required for modulating APC/C activity and timing of mitosis. *EMBO J*. PMID [19407811](https://pubmed.ncbi.nlm.nih.gov/19407811/)
- Gama Braga L et al. (2020). BUBR1 Pseudokinase Domain Promotes Kinetochore PP2A-B56 Recruitment, Spindle Checkpoint Silencing, and Chromosome Alignment. *Cell Rep*. PMID [33207204](https://pubmed.ncbi.nlm.nih.gov/33207204/)
- Kim A et al. (2026). NAPRT Expression and Epigenetic Regulation in Pediatric Rhabdomyosarcoma as a Potential Biomarker for NAMPT Inhibition. *Mol Cancer Ther*. PMID [42017774](https://pubmed.ncbi.nlm.nih.gov/42017774/)
- Landry JJM et al. (2013). The genomic and transcriptomic landscape of a HeLa cell line. *G3 (Bethesda)*. PMID [23550136](https://pubmed.ncbi.nlm.nih.gov/23550136/)
- Nacarelli T et al. (2019). NAD+ metabolism governs the proinflammatory senescence-associated secretome. *Nat Cell Biol*. PMID [30778219](https://pubmed.ncbi.nlm.nih.gov/30778219/)
- North BJ et al. (2014). SIRT2 induces the checkpoint kinase BubR1 to increase lifespan. *EMBO J*. PMID [24825348](https://pubmed.ncbi.nlm.nih.gov/24825348/)
- Pfau SJ et al. (2016). Aneuploidy impairs hematopoietic stem cell fitness and is selected against in regenerating tissues in vivo. *Genes Dev*. PMID [27313317](https://pubmed.ncbi.nlm.nih.gov/27313317/)
- Presterud R et al. (2024). Long-Term Nicotinamide Riboside Use Improves Coordination and Eye Movements in Ataxia Telangiectasia. *Mov Disord*. PMID [37899683](https://pubmed.ncbi.nlm.nih.gov/37899683/)
- Qiu D et al. (2018). Sirt2-BubR1 acetylation pathway mediates the effects of advanced maternal age on oocyte quality. *Aging Cell*. PMID [29067790](https://pubmed.ncbi.nlm.nih.gov/29067790/)
- Singh CK et al. (2014). Novel downstream molecular targets of SIRT1 in melanoma: a quantitative proteomics approach. *Oncotarget*. PMID [24743044](https://pubmed.ncbi.nlm.nih.gov/24743044/)
- Suaste V et al. (2026). Transcriptional Profiling Shows Dampening of Interferon Gene Signatures by NAD+ Augmentation in Ataxia-Telangiectasia. *Int J Mol Sci*. PMID [42449929](https://pubmed.ncbi.nlm.nih.gov/42449929/)
- Suematsu T et al. (2014). Deacetylation of the mitotic checkpoint protein BubR1 at lysine 250 by SIRT2 and subsequent effects on BubR1 degradation during the prometaphase/anaphase transition. *Biochem Biophys Res Commun*. PMID [25285631](https://pubmed.ncbi.nlm.nih.gov/25285631/)
- Suijkerbuijk SJ et al. (2010). Molecular causes for BUBR1 dysfunction in the human cancer predisposition syndrome mosaic variegated aneuploidy. *Cancer Res*. PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/)
- Wu LE et al. (2023). SIRT2 transgenic over-expression does not impact lifespan in mice. *Aging Cell*. PMID [38009412](https://pubmed.ncbi.nlm.nih.gov/38009412/)

## Other sources

- Niacor (niacin tablets), prescribing information, openFDA drug label API, search `openfda.brand_name:Niacor`, effective 2021-12-23, read 2026-10-24: https://api.fda.gov/drug/label.json?search=openfda.brand_name:Niacor

- PRIDE/PTMeXchange records of BubR1 (UniProt O60566) through the EBI Proteins API, https://www.ebi.ac.uk/proteins/api/proteomics-ptm/O60566, queried 2026-10-24: peptide TSEDQQTACGTIYSQTLSIKK (residues 648 to 668) acetylated at residue 667 (PXD005252) and ubiquitinylated at residue 667 (PXD006201, PXD023889); peptide KLSPIIEDSR (residues 668 to 677) ubiquitinylated at residue 668 (PXD027328). Processed identifications; raw spectra not reviewed.

- Scan by this report of 747 papers (607 open full texts) for K668 [UNVERIFIED: scan table not published with this report].
