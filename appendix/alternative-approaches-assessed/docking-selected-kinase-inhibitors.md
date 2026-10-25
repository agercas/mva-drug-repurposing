# Kinase inhibitors chosen by docking

## Claim as stated

One proposal docked a vendor library of marketed compounds (AutoDock Vina) at the lysine side chain that the N1002K change creates in BubR1, the spindle checkpoint protein encoded by *BUB1B*. It then ordered 14 approved drugs by the affinity predicted by a second program (DynamicBind) and named six approved cancer kinase inhibitors as docking leads: pralsetinib, lapatinib, tucatinib, entrectinib, capmatinib and ponatinib. A hit in its proposed assay is any compound that moves nuclear counts in *BUB1B*-knockdown HeLa cells toward the control value.

## Evidence for

- The proposal provides its docking and DynamicBind score tables, so the summary statistics can be recomputed from the tables, although the docking itself cannot be rerun.

- The proposal excludes spindle poisons and mitotic-kinase inhibitors by name, and excludes ponatinib and lapatinib for their boxed warnings.

## Evidence against

1. **The poses stay far from the target residue.** In the proposal's table of 14 drugs, the ligand lies 25.7 to 31.3 Å from the lysine in the mutant pose. No pose comes within 8 Å, and no pose moves toward the wild-type window (recomputed from the supplied table by this report).

2. **The ranking carries no information about the allele.** The predicted affinity for the mutant minus that for the wild type has a median of -0.06 (range -0.57 to +0.26), and the mutant and wild-type affinity columns correlate at Spearman 0.89 across the 14 drugs. The order reflects properties of each ligand (recomputed from the supplied table).

3. **Docking accuracy depends on settings.** Pose accuracy in AutoDock Vina varies with search box size and exhaustiveness (PMID [36262028](https://pubmed.ncbi.nlm.nih.gov/36262028/); abstract read), and the proposal uses a single pose per ligand with no decoys or known binder.

4. **The structural premise comes from a predicted model.** Residues 766 to 1050 are unresolved in every human experimental model. Structure-prediction metrics correlate weakly with the stability change caused by a single substitution (PMID [36928239](https://pubmed.ncbi.nlm.nih.gov/36928239/); abstract read). Whether the new lysine is exposed or is a ubiquitin acceptor is unmeasured.

5. **No stabiliser pocket is known.** A pocket search on the predicted unliganded model found no stabiliser-grade pocket, and its positive control recovered two known ligand sites at rank 1. The ChEMBL activity record for BubR1 holds 24 values over 15 molecules, with a strongest value of 9.67 µM (PMID [39818011](https://pubmed.ncbi.nlm.nih.gov/39818011/)), so a screen has to beat that value to add to the record.

6. **The readout moves with proliferation.** The assay counts nuclei: 88 in control and 43 after knockdown, in one imaging session at one magnification, without a replicate, a knockdown-efficiency measurement or a drug arm. Any compound that changes proliferation or cytotoxicity moves a nuclear count, and antiproliferative kinase inhibitors are expected to lower it.

7. **Labels record findings in children and in assays.** The entrectinib label records a potential for abnormal chromosome segregation (aneugenicity) in an in vitro assay in human lymphocytes, while the in vivo rat micronucleus assay was negative. The pralsetinib label records physeal dysplasia (abnormal growth-plate development) in non-human primates at exposures similar to the human clinical exposure.

8. **Paediatric indications limit the remaining leads.** Pralsetinib is established from 12 years for RET fusion-positive thyroid cancer only, and labelled uses of these drugs require a tumour with the matching genotype. The two leads the proposal excludes carry boxed warnings: lapatinib for hepatotoxicity, ponatinib for arterial occlusive events, venous thromboembolism, heart failure and hepatotoxicity.

## Conclusion

The approach is unsupported. The docked poses sit about 28 Å from the target residue, the ranking does not depend on the allele, the readout moves with proliferation, and the lead drugs are antiproliferative kinase inhibitors with label findings in children.

## Same weakness in this report

The report's own structure work cannot rank stabilisers either: the pocket search found no stabiliser-grade pocket, and the screening bar of 9.67 µM applies to any future screen. A measurement of the abundance and half-life of the missense protein would show whether a stabiliser has a target to act on.

## References

- Agarwal R et al. (2023). Speed vs Accuracy: Effect on Ligand Pose Accuracy of Varying Box Size and Exhaustiveness in AutoDock Vina. *Mol Inform*. PMID [36262028](https://pubmed.ncbi.nlm.nih.gov/36262028/)
- Pak MA et al. (2023). Using AlphaFold to predict the impact of single mutations on protein stability and function. *PLoS One*. PMID [36928239](https://pubmed.ncbi.nlm.nih.gov/36928239/)
- El Hafi M et al. (2025). Synthesis and biological assessment of BUB1B inhibitors for the treatment of clear cell renal cell carcinoma. *Eur J Med Chem*. PMID [39818011](https://pubmed.ncbi.nlm.nih.gov/39818011/)

## Other sources

- Score tables of the proposal (distance of the ligand to the lysine, predicted affinities for mutant and wild type): recomputed for this report from the proposal's supplied table; the table is not republished here [UNVERIFIED: the docking inputs and poses are withheld by the proposal, so the scores themselves cannot be reproduced].

- GAVRETO (pralsetinib), openFDA drug label API, search `openfda.generic_name:pralsetinib`, label effective 2025-12-30, read 2026-10-24: https://api.fda.gov/drug/label.json?search=openfda.generic_name:pralsetinib (section 8.4: established from 12 years for RET fusion-positive thyroid cancer; physeal dysplasia in non-human primates at exposures similar to the human clinical exposure).

- ROZLYTREK (entrectinib), DailyMed set id c7c71b0c-2549-4495-86b6-c2807fa54908, read 2026-10-24: https://dailymed.nlm.nih.gov/dailymed/lookup.cfm?setid=c7c71b0c-2549-4495-86b6-c2807fa54908 (section 13.1: in vitro potential for abnormal chromosome segregation in human lymphocytes; not aneugenic or clastogenic in the in vivo rat micronucleus assay).

- Lapatinib prescribing information, openFDA drug label API, search `openfda.generic_name:lapatinib`, label effective 2025-03-12, read 2026-10-24: https://api.fda.gov/drug/label.json?search=openfda.generic_name:lapatinib (boxed warning: hepatotoxicity). ICLUSIG (ponatinib), openFDA drug label API, search `openfda.generic_name:ponatinib`, label effective 2026-08-14, read 2026-10-24: https://api.fda.gov/drug/label.json?search=openfda.generic_name:ponatinib (boxed warning: arterial occlusive events, venous thromboembolic events, heart failure and hepatotoxicity).

- Residues 766 to 1050 are unresolved in the Protein Data Bank entries that map to human BubR1 (2WVI, 3SI5, 4GGD, 5JJA, 5K6S, 5SWF, 5LCW, 6TLJ, 5KHU), queried 2026-10-15 [UNVERIFIED: query not repeated on 2026-10-24].

- The claims assessed are quoted from the proposal's public repository, which is cited by claim only. The nuclear counts (88 and 43) and the single imaging session are quoted from that repository [UNVERIFIED: images not reviewed by this report].
