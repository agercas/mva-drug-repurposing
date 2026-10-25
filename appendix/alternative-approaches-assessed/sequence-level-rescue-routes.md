# Sequence-level rescue routes

## Claim as stated

One proposal works out, from the RefSeq transcript NM_001211.6, what editing chemistries can do to the two public variant codons: c.2210T>G (p.Leu737Ter, TTA to TGA, exon 17 of 23) and c.3006T>G (p.Asn1002Lys, AAT to AAG, last exon).

It lays out six research branches: native correction or controlled transcript or gene replacement; a leucine-decoding suppressor transfer RNA (tRNA) for the UGA stop; defined L737W, L737R and L737C products; protection of the N1002K protein; skipping of exon 17; and protection of the transcript from nonsense-mediated decay (NMD). The proposal names no drug and gives no measured efficiency.

## Evidence for

- Codon arithmetic reproduces from the reference. Reverting TGA to TTA and AAG to AAT each needs a G to T change, which adenine and cytosine base editors cannot make. Programmable A-to-I RNA editing (PMID [29070703](https://pubmed.ncbi.nlm.nih.gov/29070703/)) turns adenine into inosine, which the ribosome reads as guanosine, so editing the A of UGA gives UGG, tryptophan. No editing of the two adenines of AAG returns asparagine.

- Exon 17 holds 141 coding bases, so skipping keeps the reading frame and gives a protein of 1,003 residues that lacks Glu715 to Leu761 (141 / 3 = 47 residues; 1,050 − 47 = 1,003). Six exon junctions follow the stop codon, the last 746 nucleotides downstream of the codon's end (NM_001211.6: codon ends at position 2363, last junction after position 3109), which predicts decay of the stop-allele transcript.

- An adeno-associated virus (AAV)-delivered suppressor tRNA rescued a disease phenotype in a mouse model of a nonsense mutation. The effect lasted more than 6 months after one treatment, partly through readthrough and partly through inhibition of NMD (PMID [35322228](https://pubmed.ncbi.nlm.nih.gov/35322228/); abstract read).

- Anticodon-engineered tRNAs suppressed premature stop codons in mammalian cells, *Xenopus* oocytes and mice, including in *CFTR* (the cystic fibrosis transmembrane conductance regulator gene), with limited interaction with natural termination codons by ribosome profiling (PMID [30778053](https://pubmed.ncbi.nlm.nih.gov/30778053/); abstract read).

- Prime editing converted an endogenous Leu-TAA tRNA gene into a TAG suppressor with 100% leucine charging fidelity. It restored 20 to 70% of normal enzyme activity in human cell-line models of six nonsense variants and gave 6.3 to 7.6% of wild-type enzyme activity in cortex and heart of a Hurler-syndrome mouse (n = 3 per condition). Proteome mass spectrometry in HEK293T cells detected no readthrough peptides among 4,036 natural TAG stops (PMID [41261131](https://pubmed.ncbi.nlm.nih.gov/41261131/); full text read).

- A leucine UCA suppressor read through a TGA reporter in neonatal mouse brain: 23% editing of the converted gene gave 26% of the protein yield of a co-delivered TGA reporter (n = 4 per condition; the inserted residue was unmeasured; PMID [41261131](https://pubmed.ncbi.nlm.nih.gov/41261131/)).

- An arginine-decoding UCA suppressor tRNA repaired a UGA stop in mouse brain (PMID [42460447](https://pubmed.ncbi.nlm.nih.gov/42460447/); abstract read).

- Position 737 is leucine in 110 of 115 vertebrate orthologues, and none of the 115 carries tryptophan, cysteine or arginine. A leucine-decoding suppressor avoids the substitution that readthrough drugs and ADAR editing insert.

## Evidence against

1. **No route was tested in *BUB1B*.** Every source above concerns another gene. The proposal reports no efficiency, guide, delivery or off-target work.

2. **Decay removes the substrate.** The stop-allele transcript is a decay target, inferred from Northern blots in two experiments (PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/); full text read). No allele-resolved transcript measurement exists.

3. **The suppressor tRNA yield is low.** The model in section 5.7 gives a median 0.04 to 0.10 of one wild-type allele per edited cell (5th to 95th percentile 0.01 to 0.34) at an assumed readthrough of 0.05 to 0.40. Carrier-level function needs 0.7 to 1.0 added alleles. In the most favourable of the three coupling models, at 25% of cells edited, the mean product reaches 0.03 alleles in 44% of draws and stays below 0.1 in all draws.

4. **Prime-editing reversion yields more in the same cells.** Reversion by the same ex vivo edit in blood stem cells restores one wild-type allele per edited cell, 10 to 25 times the suppressor yield per edited cell. The report's prime-editing card covers it, and the lentiviral add-back card covers gene addition.

5. **Editing efficiency in blood progenitors is unmeasured.** No study reports prime editing at a tRNA gene in haematopoietic progenitors. The converted tRNA-Leu-TAA-1-1 gene was 2.5-fold (engineered) to 5.6-fold (anticodon-only) less abundant than the endogenous gene it replaced, measured for the TAG-reading suppressor (PMID [41261131](https://pubmed.ncbi.nlm.nih.gov/41261131/)).

6. **The safety data come from the TAG version.** The authors argue that TAG is the safest stop codon for suppression, and proteome-wide readthrough was measured for the TAG suppressor only. The TGA version is the one needed here. Leucine charging fidelity of the UCA variant and the residue inserted at the *BUB1B* stop are unmeasured (PMID [41261131](https://pubmed.ncbi.nlm.nih.gov/41261131/)).

7. **Delivered tRNA dilutes.** A non-integrating vector halves in concentration at each cell division. Delivered tRNA suits tissues that divide rarely, and marrow, gut and skin divide often.

8. **Readthrough drugs and ADAR editing (adenosine deaminase acting on RNA) insert other residues.** Ataluren favours near-cognate tRNAs at stop codons and produces context-dependent mixtures of residues (PMID [27702906](https://pubmed.ncbi.nlm.nih.gov/27702906/); abstract read). The proposal lists tryptophan, arginine and cysteine as the defined products, and none of the three occurs at position 737 in the 115 orthologues.

9. **Exon skipping edits both alleles.** An oligonucleotide aimed at the splice sites of exon 17 also deletes residues 715 to 761 from the N1002K copy. A break-even calculation in this report shows non-selective skipping helps only if the deleted protein keeps more than about 0.35 to 0.5 of normal activity. That activity is unmeasured, and the deleted segment contains reported patient variants [UNVERIFIED: variant count taken from the project's allele atlas].

10. **Gene replacement has no design in the proposal.** The proposal names the branch without a construct, a dose or a test.

## Conclusion

The sequence derivations hold, and the routes are established for other nonsense alleles. For *BUB1B* each route lacks the same three measurements: residual stop-allele transcript, the inserted residue, and editing efficiency in blood stem cells. The suppressor tRNA yields one tenth to one twenty-fifth of reversion per edited cell, ADAR and base editing give or leave the wrong residue, and exon skipping edits both alleles.

## Same weakness in this report

The prime-editing and lentiviral add-back cards cover the DNA-level correction routes. They depend on the same blood stem cells, conditioning and unmeasured corrected-cell advantage. An allele-resolved transcript measurement with and without a translation inhibitor shows whether the stop allele escapes decay, and a reporter assay with peptide mass spectrometry shows which residue a suppressor inserts.

## References

- Suijkerbuijk SJ et al. (2010). Molecular causes for BUBR1 dysfunction in the human cancer predisposition syndrome mosaic variegated aneuploidy. *Cancer Res*. PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/)
- Roy B et al. (2016). Ataluren stimulates ribosomal selection of near-cognate tRNAs to promote nonsense suppression. *Proc Natl Acad Sci U S A*. PMID [27702906](https://pubmed.ncbi.nlm.nih.gov/27702906/)
- Cox DBT et al. (2017). RNA editing with CRISPR-Cas13. *Science*. PMID [29070703](https://pubmed.ncbi.nlm.nih.gov/29070703/)
- Lueck JD et al. (2019). Engineered transfer RNAs for suppression of premature termination codons. *Nat Commun*. PMID [30778053](https://pubmed.ncbi.nlm.nih.gov/30778053/)
- Wang J et al. (2022). AAV-delivered suppressor tRNA overcomes a nonsense mutation in mice. *Nature*. PMID [35322228](https://pubmed.ncbi.nlm.nih.gov/35322228/)
- Pierce SE et al. (2025). Prime editing-installed suppressor tRNAs for disease-agnostic genome editing. *Nature*. PMID [41261131](https://pubmed.ncbi.nlm.nih.gov/41261131/)
- Al Saneh A et al. (2026). Programmed repair of disease-causing UGA premature termination codons in mammalian brain. *Nucleic Acids Res*. PMID [42460447](https://pubmed.ncbi.nlm.nih.gov/42460447/)

## Other sources

- RefSeq NM_001211.6 (*BUB1B*) and UniProt O60566 (BUB1B_HUMAN), read 2026-10-24; the codon and exon statements are re-derived from the reference sequence for this report.

- Conservation of position 737 across 115 vertebrate BubR1 sequences: computed for this report from UniProt O60566 orthologue alignments [UNVERIFIED: alignment source list not recorded].

- The model yield of 0.04 to 0.10 added alleles per edited cell and the 25%-edited result are projections from the model of section 5.7.

- The six branches are quoted from the proposal's public repository, which is cited by claim only.
