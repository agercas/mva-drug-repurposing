# Cell-cycle map of cyclins, CDKs and the APC/C

The map follows the cell cycle from quiescence (the resting state) to the first G1 phase (the gap phase after division). It covers cyclins, cyclin-dependent kinases (CDKs) and the anaphase-promoting complex/cyclosome (APC/C), a ubiquitin ligase that triggers chromosome separation, and shows where a low dose of BubR1, a spindle assembly checkpoint protein, acts. Its 74 rows yield six excluded drug classes and six measurements and nominate no new candidate.

Each row describes one node (a protein or regulatory step) and gives the type of evidence, the published effect of low BubR1, the available modulators and the sign of raising the node. Rows by type of evidence: 10 human biochemistry or structure, 5 human genetics, 2 patient cells, 5 mouse genetics, 50 cell lines, 2 inference.

## Findings

1. **Two-sided levers.** Twenty-three of 74 nodes are harmful when moved in either direction. Cyclin-CDK activity touches BubR1 at five points, and at four of them the lever is two-sided.

2. **Thr620 as licensing site and degron.** Thr620 (threonine 620) is the cyclin B1–CDK1 site that creates the docking position of Polo-like kinase 1 (PLK1) for error correction (PMID [17785528](https://pubmed.ncbi.nlm.nih.gov/17785528/); abstract read). One primary study (PMID [38008853](https://pubmed.ncbi.nlm.nih.gov/38008853/); full text read) reports that it is also a phosphodegron (a phosphorylated site that marks a protein for destruction) read by SCF-FBXW7, a ubiquitin ligase: in HEK293T cells a T620A mutant bound FBXW7 less and was ubiquitinated less, and CDK1 inhibition disrupted FBXW7-mediated targeting.

   Lowering CDK1 activity would then raise BubR1 amount and lower its function. The sign of a CDK1-directed hypothesis depends on whether a cell is limited by protein amount or by function.

   The degron claim rests on that one study, in overexpression assays, and lacks a validated antibody. In a cell already in mitosis, lowering CDK1 forces mitotic exit, so the trade-off applies to the interphase pool (BubR1 in cells between divisions) only.

3. **Two sensors in one domain.** The 18-residue domain that recruits the phosphatase PP2A-B56 (protein phosphatase 2A with its B56 subunit) carries a sensor of attachment (serine 670) and a sensor of tension (serine 676 and threonine 680; residues 665 to 682, reviewed in PMID [33892776](https://pubmed.ncbi.nlm.nih.gov/33892776/)). A pooled readout averages the two.

4. **Predicted p53 target.** *BUB1B* is one of 210 computationally predicted targets of the p53–p21–DREAM pathway, in which p53 raises p21 and the DREAM repressor complex then silences cell-cycle genes (PMID [26384566](https://pubmed.ncbi.nlm.nih.gov/26384566/); full text read, Table 1). The paper cites two earlier reports of p21-dependent repression of *BUB1B*. The paper reports no functional test of the regulatory element, so the pathway claim stays a prediction. Agents that raise p53 therefore stay off the candidate list.

5. **Cost of long mitosis.** Cells arrested in mitosis with monastrol (an inhibitor of the spindle motor protein Eg5) for six hours had about 60% less cyclin A and more stable microtubule attachments than cells arrested for one hour, and a higher share of anaphases with lagging chromosomes after release (PMID [24013174](https://pubmed.ncbi.nlm.nih.gov/24013174/); full text read; U2OS and RPE-1 cells; at least 10 cells for attachment measurements and 20 for lagging-chromosome scoring). The comparison covers one pair of durations and a drug-induced arrest.

6. **Available agents are inhibitors.** A census of 16 nodes among cyclins, CDKs, the APC/C and phosphatases, with working positive and negative controls, returned only inhibitors where an agent exists and no mechanism entry for 13 of 16 nodes. A stabiliser would have to be built.

7. **Higher BubR1 coincided with longer mitosis.** In HeLa cells depleted of FBXW7 by small interfering RNA (siRNA), BubR1 rose 2.33 ± 0.88-fold in mitotically synchronised lysates (Fig. 2e legend) and metaphase to anaphase lengthened from 15 to 25 minutes to 45 to 65 minutes (Fig. 1d legend; PMID [38008853](https://pubmed.ncbi.nlm.nih.gov/38008853/), full text read).

   The knockdown was in one cancer cell line, and raising BubR1 by removing a degradation pathway coincided with a delayed anaphase. A safe ceiling for raising BubR1 in patient cells needs its own measurement.

## Excluded cell-cycle drug classes

Six drug classes are excluded. The table gives the basis for each exclusion and its evidence.

| Class | Basis for exclusion | Evidence |
|---|---|---|
| CDK4/6 inhibitors | The label of the approved agent palbociclib reports that it was aneugenic (caused abnormal chromosome numbers) in Chinese hamster ovary cells and in rat bone marrow at 100 mg/kg/day or more; biallelic (both gene copies) *CDK4* loss of function caused microcephaly and short stature in individuals from two families; the class is anti-proliferative in an already growth-restricted child | Palbociclib label (openFDA, effective 2026-07-06, read 2026-10-24); PMID [40210435](https://pubmed.ncbi.nlm.nih.gov/40210435/) (full text read; two families, no replication found) |
| CDK2 inhibitors | One research group reports that CDK2 inhibition disorders centrosome stoichiometry, drives multipolar mitosis and leaves persistent polyploid cells in aneuploid lung cancer cell lines, with fewer such cells in primary alveolar epithelial cells; the comparison is cancer lines against primary cells, which differ in genetic background; raising the node has the wrong sign on the same load argument | PMIDs [38031910](https://pubmed.ncbi.nlm.nih.gov/38031910/) and [40232858](https://pubmed.ncbi.nlm.nih.gov/40232858/) (full text available, abstracts read; shared authorship) |
| CDK12/13 inhibitors | Depleting cyclin K/CDK12 lowers expression of DNA-damage-response genes and causes spontaneous DNA damage in human cells; the premise that BubR1-weak cells carry replication load comes from mice with BubR1 acetylation deficiency (K243R) crossed to p53-null mice, which is a different lesion from low BubR1 | PMIDs [22012619](https://pubmed.ncbi.nlm.nih.gov/22012619/), [33955658](https://pubmed.ncbi.nlm.nih.gov/33955658/) (abstract read) |
| Lengthening G2 (the gap phase before mitosis) | The lever moves the same CDK1 pool that runs mitosis; a prolonged p53-competent G2 can lead to senescence or to a tetraploid G1; every agent at the node points the wrong way | Senescence literature, abstract read only [UNVERIFIED] |
| Inhibiting the interphase APC/C activator (FZR1) | Three de novo (not inherited) *FZR1* missense (single amino-acid change) variants, shown to be loss of function in *Drosophila*, occurred in individuals with developmental and epileptic encephalopathy; *Fzr1* heterozygous loss impairs haematopoietic stem-cell quiescence in two mouse models | PMIDs [34788397](https://pubmed.ncbi.nlm.nih.gov/34788397/), [34635784](https://pubmed.ncbi.nlm.nih.gov/34635784/) (abstract read) |
| Weakening the mitotic-surveillance pathway | In the mitotic-surveillance (stopwatch) pathway, USP28 and 53BP1 activate p53 after delayed mitosis, and p53 loss rescues progenitor cells in several mouse models; removing the pathway would rescue cells that should be eliminated, which is the wrong direction in a cancer-predisposition syndrome | PMID [39398482](https://pubmed.ncbi.nlm.nih.gov/39398482/) (minireview; full text skimmed; primary studies not read) |

## Verification

An independent AI reviewer (a separate Claude session) rechecked ten load-bearing claims against primary sources and by rerunning code. Seven held, some with a narrowing. Three were corrected:

- A claim that the p53–p21–DREAM regulation of *BUB1B* was established became a prediction.
- A claim that no cyclin has an agent was false for cyclin D1 (palbociclib is approved against the complex).
- One degron residue range was off by one.

Fourteen hypotheses went to independent blind review by AI agents: one held unchanged, one was refuted and 12 were narrowed.

## Measurements the map specifies

1. Image attachment-sensor and tension-sensor phosphosites (phosphorylated residues) per kinetochore (the chromosome site where spindle microtubules attach) across an allelic series at equal BubR1 abundance.

2. Measure the degron site, the attachment site and kinetochore PP2A-B56 per unit BubR1 under a sub-saturating CDK1-inhibitor series, looking for opposite slopes in amount and function.

3. Run a cycloheximide chase of BubR1 (block protein synthesis, then follow the decay of BubR1) in two cell-cycle windows to measure interphase half-life.

4. Sort p21-high and p21-low sibling cells after induced missegregation and measure BubR1 in both.

5. Count lagging chromosomes and micronuclei (small extra nuclei formed from lost chromosomes) in published *CDK4* loss-of-function patient fibroblasts.

6. Image MAD1 at the kinetochore corona against BubR1 dose.

## Limits

The map's evidence is cell-line work in 50 of 74 rows. None of the 74 rows reports an effect of a low BubR1 dose measured in a cell from this disease.

## References

- Elowe S et al. (2007). Tension-sensitive Plk1 phosphorylation on BubR1 regulates the stability of kinetochore microtubule interactions. *Genes Dev*. PMID [17785528](https://pubmed.ncbi.nlm.nih.gov/17785528/)
- Blazek D et al. (2011). The Cyclin K/Cdk12 complex maintains genomic stability via regulation of expression of DNA damage response genes. *Genes Dev*. PMID [22012619](https://pubmed.ncbi.nlm.nih.gov/22012619/)
- Kabeche L et al. (2013). Cyclin A regulates kinetochore microtubules to promote faithful chromosome segregation. *Nature*. PMID [24013174](https://pubmed.ncbi.nlm.nih.gov/24013174/)
- Fischer M et al. (2016). The p53-p21-DREAM-CDE/CHR pathway regulates G2/M cell cycle genes. *Nucleic Acids Res*. PMID [26384566](https://pubmed.ncbi.nlm.nih.gov/26384566/)
- Bloom CR, North BJ (2021). Physiological relevance of post-translational regulation of the spindle assembly checkpoint protein BubR1. *Cell Biosci*. PMID [33892776](https://pubmed.ncbi.nlm.nih.gov/33892776/)
- Park J et al. (2021). Loss of BubR1 acetylation provokes replication stress and leads to complex chromosomal rearrangements. *FEBS J*. PMID [33955658](https://pubmed.ncbi.nlm.nih.gov/33955658/)
- Zhou C et al. (2022). Insufficiency of FZR1 disturbs HSC quiescence by inhibiting ubiquitin-dependent degradation of RUNX1 in aplastic anemia. *Leukemia*. PMID [34635784](https://pubmed.ncbi.nlm.nih.gov/34635784/)
- Manivannan SN et al. (2022). De novo FZR1 loss-of-function variants cause developmental and epileptic encephalopathies. *Brain*. PMID [34788397](https://pubmed.ncbi.nlm.nih.gov/34788397/)
- Nair VM et al. (2023). E3-ubiquitin ligase, FBXW7 regulates mitotic progression by targeting BubR1 for ubiquitin-mediated degradation. *Cell Mol Life Sci*. PMID [38008853](https://pubmed.ncbi.nlm.nih.gov/38008853/)
- Chen Z et al. (2023). CDK2 inhibition disorders centrosome stoichiometry and alters cellular outcomes in aneuploid cancer cells. *Cancer Biol Ther*. PMID [38031910](https://pubmed.ncbi.nlm.nih.gov/38031910/)
- Stracker TH (2024). Regulation of p53 by the mitotic surveillance/stopwatch pathway: implications in neurodevelopment and cancer. *Front Cell Dev Biol*. PMID [39398482](https://pubmed.ncbi.nlm.nih.gov/39398482/)
- Verdu Schlie A et al. (2025). CDK4 loss-of-function mutations cause microcephaly and short stature. *Genes Dev*. PMID [40210435](https://pubmed.ncbi.nlm.nih.gov/40210435/)
- Tyutyunyk-Massey L et al. (2025). CDK2 inhibition produces a persistent population of polyploid cancer cells. *JCI Insight*. PMID [40232858](https://pubmed.ncbi.nlm.nih.gov/40232858/)

## Other sources

- IBRANCE (palbociclib), prescribing information, DailyMed set id 89a142d5-7e61-48bf-9e77-e2cd124c4792: aneugenic in Chinese hamster ovary cells in vitro and in rat bone marrow at 100 mg/kg/day or more for 3 weeks. Read 2026-10-24: https://dailymed.nlm.nih.gov/dailymed/lookup.cfm?setid=89a142d5-7e61-48bf-9e77-e2cd124c4792
- Cyclin, CDK and APC/C node table: this report's literature review [UNVERIFIED: per-node evidence table not published with this report; the PMIDs cited above carry the individual claims].
