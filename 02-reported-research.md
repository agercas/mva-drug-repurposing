# Reported research on BubR1 and mosaic variegated aneuploidy

Forty-three papers name both *BUB1B* and mosaic variegated aneuploidy (MVA) or premature chromatid separation (PCS) in the title or abstract. Case reports and clinical descriptions among them come from many unrelated groups, and mechanistic and intervention claims come from a few.

*BUB1B* encodes BubR1, a protein of the mitotic checkpoint, which delays chromosome separation until every chromosome is attached to the spindle. Each candidate card in sections 3 and 4 (the one-page summary of a candidate) states how many independent groups stand behind its mechanism, using the counts below.

Sections 2.3 to 2.5 grade the evidence behind the field's best-known claims and list the red flags and open questions for the most influential papers. The report treats every mechanism in the literature as provisional.

Contents:

- [2.1 Counts](#21-counts-by-topic)
- [2.2 Authorship](#22-authorship-and-independent-groups)
- [2.3 Appraisal method](#23-appraisal-method-and-grades)
- [2.4 Critical appraisal](#24-critical-appraisal-of-influential-papers)
- [2.5 Claims beyond the data](#25-claims-that-outrun-the-data)
- [2.6 Full-text findings](#26-findings-checked-in-full-text)
- [2.7 Narrower than cited](#27-findings-narrower-than-their-abstracts)
- [2.8 Clinical and preclinical data](#28-clinical-and-preclinical-data)
- [2.9 Papers without full text](#29-papers-without-accessible-full-text)
- [2.10 Open questions](#210-open-mechanistic-questions)

## 2.1 Counts by topic

Source: Europe PMC REST API, search date 2026-10-24, fields restricted to title or abstract (`TITLE_ABS`), preprints included. The table gives the record count for each search; topics overlap, so rows do not sum. The last row searches for hypomorph (an allele that leaves reduced gene function), NAD+ (nicotinamide adenine dinucleotide, a coenzyme required by sirtuin enzymes), SIRT2 (sirtuin 2, an NAD+-dependent enzyme that removes acetyl groups from proteins) and nicotinamide.

| Topic | Definition | Records |
|---|---|---|
| Gene | *BUB1B* or *BUBR1* | 1,409 |
| Mitosis | gene plus mitosis, mitotic, checkpoint or kinetochore | 933 |
| Cancer | gene plus cancer, tumour or carcinoma | 705 |
| Ageing | gene plus ageing, senescence or progeroid | 90 |
| MVA or PCS, any gene | MVA, premature chromatid separation or PCS syndrome | 136 |
| **Gene plus MVA or PCS** | both | **43** |
| of which patient or family terms | adds patient, family, biallelic, germline, heterozygous, homozygous or proband | 38 |
| of which treatment terms | adds treatment, therapy, therapeutic, drug, inhibitor or rescue | 7 |
| Gene plus hypomorph, NAD+, SIRT2 or nicotinamide | with treatment terms | 12 |

The 43 records span 2004 to 2026 and make up 3 percent of the 1,409. By title, 7 of the 43 concern other genes or conditions (*CEP57* three times, *TRIP13*, *BUB1*, *CDC20*, ring chromosome). The report uses title-or-abstract counts throughout: a search without the `TITLE_ABS` restriction also searches full text and returns 7,228 records for the gene alone (query `BUB1B OR BUBR1`, 2026-10-24).

Coverage check: the PubMed query `BUB1B[tiab] OR BUBR1[tiab]` returns 1,275 records on 2026-10-24, and 1,256 of them (98.5 percent) are among the 1,409 Europe PMC records of the gene search. The project corpus screened all retrieved records and read 280 in depth, from full text where open [UNVERIFIED: corpus counts; the number of full-text reads was not recomputed for this report]. A further 1,634 papers that mention BubR1 only in the body text sit behind paywalls and fall outside the reviewed set [UNVERIFIED: not recomputed].

## 2.2 Authorship and independent groups

Method: authors come from the Europe PMC author string and are matched by surname and initials. We excluded common names when linking papers. **Author identity rests on name matching only and is unverified.** We named four groups from the literature review and counted their records:

| Group (by name match) | Focus | In the 43 | In the 12 | In the 90 ageing | In the 1,409 |
|---|---|---|---|---|---|
| Matsuura, Kajii, Ikeuchi, Izumi, Miyamoto, Ochiai | patient cells, genetics | 5 | 0 | 1 | 6 |
| van Deursen, Baker, Jeganathan, Wijshake, Malureanu, Sieben, Jang | hypomorph mice | 5 | 4 | 26 | 35 |
| North, Sinclair | NAD+ and SIRT2 | 2 | 5 | 5 | 7 |
| Hanks, Rahman, Yost | discovery of *BUB1B* in MVA | 6 | 0 | 0 | 7 |
| Records with any of the four | | 18 of 43 | 7 of 12 | 30 of 90 | 53 of 1,409 |
| Co-author clusters, largest cluster | | 23, 7 records (16%) | 7, 6 records (50%) | 50, 35 records (39%) | not informative |

Reading the table:

- **Clinical reports are spread widely.** Authors outside the four groups wrote 25 of the 43 records (58 percent), and the largest co-author cluster holds 7 records.

- **Candidate mechanisms are concentrated.** Half of the 12 records on hypomorph, NAD+, SIRT2 or nicotinamide sit in one co-author cluster. The hypomorph-mouse group appears in 26 of the 90 ageing records.

- Few laboratories hold the hypomorph mice, which accounts for part of the concentration. Groups also overlap through shared papers and moves between laboratories, so the table understates how connected they are.

- In the full set of 1,409, shared authors join about half the papers into one cluster through the large mitosis community, so cluster size at that scale is uninformative about dependence.

### Dependence of each claim on research groups

The table lists, for each claim a candidate needs, the groups with primary data, the independent replication found and the read basis. PMID is the PubMed identifier.

| Claim a candidate needs | Groups with primary data | Independent replication found | Read basis |
|---|---|---|---|
| Acetylation and SIRT2 control BubR1 level; NAD+ precursors raise BubR1 (North 2014, PMID [24825348](https://pubmed.ncbi.nlm.nih.gov/24825348/)) | North and Sinclair with van Deursen | None among the papers read; one small interfering RNA (siRNA) experiment from another group left total BubR1 unchanged (Suematsu 2014, PMID [25285631](https://pubmed.ncbi.nlm.nih.gov/25285631/)) | full text (partial) and full text |
| A SIRT2 transgene extends life in a BubR1-deficient background (median of both sexes +58%, P = 0.038; the gain is confined to males) | same network | The same transgene left lifespan unchanged in wild-type mice (PMID [38009412](https://pubmed.ncbi.nlm.nih.gov/38009412/)), reported by a group that includes a senior author of the original paper; independent replication in a BubR1-deficient background: none among the papers read | full text |
| Hypomorph mouse phenotype: ageing and shortened lifespan (Baker 2004, PMID [15208629](https://pubmed.ncbi.nlm.nih.gov/15208629/)) | van Deursen laboratory | Partial: aneuploidy in tissues of the same hypomorph allele, from a different laboratory (PMID [27313317](https://pubmed.ncbi.nlm.nih.gov/27313317/)) | full text for 15208629; abstract and model description for 27313317 |
| Raised polo-like kinase 1 (PLK1) activity and centrosome amplification in patient cells (Izumi 2009, PMID [19503101](https://pubmed.ncbi.nlm.nih.gov/19503101/)) | Matsuura laboratory | None for patient cells. A conditional cortex knockout with about 0.5% residual BubR1 on a hypomorph background (Emx1-Cre, n = 3 per genotype, embryonic day 14.5 to postnatal day 21) left centrosome number and primary cilia unchanged (PMID [30668728](https://pubmed.ncbi.nlm.nih.gov/30668728/), partial full text; figures not verified) | abstract only for 19503101 |
| Cilia loss in patient fibroblasts (Miyamoto 2011, PMID [21389084](https://pubmed.ncbi.nlm.nih.gov/21389084/); Miyamoto 2015, PMID [25660017](https://pubmed.ncbi.nlm.nih.gov/25660017/)). Two patient lines and one control; rescued by transfer of chromosome 15, which carries other genes, while *BUB1B* complementary DNA failed to rescue | Matsuura laboratory | None | full text (partial) for both |
| Intergenic upstream variant as a second allele (Ochiai 2014, PMID [24344301](https://pubmed.ncbi.nlm.nih.gov/24344301/)). Shown by editing the base in a colon-cancer cell line (HCT116) with a transcription activator-like effector nuclease; the paper leaves the intermediate regulatory mechanism open | Matsuura and Ochiai | None | full text (partial) |
| Gradual loss of BubR1 raises premature chromatid separation (Bohers 2008, PMID [18932004](https://pubmed.ncbi.nlm.nih.gov/18932004/)). Five hairpin lines in HeLa cells (a cervical-cancer line), one line per residual level; aneuploidy defined as DNA content above 4N | one group, human cells | The mouse dose-response (Baker 2004) is from a different group and system | full text |
| Patient genotypes and clinical features | many clinical groups | Yes | full text for the founding reports |

The report reserves the word "validated" for results with an independent replication, and none of the mechanisms above has one in the papers read.

## 2.3 Appraisal method and grades

Each claim that a candidate relies on receives one of three grades, defined below.

| Grade | Criteria |
|---|---|
| Demonstrated | Tested by manipulation in both directions (loss and gain, or loss and rescue), by more than one method, with sample sizes and effect sizes with intervals reported, and reproduced by an independent research group |
| Suggested | One method, one model system or one research group, or a subgroup analysis chosen after the data were seen |
| Speculative | Stated as an interpretation in a discussion or review and untested by any experiment in the paper |

The checklist applied to every paper covers:

- the type of evidence (association, loss of function, gain of function, rescue);
- the sample size of each experiment, subgroup analyses and multiplicity (correction for many comparisons);
- the controls (positive, negative, drug-only, vehicle);
- whether the effect came from the manipulation named in the title;
- replication and the number of independent groups;
- conflicts of interest;
- the abstract compared with the data;
- the outcomes reported or omitted (deaths, adverse events, phenotypes left unrescued).

Read basis terms:

- "Full text re-read" means the text was opened for this report.
- "Earlier appraisal" means this report relies on the earlier full-text appraisal in the project record and did not reopen the paper.

A paper cited by hundreds of records receives the same grade as a paper cited by few with the same evidence. Citation counts come from the Europe PMC snapshot of the project corpus and measure influence.

## 2.4 Critical appraisal of influential papers

**Selection.** The first group of papers carries a step in a mechanism chain in sections 3 to 5 and the appendix. The second group holds the most cited papers on BubR1, the spindle checkpoint and checkpoint-gene dosage (at least 200 citing records in the Europe PMC snapshot of 2026-10-24, drawn from the project corpus), plus the founding reports on MVA. Yeast, general cancer-expression prognosis and methods papers fall outside the selection. Each block grades its claims in a table.

### 2.4.1 North 2014: SIRT2 and lifespan

**Claim as widely cited.** SIRT2 and NAD+ stabilise BubR1, and the title states that SIRT2 "induces the checkpoint kinase BubR1 to increase lifespan" (EMBO J, PMID [24825348](https://pubmed.ncbi.nlm.nih.gov/24825348/); about 200 citing records). The paper is the main basis for proposing NAD+ precursors in BubR1 deficiency.

**What was done** (full text re-read; supplementary figures not opened).

- Cell lines: nicotinamide at 20 mM and sirtinol lowered BubR1 in HeLa cells; Sirt2-knockout fibroblasts and SIRT2 knockdown lowered it, and SIRT2 overexpression raised it (Fig. 1, Student's t-test, n = 3).

- Overexpression in 293T cells (a human embryonic kidney line): the acetyltransferase CREB-binding protein (CBP) acetylates and SIRT2 deacetylates BubR1 (Fig. 2). Lysine 668 (K668) was identified by mass spectrometry of an in vitro reaction and with an acetyl-specific antibody; K668Q and K668R mutants changed stability (Fig. 3).

- Mice: a SIRT2 transgene in BubR1 H/H hypomorph mice (Fig. 4). Median lifespan of both sexes +58%, P = 0.0384 by log-rank test (n = 31 against 33), maximum lifespan +21%. Males: +123%, P = 0.004 (n = 16 against 17). Females: P = 0.7915 (n = 15 against 16).

- Drug: nicotinamide mononucleotide (NMN), 500 mg/kg/day by intraperitoneal injection for 7 days, n = 3 per group; BubR1 could be read in testis (Fig. 6).

**Red flags and open questions**

1. **The lifespan effect and the drug experiment used different animals.** The lifespan gain came from the SIRT2 transgene in BubR1 H/H mice (Fig. 4); NMN was tested only in aged wild-type mice, for NAD+ and BubR1 level (Fig. 6). The title and abstract join the transgene result and the NMN result in one narrative. Open point: whether any NAD+ precursor has been tested for lifespan or BubR1 level in a BubR1-deficient animal since 2014; none was found in the papers read.

2. **The gain for both sexes rests on one cohort.** P = 0.0384 with 31 and 33 animals, and maximum lifespan rose 21% (Fig. 4A).

3. **The male-only effect is a post hoc subgroup.** The Discussion states that the authors "were initially surprised" that the effect was sex-specific. The statistical analysis section lists a log-rank test and a t-test and reports no multiplicity adjustment and no pre-specified sex stratification. Open points: whether sex was declared as a stratification factor before the cohort was set up, how many comparisons were made, and the median lifespans of the male and female control groups.

4. **The sex bias received a post hoc explanation.** The Discussion cites a male bias in lifespan extension by transgenic BubR1 overexpression from the same network (Baker 2013, PMID [23242215](https://pubmed.ncbi.nlm.nih.gov/23242215/)) as "a shared etiology". The Results hypothesise a cardiac cause for the sudden late deaths in hypomorph mice, because males are more prone to cardiac abnormalities (text around Fig. 5). Two transgenic lines from one network leave the mouse background or the cause of death open. Open point: whether male and female hypomorph controls die of different causes.

5. **SIRT2 may act through other targets.** BubR1 stayed below wild-type levels, and the small size, lordokyphosis (spinal curvature) and cataracts persisted (Supplementary Fig. S4). The Discussion states "a strong possibility that SIRT2 has additional targets". The paper contains no K668R knock-in mouse and no catalytic-dead SIRT2 rescue. The title asserts a chain through BubR1 that the experiments leave open.

6. **The cell-based mechanism rests on overexpression.** Nicotinamide at 20 mM and sirtinol inhibit seven sirtuins, and the paper chose SIRT2 from that set by expression site. K668 acetylation was shown with overexpressed CBP and SIRT2 in 293T cells, in a purified reaction and with acetyl-mimic mutants. The fraction of endogenous BubR1 acetylated at K668 was not measured (Fig. 2, Fig. 3).

7. **The drug experiment used 3 mice per group.** NMN was given for 7 days, NAD+ rose in heart and testis, and BubR1 was "difficult to determine" in aged heart; the BubR1 result rests on one tissue (Fig. 6D, E). The abstract states that NMN "increases BubR1 abundance in vivo".

8. **Conflict of interest.** The senior author is a consultant to and inventor on patents licensed to companies working on NAD+ and sirtuin modulation (Conflict of interest statement).

9. **Opposite sign at another site.** Acetylation at lysine 250 (K250) stabilises BubR1 in HeLa cells (Choi 2009, PMID [19407811](https://pubmed.ncbi.nlm.nih.gov/19407811/)), and SIRT2 knockdown raised K250 acetylation while total BubR1 stayed unchanged in one siRNA experiment (Suematsu 2014, PMID [25285631](https://pubmed.ncbi.nlm.nih.gov/25285631/), full text read). Open point: whether SIRT2 acts on K250, K668 or both, and the net effect on BubR1 level.

**Replication.** The same SIRT2 transgene left lifespan unchanged in wild-type mice (males 869 against 862 days, females 723 against 722 days; PMID [38009412](https://pubmed.ncbi.nlm.nih.gov/38009412/), full text re-read). The study was powered to detect a 10% median difference with 80% power. The cohort was not assayed for BubR1, K668 acetylation or NAD+.

The authors include the senior author of the 2014 paper and the investigator who supplied reagents for it, and two authors declare shareholdings in NAD+ precursor companies. This result narrows the claim to a BubR1-limited setting; the hypomorph result awaits an independent test. Research groups with primary data on the NAD+ and SIRT2 arm: one network.

| Claim | Grade | Reason |
|---|---|---|
| SIRT2 and CBP control BubR1 level through K668 in cultured cells | Suggested | One group, overexpression and acetyl-mimic mutants, n = 3 blots, opposite-sign K250 data from another group |
| SIRT2 transgene extends median lifespan of BubR1 H/H mice | Suggested | One cohort, P = 0.0384, no independent cohort |
| The effect is male-specific | Suggested | Post hoc subgroup, no multiplicity adjustment |
| NMN raises BubR1 in vivo | Suggested | n = 3 per group, one tissue, 7 days |
| NAD+ precursors extend life or improve phenotypes in BubR1 deficiency | Speculative | No experiment in the paper |
| BubR1 stabilisation explains the lifespan gain | Speculative | The authors state additional SIRT2 targets are likely |

**Use in this report.** The NAD+ precursor candidate in section 3 treats the SIRT2 step as a hypothesis to test in cells carrying the missense allele, and the card lists the main red flags above under evidence against.

### 2.4.2 Baker 2004: BubR1 hypomorph mouse

**Claim as widely cited.** BubR1 insufficiency causes early ageing, and BubR1 declines with age in normal tissues (Nat Genet, PMID [15208629](https://pubmed.ncbi.nlm.nih.gov/15208629/); about 590 citing records).

**What was done** (earlier appraisal of the full text; the full text was not reopened for this report). An allelic series gave residual BubR1 of 42% (+/H), 29% (+/-), 11% (H/H) and 4% (-/H), quantified in fibroblasts (n = 6 blots per genotype). H/H mice lived a median of about 6 months with cachexia (body wasting), lordokyphosis, cataracts, fat loss, infertility and aneuploidy.

**Red flags and open questions**

1. The hypomorph keeps 11% BubR1 in every tissue from conception. The phenotypes may combine developmental and non-checkpoint effects, and the paper reports no experiment that separates them (Fig. 1, Table 1).

2. Aneuploidy and ageing phenotypes appear together; the text calls the link "suggestive". The paper contains no experiment that reduces aneuploidy and tests the ageing phenotype.

3. The claim that BubR1 declines with age in normal tissues rests on unquantified blots and immunofluorescence (sample size, sex and strain unstated), on whole ovary, with aged tissue from a tissue bank (Fig. 5d to f). BubR1 at 22 to 32 months remains far above the 11% of the hypomorph. Open point: the quantified residual BubR1 per tissue at old age.

4. Several readouts rest on small groups: body-fat scans and skin thickness (n = 3 per group), sperm counts (n = 3) and oocytes (13 and 14).

5. The text gives 230 H/H animals and the figure legend gives 212; the difference is unexplained.

6. Apoptosis and DNA-repair results are "data not shown" in the text read.

**Replication.** The hypomorph line has been used in later papers from the same network (Baker 2008, PMID [18516091](https://pubmed.ncbi.nlm.nih.gov/18516091/); Baker 2011, PMID [22048312](https://pubmed.ncbi.nlm.nih.gov/22048312/); North 2014). A different laboratory reports aneuploidy in tissues of the same hypomorphic allele, with euploid stem cells and regenerating tissues (PMID [27313317](https://pubmed.ncbi.nlm.nih.gov/27313317/); abstract and model description read).

| Claim | Grade | Reason |
|---|---|---|
| Graded BubR1 reduction produces a threshold: nothing at 29 to 42%, severe phenotype at 11% | Suggested | One group, mouse |
| Aneuploidy drives the ageing phenotypes | Speculative | Association only |
| BubR1 decline contributes to normal ageing | Speculative | Unquantified blots |

**Use in this report.** The graded fibroblast levels supply five of the ten readouts that fit the dose-response model in the [error-free division appendix](appendix/error-free-division.md); the threshold reading carries the label Suggested.

### 2.4.3 Baker 2011 and 2016: senescent-cell clearance

**Claim as widely cited.** Removing p16Ink4a-positive senescent cells delays ageing disorders (Nature, PMID [22048312](https://pubmed.ncbi.nlm.nih.gov/22048312/); about 3,070 citing records), and extends lifespan in normal mice (Nature, PMID [26840489](https://pubmed.ncbi.nlm.nih.gov/26840489/)).

**What was done.** The 2011 paper used the INK-ATTAC transgene, which kills cells that activate the p16Ink4a promoter after a dimerising drug, in BubR1 H/H mice (abstract read; earlier appraisal of the full text). Life-long clearance delayed lordokyphosis, cataracts, muscle-fibre loss and fat loss. Heart, aorta and survival were not substantially improved. The 2016 paper used wild-type mice only (full text re-read): median lifespan rose 24% to 27% (17% to 35% by sex and background); maximum lifespan was unchanged in C57BL/6 mice.

**Red flags and open questions**

1. The intervention is a transgene plus a research dimeriser (a drug that activates the killing transgene), so genetic clearance is the only clearance method tested in a BubR1 model.

2. In the 2011 paper phenotyping used females, a mixed genetic background and group sizes of 3 to 9 with unpaired t-tests across many comparisons, uncorrected for multiplicity (earlier appraisal). The main text read describes no drug-only control in H/H mice without the transgene; supplementary material was not read.

3. The senescent identity of the killed cells rests on marker panels and staining that was negative in muscle and lens; other p16-positive cells, including some immune cells, would also die.

4. The 2016 paper reports that vehicle-treated C57BL/6 males had shorter lives than the normal range for the strain and suggests injection stress, which can inflate the apparent gain (full text re-read).

5. Two authors are inventors on patents licensed to a senescence-therapeutics company, and one is a co-founder (2016 competing interests statement). Open point: whether an independent group has repeated the lifespan result.

6. The intervention bypasses the BubR1 defect, and chromosome missegregation, the primary lesion, continues.

**Replication.** Both papers come from one network. Research groups with primary data on senescent-cell clearance in BubR1 mice: one.

| Claim | Grade | Reason |
|---|---|---|
| Genetic clearance delays adipose, muscle and eye phenotypes in BubR1 H/H mice | Suggested | One group, small groups, female-only phenotyping |
| Senolytic drugs rescue BubR1-deficient phenotypes | Speculative | No such experiment |

**Use in this report.** Senolytics appear in the appendix, among the alternative approaches.

### 2.4.4 Hanks 2004: BUB1B in MVA

**Claim as widely cited.** Biallelic *BUB1B* variants cause MVA and cancer predisposition (Nat Genet, PMID [15475955](https://pubmed.ncbi.nlm.nih.gov/15475955/); about 445 citing records).

**What was done** (earlier appraisal of the full text). Eight pedigrees; five carried variants on both alleles, each as one missense and one truncating or absent-transcript allele; 384 controls were screened.

**Red flags and open questions**

1. Missense pathogenicity rests on conservation and absence from controls alone (Table 1).
2. In one family the authors cannot assign the effect to L844F or Q921H.
3. The causal chain from aneuploidy to cancer exceeds the data (tumours in two of five families, one genotyped, no karyotype). The paper cites a mouse hypomorph at about 10% BubR1 with no excess cancer.
4. The pattern "null plus missense" has n = 5, and the authors call it possibly chance. The statement that complete loss is lethal is a hypothesis.

**Replication.** Many clinical groups have since reported patients with *BUB1B* variants, which supports the gene–disease link.

| Claim | Grade | Reason |
|---|---|---|
| Biallelic *BUB1B* variants cause MVA | Demonstrated | Many independent clinical reports |
| Missense variants in the kinase region are pathogenic | Suggested | Conservation only in this paper |
| Aneuploidy causes the cancers | Speculative | Two tumours, no karyotype |

**Use in this report.** The genotype of the child (one truncating and one missense variant) matches this pattern. The assumption that the missense variant reduces function derives from this class of evidence, so the report treats its activity as unmeasured.

### 2.4.5 Matsuura 2006: hidden second allele

**Claim as widely cited.** Seven families with premature chromatid separation carry one *BUB1B* variant, and a low-expression allele on the other copy explains the disease (Am J Med Genet A, PMID [16411201](https://pubmed.ncbi.nlm.nih.gov/16411201/); about 136 citing records).

**What was done** (earlier appraisal of the full text). Transfer of chromosome 15 restored BubR1 levels and function at the kinetochore (the chromosome structure where spindle microtubules attach) in cells from two patients. Carrier protein levels were reduced by more than half on blots.

**Red flags and open questions**

1. Chromosome 15 transfer maps the defect to the chromosome, which carries many genes. The *BUB1B*-specific rescue control failed technically, so the paper's only rescue acts at the level of the whole chromosome.

2. The reduction of more than 50% rests on single blots with overlapping ranges that the authors call "large and overlapping".

3. The rescue data come from one or two patient lines.

4. The low-expression haplotype is inferred from carrier protein levels alone. The search for a second allele covered 5 kb upstream, and the informative marker lay 54 kb upstream.

**Replication.** A later report with overlapping authors identified an upstream variant by single-base editing in a colon-cancer cell line (Ochiai 2014, PMID [24344301](https://pubmed.ncbi.nlm.nih.gov/24344301/), full text partial). The papers read report no independent replication of either result.

| Claim | Grade | Reason |
|---|---|---|
| A hidden low-expression allele explains monoallelic disease | Suggested | Indirect, one group |
| An upstream variant is the second allele | Suggested | One group, cell-line editing |

**Use in this report.** The claim bears on patients whose second allele is missing; it is labelled Suggested, and open question 8 in section 2.10 records it.

### 2.4.6 Suijkerbuijk 2010 and 2012: missense mutants

**Claim as widely cited.** Missense variants in the kinase region reduce BubR1 abundance, the kinase domain is dispensable, and BubR1 is a pseudokinase, a kinase-like protein with little or no catalytic activity (Cancer Res, PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/); Dev Cell, PMID [22698286](https://pubmed.ncbi.nlm.nih.gov/22698286/)).

**What was done** (partial full-text appraisal, 2010 text re-read for the figure cited below). Patient cell lines (four missense alleles) and tagged proteins in HeLa and U2OS cells (human cancer cell lines). Mutant levels fell after 5 hours of cycloheximide (which blocks new protein synthesis) or an inhibitor of heat shock protein 90 (HSP90), and the proteasome inhibitor reversed the HSP90 effect (Fig. 3C).

**Red flags and open questions**

1. The misfolding mechanism rests on one representative experiment with 5-hour drug treatments and steady-state protein levels. The paper contains no pulse-chase (a labelling experiment that follows protein half-life), ubiquitination assay or HSP90 binding test.

2. Stability was mostly measured as overexpressed tagged protein in cancer cell lines under a foreign promoter.

3. The claim of nonsense-mediated decay (degradation of messenger RNA that carries a premature stop codon) is indirect: Northern blots in two experiments, and the paper reports no decay-inhibitor rescue.

4. "Kinase domain dispensable" derives from knockdown-and-replace assays in cancer cells over short times; the 2012 paper shows the domain contributes to stability and phosphatase recruitment.

5. Patient lines are virus-transformed, which can alter checkpoint behaviour.

6. In 2012, adenosine triphosphate (ATP) analogue binding left thermal stability unchanged, and nucleotide binding in cells was not shown. The statement that earlier kinase-dependence studies "cannot be interpreted" is the authors' untested inference.

**Replication.** No independent test of the missense stability data was found in the papers read.

| Claim | Grade | Reason |
|---|---|---|
| Kinase-region missense variants lower BubR1 abundance | Suggested | One group; four patient alleles; tagged proteins elsewhere |
| The cause is HSP90-dependent misfolding | Speculative | One blot, no binding or ubiquitination test |
| BubR1 catalytic activity is dispensable | Suggested | Short assays, replacement in cancer cells |

**Use in this report.** These papers support the assumption that the child's missense allele lowers abundance. The [chaperone and proteostasis approaches](appendix/alternative-approaches-assessed/chaperones-and-proteostasis.md) in the appendix inherit the Speculative grade.

### 2.4.7 Choi 2009: acetylation at lysine 250

**Claim as widely cited.** Acetylation of BubR1 at K250 by the acetyltransferase p300/CBP-associated factor (PCAF) protects it from degradation and times mitotic exit (EMBO J, PMID [19407811](https://pubmed.ncbi.nlm.nih.gov/19407811/); about 113 citing records).

**What was done** (open-access full text re-read). HeLa cells, mass spectrometry, acetyl-specific antibody, K250Q (acetyl-mimic) and K250R (acetylation-deficient) mutants. K250Q was stabilised and delayed mitosis; K250R was unstable and accelerated mitosis.

**Red flags and open questions**

1. Nearly all data come from HeLa cells with transient or adenoviral overexpression. The fraction of endogenous BubR1 acetylated was not quantified.

2. K250Q is an assumed acetyl-mimic, and K250 has also been reported as a sumoylation site (Yang 2012, PMID [22167194](https://pubmed.ncbi.nlm.nih.gov/22167194/), abstract only; the paper carries a correction notice, section 2.4.19), so the mutants change both modifications.

3. Live-cell curves are described as representative, and one panel has two experiments.

4. Degradation signals in BubR1 also contribute to checkpoint function, so the degradation and checkpoint effects overlap there. Ubiquitination of BubR1 by the anaphase-promoting complex/cyclosome (APC/C) was not reproduced in vitro.

5. Cdc20 binding is unchanged by acetylation (Fig. 5E, F), so the way acetylation blocks degradation remains a conformational model (Fig. 8F).

6. The deacetylase was not identified; the sign conflicts with K668 (section 2.4.1). Open point: whether one cell system can measure K250 and K668 acetylation together and report the net effect on BubR1 half-life.

**Replication.** A knock-in mouse study with overlapping authors tested loss of acetylation (PMID [23878276](https://pubmed.ncbi.nlm.nih.gov/23878276/), earlier appraisal). No independent group was found in the papers read.

| Claim | Grade | Reason |
|---|---|---|
| K250 acetylation stabilises BubR1 in HeLa cells | Suggested | One group, overexpression, mimic mutants |
| Acetylation is the switch that times APC/C activation | Speculative | Mechanism of protection is a model |

**Use in this report.** The sign conflict with K668 is the reason the NAD+ card lists the net effect of raising NAD+ as unresolved.

### 2.4.8 Baker 2008: p16 loss in BubR1 mice

**Claim as widely cited.** Loss of p16Ink4a attenuates senescence and premature ageing in BubR1 hypomorph mice, and loss of p19Arf worsens them, so p16Ink4a is "an effector" of ageing (Nat Cell Biol, PMID [18516091](https://pubmed.ncbi.nlm.nih.gov/18516091/); about 318 citing records).

**What was done** (earlier appraisal of the full text and supplementary material; the paper was not reopened for this report). Cohorts of H/H (n = 192), H/H with p16 loss (n = 86), wild type (n = 160) and p16 null (n = 44) followed for one year; median survival rose 25% (log-rank P = 0.0142) and maximum lifespan was unchanged. Tissue panels used 3 to 4 males per genotype.

**Red flags and open questions**

1. Some P values cannot come from rank tests with 3 or 4 animals per group (fibre size, n = 3, P < 0.0001; adipose thickness, n = 4). The legends indicate pooling across fibres or sections, which makes the fibre or section the apparent unit of analysis (earlier appraisal). Open point: the results with the animal as the unit.

2. All tissue panels used males, so female tissue data are absent, and survival cohorts mixed sexes and are reported pooled.

3. The mice carry lifelong whole-body null alleles on a mixed 129 x C57BL/6 background. The paper describes no littermate matching.

4. "Effector" rests on the correlation of lower senescence markers with milder phenotypes. The p53 phenocopy that supports the "p19Arf protects" model is cited as unpublished in the Discussion.

5. The cost was lung adenocarcinoma in 9% of the compound mutants (8 of 9 tumours), against under 1% in H/H. Cataract onset was delayed modestly, and dwarfism, dermal thickness, arterial stiffening and infertility were unchanged.

6. The compound mutants were not assayed for aneuploidy or BubR1 protein, so the primary lesion remains unexamined.

**Replication.** Later work from the same network used the same crosses and a transgene-based clearance model (Baker 2011, PMID [22048312](https://pubmed.ncbi.nlm.nih.gov/22048312/)). Research groups with primary data on p16 loss in BubR1 mice: one.

| Claim | Grade | Reason |
|---|---|---|
| p16 loss delays muscle, fat and eye phenotypes and raises median survival of H/H mice | Suggested | One group, mixed-sex survival cohorts, small tissue panels with unclear unit of analysis |
| p16 is an effector of BubR1-driven ageing | Speculative | Correlation of markers with phenotype, no isolated mechanism |

**Use in this report.** No candidate in sections 3 or 4 cites the paper. Its subject, p16-positive cells, is the target of the [senolytic approaches](appendix/alternative-approaches-assessed/senolytics.md) in the appendix.

### 2.4.9 Baker 2013: BubR1 overexpression

**Claim as widely cited.** Sustained high BubR1 protects against aneuploidy and cancer and extends healthy lifespan, and modulating BubR1 offers "a unique opportunity to extend healthy lifespan" (Nat Cell Biol, PMID [23242215](https://pubmed.ncbi.nlm.nih.gov/23242215/); about 208 citing records).

**What was done** (author manuscript re-read; figure panels and group sizes shown only in figures were not extracted).

- Two Flag-BubR1 transgenic lines, T7 (moderate) and T23 (high), with a green fluorescent protein (GFP)-only transgenic control (T-GFP).

- Skin and lung tumours induced by 7,12-dimethylbenz[a]anthracene (DMBA): 33% of T23 mice developed tumours, against 100% of wild type.

- KrasLA1 lung tumours at 6 weeks: 8 against 17 on average.

- Survival curves with mixed sexes; maximum lifespan by one-sided Wang-Allison test (P = 0.05 against wild type and P = 0.0056 against T-GFP).

- Interphase fluorescence in situ hybridisation (FISH) for chromosomes 4 and 7 in 3 and 24-month tissues, n = 3 males per genotype, per tissue, per age (Table 1).

**Red flags and open questions**

1. Only the high-expressing line protected. T7 did not reduce tumours, and the paper attributes this to a threshold. Two lines were studied, so a line-specific effect of the integration site stays open.

2. Maximum lifespan was tested one-sided, and the comparison with wild type sits at P = 0.05 (Fig. 3 legend).

3. Lifespan extension is reported for both sexes, "more profoundly in males", in curves labelled mixed gender. Sex-specific group sizes and medians are in the figures only.

4. The aneuploidy readout covers two chromosomes in three males per group. Bone marrow and small intestine showed no protection, and cataracts and osteoporosis were not delayed.

5. Spontaneous tumours that did arise in T23 mice had low transgene expression, which the authors read as selection against the transgene.

6. The Discussion states "it is tempting to speculate" that BubR1 extends health by attenuating chromosome instability, and the closing paragraph states the effects occur "in the absence of apparent side effects" and calls BubR1 a promising target.

7. The manuscript version read carries no competing-interests statement.

**Replication.** No independent group was found in the papers read. Research groups with primary data on BubR1 overexpression and lifespan: one.

| Claim | Grade | Reason |
|---|---|---|
| High BubR1 reduces carcinogen- and Kras-induced tumours in mice | Suggested | One high line, one group |
| High BubR1 extends median and maximum lifespan | Suggested | One line, mixed sexes, one-sided test for maximum |
| Reduced aneuploidy explains the benefit | Speculative | Stated as "tempting to speculate" |

**Use in this report.** The [lentiviral add-back card](04-non-approved-therapies/lentiviral-add-back.md) and the [residue atlas](appendix/residue-atlas.md) cite the paper as evidence that raising BubR1 above wild type was tolerated in mice. The card keeps the grade Suggested and lists the single-line and threshold findings under evidence against.

### 2.4.10 Dai 2004: BubR1 haploinsufficiency

**Claim as widely cited.** BubR1 heterozygous mice are defective in spindle checkpoint activation and develop lung and intestinal adenocarcinomas after a carcinogen (Cancer Res, PMID [14744753](https://pubmed.ncbi.nlm.nih.gov/14744753/); about 231 citing records).

**What was done** (abstract only; earlier appraisal also abstract only). Heterozygous mouse embryonic fibroblasts showed reduced securin and Cdc20 and more micronuclei (small secondary nuclei formed from chromosomes left behind in mitosis); heterozygous mice "rapidly develop" tumours after carcinogen challenge.

**Red flags and open questions**

1. Group sizes, carcinogen, dose, sex and background are unchecked, so the effect size is unknown.
2. A heterozygous allele plus carcinogen differs from germline biallelic disease. Hanks 2004 (section 2.4.4) cites a hypomorph at about 10% BubR1 without excess cancer.
3. The abstract leaves open whether spontaneous tumours occur in this line.

**Replication.** Not assessed.

| Claim | Grade | Reason |
|---|---|---|
| BubR1 reduction predisposes mice to carcinogen-induced tumours | Suggested (abstract only) | Unchecked group sizes and design |

**Use in this report.** The paper is background for the cancer-direction field of every card; conclusions rest on other sources.

### 2.4.11 Sudakin 2001 and Tang 2001: checkpoint complex

**Claim as widely cited.** BubR1, Bub3, Cdc20 and Mad2 form a mitotic checkpoint complex (MCC) that inhibits the APC/C (J Cell Biol, PMID [11535616](https://pubmed.ncbi.nlm.nih.gov/11535616/); about 710 citing records), and BubR1 inhibits APC-Cdc20 without Mad2 and without its kinase activity (Dev Cell, PMID [11702782](https://pubmed.ncbi.nlm.nih.gov/11702782/); about 331 citing records).

**What was done.** Sudakin (full text re-read): purification of an APC/C inhibitory factor from HeLa cells, near-equal stoichiometry of the four proteins, Mad2 content by quantitative immunoblot, activity "3,000-fold greater than recombinant MAD2", and activity in G1/S-arrested cells. Tang (abstract only): mitotic human cell extracts, Xenopus egg extracts and cells overexpressing Cdc20.

**Red flags and open questions**

1. The biochemistry comes from HeLa cell extracts and in vitro assays.

2. The claims that MCC is "present and active in interphase cells" and "not generated from kinetochores" are proposals ("we propose") from one group. Kulukian 2009 (PMID [19154722](https://pubmed.ncbi.nlm.nih.gov/19154722/), abstract only) reports that unattached kinetochores catalytically generate the inhibitor and that this requires Mad1-bound Mad2. Nilsson 2008 (PMID [18997788](https://pubmed.ncbi.nlm.nih.gov/18997788/), abstract only) reports that most Cdc20 lies outside a complex with Mad2 and that Mad2 is required for the BubR1-Cdc20 complex. Open point: the size of the interphase pool in unperturbed human cells.

3. Tang reports that BubR1 kinase activity is dispensable for APC inhibition. A kinase-dead BubR1 failed to restore the checkpoint in Xenopus extract (Mao 2003, PMID [12859900](https://pubmed.ncbi.nlm.nih.gov/12859900/), section 2.7), and pseudokinase mutants later proved to be destabilised (section 2.4.6), which confounds both readings.

**Replication.** A third group provided structures of the complex (the two papers share their last author, Barford): fission yeast MCC (Chao 2012, PMID [22437499](https://pubmed.ncbi.nlm.nih.gov/22437499/)) and human APC/C-MCC by cryo-electron microscopy (Alfieri 2016, PMID [27509861](https://pubmed.ncbi.nlm.nih.gov/27509861/)), both abstract only. The human structure shows BubR1 degron-like sequences (a degron is a sequence that targets a protein for degradation) blocking degron recognition sites on Cdc20. Three groups with different last authors (Yen, Yu and Barford) support BubR1 in an APC/C-inhibitory complex.

| Claim | Grade | Reason |
|---|---|---|
| BubR1, Bub3, Cdc20 and Mad2 form an APC/C-inhibitory complex | Demonstrated | Biochemistry from two groups plus two structure papers from a third group |
| A preformed interphase pool of MCC | Suggested | One group, HeLa purification, challenged by kinetochore-catalysis data |
| BubR1 kinase activity is dispensable for APC/C inhibition | Suggested | Conflicting extract results |

**Use in this report.** The papers underlie the assumption that lower BubR1 weakens the checkpoint; the cards use that assumption alone.

### 2.4.12 Sayin 2014: antioxidants and lung cancer

**Claim as widely cited.** Dietary N-acetylcysteine (NAC) and vitamin E increase tumour progression and reduce survival in mouse models of lung cancer (Sci Transl Med, PMID [24477002](https://pubmed.ncbi.nlm.nih.gov/24477002/); about 644 citing records).

**What was done** (abstract only). Mouse models of B-RAF- and K-RAS-induced lung cancer fed NAC or vitamin E; RNA sequencing; mouse and human lung tumour cells; p53 inactivation.

**Red flags and open questions**

1. Group sizes, diet doses and the human-equivalent exposure of NAC were not checked, so the NAC card states the finding as an animal result.
2. The effect depended on p53 (inactivating p53 gave a similar increase and removed the antioxidant effect), so it describes tumours with intact p53 and an oncogenic driver. Open point: whether the result applies to a child without an established oncogene-driven lesion.
3. The sentence about smokers and patients with chronic obstructive pulmonary disease is an extrapolation in the abstract.

**Replication.** Not assessed. A human observational study of antioxidant supplements other than NAC (vitamins A, C and E, carotenoids, coenzyme Q10) during chemotherapy in 1,134 patients with breast cancer reported an adjusted hazard ratio for recurrence of 1.41 (95% confidence interval 0.98 to 2.04; P = 0.06) (PMID [31855498](https://pubmed.ncbi.nlm.nih.gov/31855498/); abstract read), as described on the NAC card.

| Claim | Grade | Reason |
|---|---|---|
| Antioxidants accelerate oncogene-driven lung tumours in mice | Suggested (abstract only) | One group, mouse models, unchecked design |
| Antioxidants accelerate early human lesions | Speculative | Extrapolation in the abstract |

**Use in this report.** The NAC card lists the paper under evidence against and notes that the experiments used an oncogene-driven tumour model.

### 2.4.13 Nacarelli 2019: NAD+ and the secretome

**Claim as widely cited.** NAD+ metabolism governs the proinflammatory senescence-associated secretory phenotype (SASP), and "anti-ageing dietary NAD+ augmentation should be administered with precision" (Nat Cell Biol, PMID [30778219](https://pubmed.ncbi.nlm.nih.gov/30778219/); about 368 citing records).

**What was done** (author manuscript re-read). IMR90 human fibroblasts at 2% oxygen with oncogenic RAS-induced senescence; knockdown of HMGA1 or NAMPT, the NAMPT inhibitor FK866 and NMN rescue. Mice: NMN 500 mg/kg intraperitoneally for 13 days in a Kras-driven pancreatic model; ovarian cancer cells grown with senescent fibroblasts; nicotinamide in a xenograft (n = 9 mice per group). Replication statement: "representative of a minimum of three independent experiments", and some panels use two biological replicates.

**Red flags and open questions**

1. The mechanism rests on one fibroblast line with one senescence trigger. The extension to dietary supplements is the authors' inference.

2. The mouse NMN experiment lasted 13 days at 500 mg/kg, the dose also used in North 2014, in a Kras-driven model with premalignant lesions. The pancreas experiment used 10 mice per group unless the figure legend states otherwise.

3. NMN in the pancreas increased desmoplasia (fibrous tissue build-up) and IL1B, IL6 and IL8 expression and decreased normal acinar area. The paper reads this as tumour-promoting inflammation. Open point: whether the same dose raises cytokines in tissues without an oncogenic lesion.

4. The authors declare no competing interests.

**Replication.** No independent test of the HMGA-NAMPT-SASP axis was found in the papers read.

| Claim | Grade | Reason |
|---|---|---|
| NAMPT-NAD+ activity supports the proinflammatory SASP in RAS-senescent fibroblasts | Suggested | One group, one line |
| NMN supplementation promotes inflammation and lesions in a Kras pancreatic model | Suggested | One model, short exposure, 10 mice per group |
| Dietary NAD+ supplements are tumour-promoting in people | Speculative | Inference |

**Use in this report.** The NAD+ precursor card and the anakinra card list the paper under evidence against.

### 2.4.14 Santaguida 2017 and Wang 2021: immune clearance

**Claim as widely cited.** Cells with complex karyotypes after chromosome missegregation arrest, show senescence features, produce inflammatory signals and are cleared by the immune system (Dev Cell, PMID [28633018](https://pubmed.ncbi.nlm.nih.gov/28633018/); about 338 citing records), and the clearance by natural killer (NK) cells depends on nuclear factor kappa B (NF-kB) signalling (EMBO Rep, PMID [34105235](https://pubmed.ncbi.nlm.nih.gov/34105235/); about 66 citing records).

**What was done** (both full texts re-read). Untransformed human RPE-1 hTERT cells (a telomerase-immortalised retinal pigment epithelial line) released from a G1/S block into inhibitors of the kinase MPS1 (monopolar spindle 1), reversine or NMS-P715; live-cell imaging; co-culture with the immortalised NK line NK-92 (NK-92MI in Wang 2021) at 2.5 to 1 and 5 to 1 ratios for 36 hours; knockdown or inhibition of NF-kB. Most panels used 3 biological replicates and some used 2.

**Red flags and open questions**

1. The aneuploidy is induced by drugs that abolish the checkpoint and give high error rates, far above the rate in a BubR1 hypomorph, so the dose of missegregation differs by orders of magnitude from the case here.

2. Most data come from one human cell line, and the NK cells are an immortalised line that produces interleukin-2 (IL-2). These papers report no primary NK cells and no clearance of aneuploid cells in an animal or a person.

3. Santaguida 2017 states that chromosome missegregation "rarely" activates p53 and that the arrested cells carry abnormal karyotypes, so the clearance model applies to a minority subset of cells.

4. Wang 2021 reports that NF-kB upregulation in cancer lines correlates with aneuploidy but does not trigger NK clearance, so the clearance does not hold in transformed cells.

5. The two papers share a research network (Santaguida and Amon are authors on both).

**Replication.** No independent group was found in the papers read. Research groups: one network.

| Claim | Grade | Reason |
|---|---|---|
| NK-92MI cells kill drug-induced complex-karyotype RPE-1 cells in vitro through NF-kB | Suggested | One cell line, one NK line, one network |
| Aneuploid cells are cleared by immune cells in human tissue | Speculative | Proposed in the abstract, no in vivo data in these papers |

**Use in this report.** The anakinra card lists possible loss of NK-mediated clearance under evidence against and grades it Speculative.

### 2.4.15 Sullivan 2016 and Li 2023: interferon signalling

**Claim as widely cited.** Trisomy 21 consistently activates the interferon response, and Janus kinase (JAK) inhibition rescues trisomy 21 fibroblast proliferation (eLife, PMID [27472900](https://pubmed.ncbi.nlm.nih.gov/27472900/); about 315 citing records). Chromosomal instability (CIN) drives metastasis through chronic activation of the cGAS-STING pathway (cyclic GMP-AMP synthase and stimulator of interferon genes, a DNA-sensing innate-immune route) (Nature, PMID [37612508](https://pubmed.ncbi.nlm.nih.gov/37612508/); about 329 citing records).

**What was done** (both full texts re-read). Sullivan: RNA sequencing of 12 age- and sex-matched fibroblast lines, 6 lymphoblastoid lines and primary cells from 10 trisomy 21 and 7 control individuals; a kinome shRNA screen (3,075 shRNAs against 654 kinases) in 12 fibroblast lines; ruxolitinib in two control and trisomy pairs. Li: four syngeneic mouse cancer models; for 4T1 tumours n = 19 and 23 animals in immune-competent hosts and n = 10 per condition in other experiments; cGAS or STING knockout and STING inhibitors.

**Red flags and open questions**

1. Trisomy 21 is a constitutional (present in every cell) extra copy of one chromosome that carries four interferon receptor genes. The authors state the activation "could merely be a result of increased gene dosage" of those receptors, so the mechanism may not transfer to random mosaic aneuploidy.

2. The JAK result comes from two fibroblast pairs. The authors note that dose-limiting toxicities of ruxolitinib are anaemia and thrombocytopenia and that a therapeutic window needs "rigorous clinical investigations".

3. Li 2023 studies cancer cell lines with experimentally altered CIN and measures metastasis. Germline mosaic aneuploidy in normal tissue and the interferon outcome there fall outside its scope.

4. Li 2023 competing interests: the senior author holds a patent related to targeting CIN and the cGAS-STING pathway, and has equity in, receives compensation from and sits on the scientific advisory board and board of directors of Volastra Therapeutics (competing-interests statement).

**Replication.** Not assessed beyond the papers read. Sullivan lists one reviewing-editor role as a competing interest.

| Claim | Grade | Reason |
|---|---|---|
| Trisomy 21 cells carry an interferon transcriptional signature | Suggested | One group, several cell types and individuals, no independent test in the papers read |
| JAK inhibition rescues trisomy 21 fibroblast proliferation | Suggested | Two cell pairs |
| An interferon signature exists in MVA cells | Speculative | No such measurement in these papers |
| STING activation by CIN drives metastasis | Suggested | Mouse cancer models, one group, disclosed commercial interests |

**Use in this report.** The appendix assessment of [interferon blockade](appendix/alternative-approaches-assessed/interferon-and-jak-blockade.md) treats the MVA signature as unmeasured.

### 2.4.16 Thompson 2008: baseline error rate

**Claim as widely cited.** Chromosome missegregation in chromosomally stable human cells is rare and rises when merotely (attachment of one kinetochore to microtubules from both spindle poles) is increased, and aneuploid tumour cells with CIN missegregate chromosomes at high rates (J Cell Biol, PMID [18283116](https://pubmed.ncbi.nlm.nih.gov/18283116/); about 453 citing records).

**What was done** (full text re-read). Live-cell imaging and clonal analysis in two stable lines (HCT116 and RPE-1) and three CIN lines (HT29, MCF-7, Caco2). Interphase FISH with centromere probes for four chromosomes. Lagging chromatids in video: 24% of HT29 cells (n = 34), 75% of Caco2 (n = 28), 42% of MCF-7 (n = 33).

**Red flags and open questions**

1. The basal rate of about 0.025% per chromosome (one chromosome per 100 divisions) comes from two lines and four probed chromosomes. The paper notes that chromosomes in micronuclei are missed in the FISH analysis.
2. Video sample sizes for the CIN lines are 28 to 34 cells.
3. HCT116 is a colon cancer line, and RPE-1 is hTERT-immortalised, so both are cultured lines that differ from a primary diploid cell in a tissue.

**Replication.** The paper cites comparable rates in primary human fibroblasts; independent replication was not assessed here.

| Claim | Grade | Reason |
|---|---|---|
| Stable lines missegregate about 0.025% of chromosomes per division | Suggested | Two lines, four chromosomes |

**Use in this report.** The error-free division estimate in the appendix compares its own baseline with this measured value; the model baseline is 2.5 times higher. The comparison depends on two cell lines.

### 2.4.17 Sotillo 2007 and Ricke 2011: checkpoint overexpression

**Claim as widely cited.** Overexpression of the checkpoint proteins Mad2 (Cancer Cell, PMID [17189715](https://pubmed.ncbi.nlm.nih.gov/17189715/); about 500 citing records) and Bub1 (J Cell Biol, PMID [21646403](https://pubmed.ncbi.nlm.nih.gov/21646403/); about 162 citing records) causes aneuploidy and tumours in mice, so a higher level of a checkpoint protein can carry its own tumour risk.

**What was done.** Sotillo (earlier appraisal of the full text): doxycycline-regulated Mad2 transgene; 40 Tet-Off mice against 15 littermates, with tumours mostly after 12 months; 9 of 18 Tet-On mice on doxycycline developed tumours; Emu-myc lymphoma 100% against 40% (n = 17 and 10). Ricke (full text re-read): Bub1 transgenic mice aged to 12 to 16 months with a significant rise in spontaneous tumours (Fisher's exact test) and faster Myc lymphoma (median survival 13 against 21 weeks).

**Red flags and open questions**

1. Both used ubiquitous, long-term overexpression of a different checkpoint protein, so the findings address overexpression above wild type for a different protein; BubR1 raised from a hypomorphic level to wild type is untested.

2. Sotillo notes that the high Tet-On line causes cell death in culture, so the tumours may reflect selection for tolerated levels.

3. Ricke shows that BubR1 overexpression corrects the segregation errors caused by Bub1 overexpression in cells, as stated in the text.

4. Both papers come from mouse models on mixed backgrounds; Ricke is from the same research network as the BubR1 transgenic papers.

**Replication.** Independent confirmation of each was not assessed here. Together, the two papers and Baker 2013 (section 2.4.9) show that the outcome of raising a checkpoint protein depends on the protein and on the level.

| Claim | Grade | Reason |
|---|---|---|
| Mad2 or Bub1 overexpression causes aneuploidy and tumours in mice | Suggested | Mouse transgenics, one group each |
| Raising BubR1 is safe in a hypomorph | Speculative | No such experiment |

**Use in this report.** The [lentiviral add-back card](04-non-approved-therapies/lentiviral-add-back.md) cites both papers under delivery and exposure and keeps the overshoot risk as a stated hazard.

### 2.4.18 Cohen-Sharir 2021: aneuploidy and checkpoint dependency

**Claim as widely cited.** Aneuploid cancer cells are vulnerable to inhibition of the spindle checkpoint (Nature, PMID [33505028](https://pubmed.ncbi.nlm.nih.gov/33505028/); about 280 citing records).

**What was done** (author manuscript re-read). Aneuploidy scores for 997 cancer cell lines from the Cancer Cell Line Encyclopedia; analysis of loss-of-function screens in 689 and 712 lines (BUB1B and MAD2 at the top of the hit list); a modest reduction of BUB1B and MAD2 messenger RNA and protein in aneuploid lines; validation in isogenic (otherwise genetically identical) aneuploid derivatives of HCT116 and RPE-1; inhibitors of the kinase TTK (also called MPS1), including reversine.

**Red flags and open questions**

1. The dependency is a correlation across cell lines. The authors note that the aneuploidy score tracks tissue type, proliferation rate, CIN, whole-genome doubling and p53 function, and they test lineage, proliferation and other covariates.

2. In the isogenic aneuploid derivatives the lines with high aneuploidy were more resistant to knockdown of BUB1B, MAD2 and TTK and to TTK inhibitors over 5 days, which runs opposite to the cell-line correlation. The paper resolves this with time-dependent sensitivity.

3. The abstract states a "synthetic lethal interaction between aneuploidy and the SAC", the spindle assembly checkpoint. Synthetic lethal means that two perturbations together kill cells that tolerate either alone. The evidence consists of correlations, short drug exposures and a kinesin (KIF18A) mechanism, and the text read reports no in vivo test.

4. Competing interests include consultancies and company foundings among the authors.

**Replication.** Not assessed beyond the paper.

| Claim | Grade | Reason |
|---|---|---|
| Aneuploid cancer lines depend more on BUB1B than near-euploid lines | Suggested | Correlation across lines; the isogenic lines resisted knockdown |
| Aneuploid cells are synthetically lethal with SAC weakening | Speculative | Interpretation of time-dependent data |

**Use in this report.** The appendix on mitotic inhibitors cites the paper. The interpretation for MVA is limited, since cells in MVA carry a constitutive checkpoint hypomorph and the experiments here used cancer lines.

### 2.4.19 Retraction and correction check

We queried Europe PMC by title for retraction, retracted-publication, erratum and expression-of-concern notices on the papers appraised in this section. Author-level queries (retraction and expression-of-concern types) covered five authors of the BubR1 and SIRT2 papers. These queries found no retraction and no expression of concern. A second check on 2026-10-24 read the publication-type and comment-and-correction fields of the Europe PMC records of all 52 papers in the References and found no retraction and no expression of concern.

The second check found three corrections. Baker 2008 (PMID [18516091](https://pubmed.ncbi.nlm.nih.gov/18516091/)) carries an erratum (Nat Cell Biol 2012;14(6):649) that the PubMed record describes as an author-name correction (Pitel, Kevin to Pitel, Kevin S). The erratum itself was not read.

Yang 2012 (PMID [22167194](https://pubmed.ncbi.nlm.nih.gov/22167194/)), cited in section 2.4.7 for sumoylation at K250, carries an Additions and Corrections notice (J Biol Chem 2016;291(1):426-7, PMID [26724313](https://pubmed.ncbi.nlm.nih.gov/26724313/)). The notice was not read, and the sumoylation statement rests on the abstract.

Sieben 2020, "BubR1 allelic effects drive phenotypic heterogeneity in mosaic-variegated aneuploidy progeria syndrome" (PMID [31738183](https://pubmed.ncbi.nlm.nih.gov/31738183/)), has a corrigendum (J Clin Invest 2020;130(11):6188, PMID [33136097](https://pubmed.ncbi.nlm.nih.gov/33136097/), DOI [10.1172/JCI144781](https://doi.org/10.1172/JCI144781)). The content of the corrigendum was not read. The report cites the paper for raised mechanistic target of rapamycin complex 1 (mTORC1) signalling in monoallelic mouse muscle, in the [mTOR and autophagy appendix section](appendix/alternative-approaches-assessed/mtor-and-autophagy.md), and that statement stays unconfirmed until the corrigendum is read.

The check covers Europe PMC publication-type tags and correction links only; PubPeer and Retraction Watch were not searched.

## 2.5 Claims that outrun the data

The table sets each claim in circulation beside what the cited data show, with the source and its read basis.

| Claim in circulation | What the data show | Source |
|---|---|---|
| NAD+ precursors raise BubR1 and extend life in BubR1-deficient animals | A transgene extended median life by 58% across both sexes (P = 0.0384) with a male-only subgroup; the drug was tested in 3 mice for 7 days in one tissue | PMID [24825348](https://pubmed.ncbi.nlm.nih.gov/24825348/), full text re-read |
| SIRT2 protects against BubR1-driven ageing | Overexpression left lifespan unchanged in wild-type mice, reported by authors overlapping with the 2014 paper; the hypomorph result has no independent test | PMID [38009412](https://pubmed.ncbi.nlm.nih.gov/38009412/), full text re-read |
| BubR1 decline drives normal ageing | Association in unquantified blots; BubR1 in old tissue stays far above the hypomorph level | PMID [15208629](https://pubmed.ncbi.nlm.nih.gov/15208629/), earlier appraisal |
| Senolytics rescue BubR1 progeria | Genetic clearance with a research dimeriser delayed three tissue phenotypes; heart and aorta were not rescued and survival was not extended; the BubR1 model was tested with genetic clearance alone | PMID [22048312](https://pubmed.ncbi.nlm.nih.gov/22048312/), abstract and earlier appraisal |
| Kinase activity of BubR1 is a drug target | Human BubR1 shows no detectable phosphotransfer in vitro, and catalytic-aspartate mutants are stable and functional | PMID [22698286](https://pubmed.ncbi.nlm.nih.gov/22698286/), partial full text |
| Missense variants misfold and depend on HSP90 | One representative blot with 5-hour treatments in overexpressing cells | PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/), full text re-read for Fig. 3C |
| A hidden low-expression allele explains monoallelic PCS | Chromosome 15 transfer corrected the defect; *BUB1B* complementary DNA failed to correct it; one group | PMID [16411201](https://pubmed.ncbi.nlm.nih.gov/16411201/), earlier appraisal |
| The hypomorph mouse models MVA | The mouse has about 11% BubR1 in every tissue from conception; patients are mosaic and biallelic | PMID [15208629](https://pubmed.ncbi.nlm.nih.gov/15208629/), earlier appraisal |
| BubR1 overexpression extends healthy lifespan | One high-expressing line of two protected; mixed sexes; maximum lifespan by a one-sided test at P = 0.05 against wild type; the mechanism is described as "tempting to speculate" | PMID [23242215](https://pubmed.ncbi.nlm.nih.gov/23242215/), full text re-read |
| NAD+ boosting is a safe anti-ageing strategy | NMN at 500 mg/kg/day for 13 days increased pancreatic lesions, desmoplasia and IL1B, IL6 and IL8 in a Kras-driven mouse model | PMID [30778219](https://pubmed.ncbi.nlm.nih.gov/30778219/), full text re-read |
| The immune system clears aneuploid cells | Drug-induced complex karyotypes in one human cell line, killed by an immortalised NK line in vitro; no in vivo clearance in these papers | PMIDs [28633018](https://pubmed.ncbi.nlm.nih.gov/28633018/) and [34105235](https://pubmed.ncbi.nlm.nih.gov/34105235/), full text re-read |
| Interferon activation is a general consequence of aneuploidy | Trisomy 21 carries four interferon receptor genes on the extra chromosome; the authors state the signature could result from gene dosage; JAK rescue tested in two cell pairs | PMID [27472900](https://pubmed.ncbi.nlm.nih.gov/27472900/), full text re-read |
| Aneuploid cells depend on the checkpoint | Correlation across cancer lines; isogenic aneuploid derivatives resisted BUB1B knockdown over 5 days | PMID [33505028](https://pubmed.ncbi.nlm.nih.gov/33505028/), full text re-read |
| More of a checkpoint protein is protective | Mad2 and Bub1 overexpression caused tumours in mice; the benefit of BubR1 overexpression came from one of two lines | PMIDs [17189715](https://pubmed.ncbi.nlm.nih.gov/17189715/), [21646403](https://pubmed.ncbi.nlm.nih.gov/21646403/), [23242215](https://pubmed.ncbi.nlm.nih.gov/23242215/) |

## 2.6 Findings checked in full text

Each finding below was checked in the full text of the cited paper (in the earlier appraisal where section 2.4 says so), except where the row states otherwise. The last column gives the main caveat.

| Finding | Location | Source | Main caveat |
|---|---|---|---|
| Hypomorph homozygotes keep about 11% of wild-type BubR1, live to adulthood and die at a median of about 6 months with ageing-like features; genotypes with 29% to 42% show none of these. Several readouts rest on groups of 3 to 10 animals | main text, Table 1 and Fig. 1 | Baker 2004, PMID [15208629](https://pubmed.ncbi.nlm.nih.gov/15208629/) | One group; several readouts use 3 to 10 animals; 11% residual BubR1 in every tissue from conception |
| Five of eight MVA pedigrees carry variants on both *BUB1B* alleles, each as one missense and one truncating or absent-transcript allele; five of six missense variants lie in the kinase domain; two of the five families included a patient with embryonal rhabdomyosarcoma (a muscle tumour); three pedigrees were negative. Missense pathogenicity rests on conservation and absence from controls alone | main text and Table 1 | Hanks 2004, PMID [15475955](https://pubmed.ncbi.nlm.nih.gov/15475955/) | Missense pathogenicity inferred from conservation; five biallelic cases |
| One man homozygous for a deep intronic splice-gain variant has adult-onset gastrointestinal cancers; most transcripts are lost to decay and a small amount of normal BubR1 remains (about 10 to 15 percent of control, inferred from an end-point gel ratio). Restoring BubR1 lowered premature chromatid separation. One patient; the link to the cancers is by exclusion of other genes | main text and rescue figures | Rio Frio 2010, PMID [21190457](https://pubmed.ncbi.nlm.nih.gov/21190457/) | One patient; the residual level is inferred from an end-point gel ratio |
| Seven Japanese families with premature chromatid separation carry one *BUB1B* variant each and no second coding variant; transfer of chromosome 15 restored BubR1 levels and kinetochore function in two patients' cells. A low-expression haplotype is proposed as the hidden second allele, inferred from carrier protein levels on unreplicated blots | abstract and earlier appraisal of the full text [UNVERIFIED: full text not re-read for this report] | Matsuura 2006, PMID [16411201](https://pubmed.ncbi.nlm.nih.gov/16411201/) | Chromosome transfer maps the defect to chromosome 15, which carries many genes; unreplicated blots |
| Premature chromatid separation rises as BubR1 falls; residual levels were 8.5, 10, 14, 58 and 77 percent, so the series stops at 14 percent and resumes at 58 percent. The scored "aneuploidy" is DNA content above 4N after prolonged nocodazole, a measure of checkpoint failure that leaves chromosome gains and losses uncounted | dose-response table | Bohers 2008, PMID [18932004](https://pubmed.ncbi.nlm.nih.gov/18932004/) | Five stable HeLa lines; aneuploidy is a DNA-content proxy |
| Targeting the phosphatase subunit B56 to the outer kinetochore with a fusion protein restored chromosome alignment in two patient fibroblast lines (transient expression, alignment under proteasome inhibition); a BubR1 mutant that cannot bind B56 failed to rescue | rescue figures (Fig. 4B) | Xu 2013, PMID [23789096](https://pubmed.ncbi.nlm.nih.gov/23789096/) | Transient overexpression in two patient lines |
| Mutations in the pseudokinase domain (K795A, K795R, D911N, V793R) destabilise BubR1, while D882N and D882A are stable | main text | Suijkerbuijk 2012, PMID [22698286](https://pubmed.ncbi.nlm.nih.gov/22698286/) | Overexpressed tagged proteins in cancer cells; nucleotide binding in cells not shown |
| Germline p16 loss extended median survival of hypomorph mice by 25 percent (maximum unchanged) and delayed muscle, fat and eye phenotypes; lung adenocarcinomas appeared; dwarfism, dermal thickness, arterial stiffening and infertility were unchanged. Several muscle and fat panels use 3 to 4 males per genotype | survival curves and supplementary table | Baker 2008, PMID [18516091](https://pubmed.ncbi.nlm.nih.gov/18516091/) | One group; groups of 3 to 4 males in several panels; lung tumours increased |

## 2.7 Findings narrower than their abstracts

The table gives, for each claim in circulation, the full-text result, where the result sits in the paper and the source.

| Claim in circulation | Full-text result | Location | Source |
|---|---|---|---|
| NMN or NAD+ raises BubR1 and doubles lifespan | The lifespan gain came from a SIRT2 transgene. It was male-driven (males +123%, P = 0.004, n = 16 and 17; females no effect, P = 0.79) and the sex split is a post hoc subgroup. The median gain across both sexes was +58% (P = 0.038, n = 31 and 33; maximum +21%). BubR1 stayed below wild type, and the small size, spinal curvature and cataracts persisted. NMN (500 mg/kg/day intraperitoneally for 7 days) was given to aged wild-type mice, n = 3 per group, and BubR1 could be read in one tissue (testis); the only lifespan test used the transgene. Nicotinamide at 20 mM, the paper's own sirtuin-dependence test, lowered BubR1. The senior author discloses consulting and patent interests in NAD+ and sirtuin companies | survival, Western blot and NMN figures; main text, legends and methods read, supplementary figures not opened | North 2014, PMID [24825348](https://pubmed.ncbi.nlm.nih.gov/24825348/) |
| SIRT2 extends life | Lifespan unchanged in wild-type mice (males 869 against 862 days; females 723 against 722 days); BubR1 was not measured in that cohort | survival curves | PMID [38009412](https://pubmed.ncbi.nlm.nih.gov/38009412/) |
| Acetylation stabilises BubR1 | The sign depends on the site. K250 acetylation was reported to protect BubR1 during mitosis (Choi 2009, PMID [19407811](https://pubmed.ncbi.nlm.nih.gov/19407811/), full text; reinforced by a BRCA2-dependent acetylation in Choi 2012, PMID [22340495](https://pubmed.ncbi.nlm.nih.gov/22340495/), abstract only), and SIRT2 knockdown raised K250 acetylation while total BubR1 stayed unchanged (Suematsu 2014, PMID [25285631](https://pubmed.ncbi.nlm.nih.gov/25285631/)). K668 acetylation marks it for degradation (overexpression and acetyl-mimics in one laboratory; PMID [24825348](https://pubmed.ncbi.nlm.nih.gov/24825348/)) | as cited | Choi 2009, PMID [19407811](https://pubmed.ncbi.nlm.nih.gov/19407811/); Choi 2012, PMID [22340495](https://pubmed.ncbi.nlm.nih.gov/22340495/); Suematsu 2014, PMID [25285631](https://pubmed.ncbi.nlm.nih.gov/25285631/); North 2014, PMID [24825348](https://pubmed.ncbi.nlm.nih.gov/24825348/) (full text for 19407811, 25285631 and 24825348; abstract for 22340495) |
| HSP90 inhibitors are contraindicated | One experiment of about 5 hours on two alleles as tagged protein in U2OS cells, one representative blot | Fig 3C | Suijkerbuijk 2010, PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/) |
| BubR1 kinase activity is a druggable checkpoint step | Human BubR1 showed no detectable phosphotransfer in vitro, and catalytic-aspartate mutants (D882N, D882A) were stable and functional, while mutants of residues that contact ATP (K795, D911, V793) lowered protein level (PMID [22698286](https://pubmed.ncbi.nlm.nih.gov/22698286/)). In Xenopus extract, kinase-dead BubR1 restored the checkpoint only when total BubR1 was near normal with some kinase-competent copies (PMID [12859900](https://pubmed.ncbi.nlm.nih.gov/12859900/)), and kinase-dead lysine-to-arginine mutants are later shown to be destabilised, which confounds that result | Figs 2 to 3 of 22698286; Fig 4D of 12859900 | Suijkerbuijk 2012, PMID [22698286](https://pubmed.ncbi.nlm.nih.gov/22698286/) (partial full text); Mao 2003, PMID [12859900](https://pubmed.ncbi.nlm.nih.gov/12859900/) (full text) |
| Senolytics, mTOR inhibitors or JAK inhibitors rescue the progeroid phenotype | Only genetic clearance of p16-positive cells (a transgene activated by a drug) has been tested in a BubR1 model; life-long clearance delayed the onset of pathologies in fat, muscle and eye, and earlier appraisal of the full text records no benefit for heart, arteries or survival | abstract; earlier appraisal of the full text | Baker 2011, PMID [22048312](https://pubmed.ncbi.nlm.nih.gov/22048312/) |
| Compounds bind BubR1 (inhibitor papers) | Each rests on a single pull-down or an abstract. One 2025 paper designed analogues by docking into the *Bub1* kinase domain structure labelled BUB1B (Protein Data Bank entry 6F7B) and measured thermal-shift binding and an enzymatic half-maximal inhibitory concentration (IC50) of about 10 micromolar. Human BubR1 shows no detectable phosphotransfer in vitro, and the paper's reference BUB1 inhibitor was inactive, so the activity assay has no working positive control for BubR1 catalysis | methods, docking and enzymatic sections | El Hafi 2025, PMID [39818011](https://pubmed.ncbi.nlm.nih.gov/39818011/) |
| Many "BUB1B prognostic hub gene" papers | Of about 265 core cancer-expression records, 71 are computational only, and 46 of those mention no wet-laboratory work | corpus count | Count from the literature corpus of this project [UNVERIFIED: corpus table not published with this report] |

## 2.8 Clinical and preclinical data

- **Registered trials.** ClinicalTrials.gov (API version 2, searched 2026-10-17) returns 0 studies for *BUB1B*, MVA or PCS in any of 48 cells (3 conditions by 16 term groups, including an unfiltered row). Cell precision is low, since free-text matching returns unrelated oncology studies.

- **Positive controls.** Three controls passed: Fanconi anaemia 152 studies, Fanconi anaemia with eltrombopag 2, Li-Fraumeni syndrome with magnetic resonance imaging 10.

- **Nearest registered designs.** Fanconi anaemia (152 studies) and ataxia telangiectasia (60).

- **Cancer spectrum.** The American Association for Cancer Research consensus (PMID [39264246](https://pubmed.ncbi.nlm.nih.gov/39264246/)) names the main cancers in MVA1; [section 1.1](01-disease-and-case.md#11-mosaic-variegated-aneuploidy-and-bub1b) lists them.

- **Treatment.** No study reports a drug that raised BubR1 in a *BUB1B*-variant line. The direct rescues in patient cells are re-expression of the wild-type gene, the B56 tether and chromosome 15 transfer. Mouse studies cover genetic clearance of p16-positive cells, germline p16 loss and a SIRT2 transgene.

- **Case-report outcomes.** Management evidence exists for haematological malignancy, tumour treatment and chemotherapy intolerance only, from case reports without denominators [UNVERIFIED: the case reports behind this statement are not recorded].

## 2.9 Papers without accessible full text

Three relevant papers stayed behind paywalls after every legal route (open-access indexes, preprint servers, institutional repositories and an institutional subscription).

| Paper | Identifier | Read basis |
|---|---|---|
| Pham 2026, *Bioorg Chem*: a griseofulvin-derived compound and the spindle checkpoint | DOI [10.1016/j.bioorg.2026.110130](https://doi.org/10.1016/j.bioorg.2026.110130), PMID [42330849](https://pubmed.ncbi.nlm.nih.gov/42330849/) | abstract only |
| Martinez 2026, *Cancer Res*: BUB1B kinase dependency and CENP-E inhibition | DOI [10.1158/0008-5472.can-26-0874](https://doi.org/10.1158/0008-5472.can-26-0874), PMID [42757823](https://pubmed.ncbi.nlm.nih.gov/42757823/) | abstract only |
| Malumbres and Villarroya-Beltri 2024, *Nat Rev Genet*: MVA in development, ageing and cancer | DOI [10.1038/s41576-024-00762-6](https://doi.org/10.1038/s41576-024-00762-6), PMID [39169218](https://pubmed.ncbi.nlm.nih.gov/39169218/) | abstract only |

The conclusions in this report cite sources other than these three papers. Where a public proposal relies on one, the claim is listed as unchecked.

- Of the first 228 papers reviewed in depth, 64 were readable as abstracts only and were retried through every legal route (one opened) [UNVERIFIED: project corpus count].
- A separate set of 27 abstract-only papers was later obtained by hand and re-reviewed [UNVERIFIED: project corpus count].
- Supplementary files and figure images were read only where a section states it.
- Language-model agents produced the reviews under a written protocol. An independent verification pass covered the syntheses by theme; the 27 re-reviews await it.

## 2.10 Open mechanistic questions

1. **Protein abundance and activity of the missense allele.** Both are unmeasured in the papers read. The candidates in sections 3 and 4 depend on both.

2. **Phase of the two variants.** The report assumes the two variants lie in trans (one on each copy of the gene); phasing is unmeasured.

3. **Dose-response between 14 and 58 percent BubR1.** The only human-cell data stop at 14 percent and resume at 58 percent.

4. **Small molecules that raise BubR1 from a patient allele.** None has been reported.

5. **Replication of the SIRT2 and NAD+ effect outside the originating network.** The unchanged lifespan in wild-type mice and the single-siRNA result narrow it, and the papers read contain no independent test of the BubR1 effect.

6. **Sign of the acetylation effect in humans.** K250 and K668 act in opposite directions in separate systems.

7. **PLK1-driven centrosome and cilia phenotype in acute BubR1 loss in diploid cells.** The evidence is one laboratory and truncating alleles.

8. **Contribution of the upstream regulatory variant to the missing second allele.** One laboratory reported it.

9. **Output of the surviving allele after decay of the stop allele.** In zebrafish and mouse, decay of a mutant transcript raised output from related genes, and in zebrafish heterozygotes from the wild-type allele of the same gene (PMID [30944477](https://pubmed.ncbi.nlm.nih.gov/30944477/)). The mechanism runs through the RNA-binding protein ILF3 in mouse and human cells (PMID [41678638](https://pubmed.ncbi.nlm.nih.gov/41678638/)). Passages on the wild-type allele were read in both open-access full texts.

   *BUB1B* is untested. Depletion of UPF1 (a core factor of nonsense-mediated decay) and of ILF3 in the allele-resolved transcript measurement of section 5.10 decides it, and the result sets the dose arithmetic for any route that relieves decay.

10. **Safe upper limit of BubR1.** Mice with about 10 times normal BubR1 developed fewer tumours (PMID [23242215](https://pubmed.ncbi.nlm.nih.gov/23242215/)), and overexpression of Mad2 or Bub1 caused tumours in mice (PMIDs [17189715](https://pubmed.ncbi.nlm.nih.gov/17189715/), [21646403](https://pubmed.ncbi.nlm.nih.gov/21646403/)). No human-cell dose above normal has been tested. A titration of BubR1 above 100% in the platform of section 5.10 gives the limit, and the lentiviral add-back card depends on it.

## References

- Sudakin V et al. (2001). Checkpoint inhibition of the APC/C in HeLa cells is mediated by a complex of BUBR1, BUB3, CDC20, and MAD2. *J Cell Biol*. PMID [11535616](https://pubmed.ncbi.nlm.nih.gov/11535616/)
- Tang Z et al. (2001). Mad2-Independent inhibition of APCCdc20 by the mitotic checkpoint protein BubR1. *Dev Cell*. PMID [11702782](https://pubmed.ncbi.nlm.nih.gov/11702782/)
- Mao Y et al. (2003). Activating and silencing the mitotic checkpoint through CENP-E-dependent activation/inactivation of BubR1. *Cell*. PMID [12859900](https://pubmed.ncbi.nlm.nih.gov/12859900/)
- Dai W et al. (2004). Slippage of mitotic arrest and enhanced tumor development in mice with BubR1 haploinsufficiency. *Cancer Res*. PMID [14744753](https://pubmed.ncbi.nlm.nih.gov/14744753/)
- Baker DJ et al. (2004). BubR1 insufficiency causes early onset of aging-associated phenotypes and infertility in mice. *Nat Genet*. PMID [15208629](https://pubmed.ncbi.nlm.nih.gov/15208629/)
- Hanks S et al. (2004). Constitutional aneuploidy and cancer predisposition caused by biallelic mutations in BUB1B. *Nat Genet*. PMID [15475955](https://pubmed.ncbi.nlm.nih.gov/15475955/)
- Matsuura S et al. (2006). Monoallelic BUB1B mutations and defective mitotic-spindle checkpoint in seven families with premature chromatid separation (PCS) syndrome. *Am J Med Genet A*. PMID [16411201](https://pubmed.ncbi.nlm.nih.gov/16411201/)
- Sotillo R et al. (2007). Mad2 overexpression promotes aneuploidy and tumorigenesis in mice. *Cancer Cell*. PMID [17189715](https://pubmed.ncbi.nlm.nih.gov/17189715/)
- Thompson SL et al. (2008). Examining the link between chromosomal instability and aneuploidy in human cells. *J Cell Biol*. PMID [18283116](https://pubmed.ncbi.nlm.nih.gov/18283116/)
- Baker DJ et al. (2008). Opposing roles for p16Ink4a and p19Arf in senescence and ageing caused by BubR1 insufficiency. *Nat Cell Biol*. PMID [18516091](https://pubmed.ncbi.nlm.nih.gov/18516091/)
- Bohers E et al. (2008). Gradual reduction of BUBR1 protein levels results in premature sister-chromatid separation then in aneuploidy. *Hum Genet*. PMID [18932004](https://pubmed.ncbi.nlm.nih.gov/18932004/)
- Nilsson J et al. (2008). The APC/C maintains the spindle assembly checkpoint by targeting Cdc20 for destruction. *Nat Cell Biol*. PMID [18997788](https://pubmed.ncbi.nlm.nih.gov/18997788/)
- Kulukian A et al. (2009). Unattached kinetochores catalyze production of an anaphase inhibitor that requires a Mad2 template to prime Cdc20 for BubR1 binding. *Dev Cell*. PMID [19154722](https://pubmed.ncbi.nlm.nih.gov/19154722/)
- Choi E et al. (2009). BubR1 acetylation at prometaphase is required for modulating APC/C activity and timing of mitosis. *EMBO J*. PMID [19407811](https://pubmed.ncbi.nlm.nih.gov/19407811/)
- Izumi H et al. (2009). BubR1 localizes to centrosomes and suppresses centrosome amplification via regulating Plk1 activity in interphase cells. *Oncogene*. PMID [19503101](https://pubmed.ncbi.nlm.nih.gov/19503101/)
- Suijkerbuijk SJ et al. (2010). Molecular causes for BUBR1 dysfunction in the human cancer predisposition syndrome mosaic variegated aneuploidy. *Cancer Res*. PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/)
- Rio Frio T et al. (2010). Homozygous BUB1B mutation and susceptibility to gastrointestinal neoplasia. *N Engl J Med*. PMID [21190457](https://pubmed.ncbi.nlm.nih.gov/21190457/)
- Miyamoto T et al. (2011). Insufficiency of BUBR1, a mitotic spindle checkpoint regulator, causes impaired ciliogenesis in vertebrates. *Hum Mol Genet*. PMID [21389084](https://pubmed.ncbi.nlm.nih.gov/21389084/)
- Ricke RM et al. (2011). Bub1 overexpression induces aneuploidy and tumor formation through Aurora B kinase hyperactivation. *J Cell Biol*. PMID [21646403](https://pubmed.ncbi.nlm.nih.gov/21646403/)
- Baker DJ et al. (2011). Clearance of p16Ink4a-positive senescent cells delays ageing-associated disorders. *Nature*. PMID [22048312](https://pubmed.ncbi.nlm.nih.gov/22048312/)
- Choi E et al. (2012). BRCA2 fine-tunes the spindle assembly checkpoint through reinforcement of BubR1 acetylation. *Dev Cell*. PMID [22340495](https://pubmed.ncbi.nlm.nih.gov/22340495/)
- Chao WC et al. (2012). Structure of the mitotic checkpoint complex. *Nature*. PMID [22437499](https://pubmed.ncbi.nlm.nih.gov/22437499/)
- Suijkerbuijk SJ et al. (2012). The vertebrate mitotic checkpoint protein BUBR1 is an unusual pseudokinase. *Dev Cell*. PMID [22698286](https://pubmed.ncbi.nlm.nih.gov/22698286/)
- Yang F et al. (2012). BubR1 is modified by sumoylation during mitotic progression. *J Biol Chem*. PMID [22167194](https://pubmed.ncbi.nlm.nih.gov/22167194/)
- Baker DJ et al. (2013). Increased expression of BubR1 protects against aneuploidy and cancer and extends healthy lifespan. *Nat Cell Biol*. PMID [23242215](https://pubmed.ncbi.nlm.nih.gov/23242215/)
- Xu P et al. (2013). BUBR1 recruits PP2A via the B56 family of targeting subunits to promote chromosome congression. *Biol Open*. PMID [23789096](https://pubmed.ncbi.nlm.nih.gov/23789096/)
- Park I et al. (2013). Loss of BubR1 acetylation causes defects in spindle assembly checkpoint signaling and promotes tumor formation. *J Cell Biol*. PMID [23878276](https://pubmed.ncbi.nlm.nih.gov/23878276/)
- Ochiai H et al. (2014). TALEN-mediated single-base-pair editing identification of an intergenic mutation upstream of BUB1B as causative of PCS (MVA) syndrome. *Proc Natl Acad Sci U S A*. PMID [24344301](https://pubmed.ncbi.nlm.nih.gov/24344301/)
- Sayin VI et al. (2014). Antioxidants accelerate lung cancer progression in mice. *Sci Transl Med*. PMID [24477002](https://pubmed.ncbi.nlm.nih.gov/24477002/)
- North BJ et al. (2014). SIRT2 induces the checkpoint kinase BubR1 to increase lifespan. *EMBO J*. PMID [24825348](https://pubmed.ncbi.nlm.nih.gov/24825348/)
- Suematsu T et al. (2014). Deacetylation of the mitotic checkpoint protein BubR1 at lysine 250 by SIRT2 and subsequent effects on BubR1 degradation during the prometaphase/anaphase transition. *Biochem Biophys Res Commun*. PMID [25285631](https://pubmed.ncbi.nlm.nih.gov/25285631/)
- Miyamoto T et al. (2015). The Microtubule-Depolymerizing Activity of a Mitotic Kinesin Protein KIF2A Drives Primary Cilia Disassembly Coupled with Cell Proliferation. *Cell Rep*. PMID [25660017](https://pubmed.ncbi.nlm.nih.gov/25660017/)
- Baker DJ et al. (2016). Naturally occurring p16(Ink4a)-positive cells shorten healthy lifespan. *Nature*. PMID [26840489](https://pubmed.ncbi.nlm.nih.gov/26840489/)
- Yang F et al. (2016). Additions and Corrections: BubR1 is modified by sumoylation during mitotic progression. *J Biol Chem*. PMID [26724313](https://pubmed.ncbi.nlm.nih.gov/26724313/)
- Pfau SJ et al. (2016). Aneuploidy impairs hematopoietic stem cell fitness and is selected against in regenerating tissues in vivo. *Genes Dev*. PMID [27313317](https://pubmed.ncbi.nlm.nih.gov/27313317/)
- Sullivan KD et al. (2016). Trisomy 21 consistently activates the interferon response. *Elife*. PMID [27472900](https://pubmed.ncbi.nlm.nih.gov/27472900/)
- Alfieri C et al. (2016). Molecular basis of APC/C regulation by the spindle assembly checkpoint. *Nature*. PMID [27509861](https://pubmed.ncbi.nlm.nih.gov/27509861/)
- Santaguida S et al. (2017). Chromosome Mis-segregation Generates Cell-Cycle-Arrested Cells with Complex Karyotypes that Are Eliminated by the Immune System. *Dev Cell*. PMID [28633018](https://pubmed.ncbi.nlm.nih.gov/28633018/)
- Simmons AJ et al. (2019). Nearly complete deletion of BubR1 causes microcephaly through shortened mitosis and massive cell death. *Hum Mol Genet*. PMID [30668728](https://pubmed.ncbi.nlm.nih.gov/30668728/)
- Nacarelli T et al. (2019). NAD+ metabolism governs the proinflammatory senescence-associated secretome. *Nat Cell Biol*. PMID [30778219](https://pubmed.ncbi.nlm.nih.gov/30778219/)
- El-Brolosy MA et al. (2019). Genetic compensation triggered by mutant mRNA degradation. *Nature*. PMID [30944477](https://pubmed.ncbi.nlm.nih.gov/30944477/)
- Sieben CJ et al. (2020). BubR1 allelic effects drive phenotypic heterogeneity in mosaic-variegated aneuploidy progeria syndrome. *J Clin Invest*. PMID [31738183](https://pubmed.ncbi.nlm.nih.gov/31738183/)
- Sieben CJ et al. (2020). Corrigendum to "BubR1 allelic effects drive phenotypic heterogeneity in mosaic-variegated aneuploidy progeria syndrome". *J Clin Invest*. PMID [33136097](https://pubmed.ncbi.nlm.nih.gov/33136097/); DOI [10.1172/JCI144781](https://doi.org/10.1172/JCI144781)
- Ambrosone CB et al. (2020). Dietary Supplement Use During Chemotherapy and Survival Outcomes of Patients With Breast Cancer Enrolled in a Cooperative Group Clinical Trial (SWOG S0221). *J Clin Oncol*. PMID [31855498](https://pubmed.ncbi.nlm.nih.gov/31855498/)
- Cohen-Sharir Y et al. (2021). Aneuploidy renders cancer cells vulnerable to mitotic checkpoint inhibition. *Nature*. PMID [33505028](https://pubmed.ncbi.nlm.nih.gov/33505028/)
- Wang RW et al. (2021). Aneuploid senescent cells activate NF-κB to promote their immune clearance by NK cells. *EMBO Rep*. PMID [34105235](https://pubmed.ncbi.nlm.nih.gov/34105235/)
- Li J et al. (2023). Non-cell-autonomous cancer progression from chromosomal instability. *Nature*. PMID [37612508](https://pubmed.ncbi.nlm.nih.gov/37612508/)
- Wu LE et al. (2023). SIRT2 transgenic over-expression does not impact lifespan in mice. *Aging Cell*. PMID [38009412](https://pubmed.ncbi.nlm.nih.gov/38009412/)
- Malumbres M et al. (2024). Mosaic variegated aneuploidy in development, ageing and cancer. *Nat Rev Genet*. PMID [39169218](https://pubmed.ncbi.nlm.nih.gov/39169218/); DOI [10.1038/s41576-024-00762-6](https://doi.org/10.1038/s41576-024-00762-6)
- Nakano Y et al. (2024). Update on Recommendations for Cancer Screening and Surveillance in Children with Genomic Instability Disorders. *Clin Cancer Res*. PMID [39264246](https://pubmed.ncbi.nlm.nih.gov/39264246/)
- El Hafi M et al. (2025). Synthesis and biological assessment of BUB1B inhibitors for the treatment of clear cell renal cell carcinoma. *Eur J Med Chem*. PMID [39818011](https://pubmed.ncbi.nlm.nih.gov/39818011/)
- El-Brolosy MA et al. (2026). Mechanisms linking cytoplasmic decay of translation-defective mRNA to transcriptional adaptation. *Science*. PMID [41678638](https://pubmed.ncbi.nlm.nih.gov/41678638/)
- Pham HT et al. (2026). Norlichexanthone, a shunt product of Griseofulvin, disrupts spindle assembly checkpoint and nucleocytoplasmic transport by targeting TPR in the nuclear pore complex. *Bioorg Chem*. PMID [42330849](https://pubmed.ncbi.nlm.nih.gov/42330849/); DOI [10.1016/j.bioorg.2026.110130](https://doi.org/10.1016/j.bioorg.2026.110130)
- Martinez MJ et al. (2026). BUB1B Mitotic Kinase Dependency Reveals CENP-E Inhibition as a Tractable Approach for Castration and Enzalutamide Resistant Prostate Cancer. *Cancer Res*. PMID [42757823](https://pubmed.ncbi.nlm.nih.gov/42757823/); DOI [10.1158/0008-5472.can-26-0874](https://doi.org/10.1158/0008-5472.can-26-0874)

## Other sources

- Europe PMC REST API, https://www.ebi.ac.uk/europepmc/webservices/rest/search, `resultType=lite`, cursor pagination, search date 2026-10-24.

  - Gene = `(TITLE_ABS:BUB1B OR TITLE_ABS:BUBR1)`.

  - MVA = `(TITLE_ABS:"mosaic variegated aneuploidy" OR TITLE_ABS:"premature chromatid separation" OR TITLE_ABS:"PCS syndrome")`.

  - Rows: gene; gene AND (mitosis OR mitotic OR checkpoint OR kinetochore); gene AND (cancer OR tumor OR tumour OR carcinoma); gene AND (aging OR ageing OR senescence OR progeroid); MVA; gene AND MVA; gene AND MVA AND (patient, patients, family, families, biallelic, germline, heterozygous, homozygous, proband); gene AND MVA AND (treatment, therapy, therapeutic, drug, inhibitor, rescue); gene AND (treatment, therapy, therapeutic, drug, inhibitor, rescue) AND (hypomorph*, "NAD+", SIRT2, nicotinamide).

- ClinicalTrials.gov API v2 (https://clinicaltrials.gov/data-api/api): census of ten chromosome-instability syndromes (BUB1B, mosaic variegated aneuploidy, premature chromatid separation, Fanconi anaemia, ataxia telangiectasia, Bloom, Nijmegen breakage, Seckel, Li-Fraumeni, constitutional mismatch repair deficiency) by 16 term groups, `query.cond` = syndrome, `query.term` = term group, run 2026-10-17; positive controls Fanconi anaemia 152 studies, Fanconi anaemia with eltrombopag 2, Li-Fraumeni syndrome with magnetic resonance imaging 10.

- EU Clinical Trials Information System (CTIS) and Japan Registry of Clinical Trials (jRCT): condition terms for MVA, BUB1B, BubR1 and premature chromatid separation, searched 2026-10-15, zero registered studies and zero expanded-access records. The Chinese Clinical Trial Registry (ChiCTR) returned HTTP 405 and was not searched.

- Author groups (section 2.2): Europe PMC author strings matched by surname and initials; author identity is unverified.

- Erratum to Baker 2008 (section 2.4.19): Nat Cell Biol 2012;14(6):649, an author-name correction in the PubMed record of PMID [18516091](https://pubmed.ncbi.nlm.nih.gov/18516091/); the PubMed record carries no PMID for the erratum.

- Count of 1,770 harvested, 930 core and 280 deeply read records, of which 216 from full text, and the 1,634 paywalled body-text papers (section 2.1): project literature corpus [UNVERIFIED: corpus table not published with this report].

- Coverage check (section 2.1): NCBI E-utilities `esearch`, `db=pubmed`, term `BUB1B[tiab] OR BUBR1[tiab]`, run 2026-10-24, 1,275 records, compared by PMID with the 1,256 records of the Europe PMC gene search that carry a PMID. The unrestricted full-text count (7,228) uses the query `BUB1B OR BUBR1` on the same date.
