# Disease and case

Mosaic variegated aneuploidy (MVA) is a recessive chromosome-instability syndrome (disease appears when both copies of the gene are affected). The child in this report carries two different *BUB1B* variants: a stop-gain (a change that ends the protein early) and a missense change (a change that swaps one amino acid). The amount of working BubR1 protein they leave is unmeasured. Navigation: [README](README.md) · next: [Reported research](02-reported-research.md).

## 1.1 Mosaic variegated aneuploidy and *BUB1B*

MVA cells carry whole-chromosome gains and losses (aneuploidy) that differ from cell to cell. The hallmark is constitutional mosaicism (cells with different chromosome numbers in one person, present from early development) for trisomies (an extra copy of a chromosome) and monosomies (a missing copy) (PubMed identifier, PMID [15475955](https://pubmed.ncbi.nlm.nih.gov/15475955/), abstract read). A mouse-model paper describes the syndrome as typically involving aneuploidy in more than 25% of cells (PMID [23300461](https://pubmed.ncbi.nlm.nih.gov/23300461/), full text read; a secondary statement citing patient reports). A formal diagnostic cut-off is [UNVERIFIED: not established in the sources read].

Premature chromatid separation (PCS) is the cytogenetic sign of a weak spindle assembly checkpoint. In PCS, the two copies of a replicated chromosome (sister chromatids) part before anaphase, the stage when they are pulled apart. The checkpoint is the control that delays chromosome separation until every chromosome is attached to the spindle (PMID [16411201](https://pubmed.ncbi.nlm.nih.gov/16411201/), abstract read).

Biallelic variants (a change on each copy of the gene) in *BUB1B* cause MVA type 1 (MVA1). ClinVar, the archive of variant classifications kept by the National Center for Biotechnology Information (NCBI), lists the stop-gain below (record 533901) as pathogenic or likely pathogenic for MVA1.

The founding report describes growth retardation, microcephaly, childhood cancer and constitutional mosaicism for chromosomal gains and losses, with embryonal rhabdomyosarcoma in two of five families with biallelic variants (PMID [15475955](https://pubmed.ncbi.nlm.nih.gov/15475955/), full text read). A 2024 update from the American Association for Cancer Research workshop of July 2023, based on case reports and small series, lists Wilms tumour and rhabdomyosarcoma as the main cancers in MVA1, with myelodysplastic syndrome, acute myeloid leukaemia and acute lymphoblastic leukaemia also reported (PMID [39264246](https://pubmed.ncbi.nlm.nih.gov/39264246/), full text read).

## 1.2 BubR1 in the spindle assembly checkpoint

*BUB1B* encodes BubR1 (UniProt O60566), a component of the spindle assembly checkpoint (SAC). BubR1 inhibits the anaphase-promoting complex/cyclosome (APC/C, the enzyme complex that starts anaphase) (PMIDs [11535616](https://pubmed.ncbi.nlm.nih.gov/11535616/), [11702782](https://pubmed.ncbi.nlm.nih.gov/11702782/); read basis in [section 2.4.11](02-reported-research.md#2411-sudakin-2001-and-tang-2001-checkpoint-complex)). Too little BubR1 weakens the checkpoint, and cells then segregate chromosomes unevenly.

BubR1 has further reported roles at the kinetochore (the protein structure where spindle fibres attach to a chromosome). It recruits the phosphatase PP2A-B56 (protein phosphatase 2A with a B56 regulatory subunit), which opposes Aurora B kinase (PMID [23789096](https://pubmed.ncbi.nlm.nih.gov/23789096/)). It inhibits polo-like kinase 1 (PLK1) in interphase cells (PMID [19503101](https://pubmed.ncbi.nlm.nih.gov/19503101/)). It interacts with the motor protein CENP-E (centromere protein E) (PMID [11702782](https://pubmed.ncbi.nlm.nih.gov/11702782/)). The report read the abstracts for these three roles, and the rescue figures of the first paper in full text ([section 2.6](02-reported-research.md#26-findings-checked-in-full-text)). [Reported research](02-reported-research.md) reviews the evidence for each role.

## 1.3 The two variants

| | Allele 1 | Allele 2 |
|---|---|---|
| Position (GRCh38, the human reference genome build) | chr15:40209701 T>G | chr15:40220612 T>G |
| Transcript change | NM_001211.6:c.2210T>G | NM_001211.6:c.3006T>G |
| Protein change | p.Leu737Ter (stop-gain, exon 17 of 23) | p.Asn1002Lys (missense, last exon, kinase domain) |
| Expected effect | Nonsense-mediated decay (NMD, degradation of transcripts with premature stop signals) | Altered protein; effect unmeasured |
| ClinVar (read 2026-10-24) | 533901: pathogenic or likely pathogenic for MVA1; criteria provided, multiple submitters, no conflicts | Not recorded for this nucleotide change; 4600147 (c.3006T>A, same protein change) is a variant of uncertain significance with criteria provided and a single submitter |
| gnomAD v4 (Genome Aggregation Database; read 2026-10-24) | 115 of 1,461,846 exome alleles (7.9e-05) and 5 of 152,174 genome alleles | 1 of 1,461,878 exome alleles; absent from genomes |

These are the only two protein-altering variants called in the gene (2 of 14 variants called in the gene change the protein; Track 1 repository, `results/crosscheck.txt`). Short-read data identify each variant but leave open which copy of chromosome 15 carries it (phase), so the report treats them as compound heterozygous (a different change on each copy of the gene), which is consistent with recessive disease. The Track 1 report documents the identification and the exon-depth check that excludes exon-scale deletions.

## 1.4 Mechanism characterisation

The best-supported reading is loss of function: allele 1 is expected to make little or no BubR1, and the residual protein comes from allele 2. Truncating variants in the last exon would escape NMD. Allele 1 lies in exon 17 of 23, about 750 bases before the last exon-exon junction (Track 1 report, section 4.2; 746 nucleotides from the end of the stop codon in [section 5.1](05-computational-findings.md#51-two-allele-architecture)), so NMD is predicted. The transcript of this allele is unmeasured. Five steps connect the genotype to the cellular phenotype:

1. Allele 1 reduces BubR1 transcript through NMD.
2. Allele 2 supplies the only full-length protein, of unmeasured abundance and activity.
3. Low functional BubR1 weakens the SAC and APC/C inhibition.
4. Chromatids separate early (PCS) and daughter cells inherit the wrong chromosome number.
5. Aneuploid cells arrest, die or persist, which is the proposed route to growth restriction and cancer predisposition.

Two cell results come from one paper (PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/), main text and legends read; supplement not read):

- In HeLa and U2OS cells (human cancer cell lines) expressing tagged BubR1, kinase-region missense proteins (I909T, L1012P and others) were 5 to 10 times less abundant than wild type. I909T and L1012P restored checkpoint function when overexpressed to near-wild-type level, and L844F was poorly expressed and restored none of the defects.
- A doxycycline titration in HeLa cells gave near-normal segregation at about 13% BubR1 and errors at about 6%.

The system is transformed cell lines with ectopic protein, and the degradation mechanism rests on one representative experiment. [Reported research](02-reported-research.md) grades the pathway evidence for steps 3 to 5.

## 1.5 Phenotype terms supplied

The data provider supplied eight terms from the Human Phenotype Ontology (HPO, a standard vocabulary of clinical features).

## 1.6 Further genetic findings from Track 1

Besides the *BUB1B* stop-gain, the Track 1 analysis found five heterozygous variants (one copy of the gene affected) with good read support: one secondary finding, listed in the Track 1 report, and four carrier-state variants (a single damaged copy of a recessive gene) in genes unrelated to *BUB1B*. Counting the stop-gain, the Track 1 report lists six such variants in all (sections 4.4 and 7).

Each candidate card in [Approved drugs](03-approved-drugs/README.md) and [Non-approved therapies](04-non-approved-therapies/README.md) records a pass or fail on whether the candidate's known effects bear on genes carrying such variants. The report gives the four carrier-state variants as a count and as these per-candidate results; anyone holding the child's genome can check any candidate against all variants in it.

## 1.7 Unmeasured quantities that bear on every candidate

Four unmeasured quantities decide which candidates are worth testing:

| Quantity | Why it matters |
|---|---|
| BubR1 protein abundance from allele 2 | Sets how many-fold a treatment must raise functional protein |
| BubR1 protein half-life from allele 2 | Separates a synthesis problem from a degradation problem |
| Activity of the allele 2 protein in the checkpoint | Separates low abundance from low function |
| Phase of the two variants | A single-chromosome reading (both variants on one copy) would change the genotype class |

[Section 5.10](05-computational-findings.md#510-experimental-platform-shared-by-sections-3-and-4) describes each measurement in the shared experimental platform. Candidate cards in sections 3 and 4 refer back to these four quantities.

## References

- Sudakin V et al. (2001). Checkpoint inhibition of the APC/C in HeLa cells is mediated by a complex of BUBR1, BUB3, CDC20, and MAD2. *J Cell Biol*. PMID [11535616](https://pubmed.ncbi.nlm.nih.gov/11535616/)
- Tang Z et al. (2001). Mad2-Independent inhibition of APCCdc20 by the mitotic checkpoint protein BubR1. *Dev Cell*. PMID [11702782](https://pubmed.ncbi.nlm.nih.gov/11702782/)
- Hanks S et al. (2004). Constitutional aneuploidy and cancer predisposition caused by biallelic mutations in BUB1B. *Nat Genet*. PMID [15475955](https://pubmed.ncbi.nlm.nih.gov/15475955/)
- Matsuura S et al. (2006). Monoallelic BUB1B mutations and defective mitotic-spindle checkpoint in seven families with premature chromatid separation (PCS) syndrome. *Am J Med Genet A*. PMID [16411201](https://pubmed.ncbi.nlm.nih.gov/16411201/)
- Izumi H et al. (2009). BubR1 localizes to centrosomes and suppresses centrosome amplification via regulating Plk1 activity in interphase cells. *Oncogene*. PMID [19503101](https://pubmed.ncbi.nlm.nih.gov/19503101/)
- Suijkerbuijk SJ et al. (2010). Molecular causes for BUBR1 dysfunction in the human cancer predisposition syndrome mosaic variegated aneuploidy. *Cancer Res*. PMID [20516114](https://pubmed.ncbi.nlm.nih.gov/20516114/)
- Wijshake T et al. (2012). Reduced life- and healthspan in mice carrying a mono-allelic BubR1 MVA mutation. *PLoS Genet*. PMID [23300461](https://pubmed.ncbi.nlm.nih.gov/23300461/)
- Xu P et al. (2013). BUBR1 recruits PP2A via the B56 family of targeting subunits to promote chromosome congression. *Biol Open*. PMID [23789096](https://pubmed.ncbi.nlm.nih.gov/23789096/)
- Chen S et al. (2024). A genomic mutational constraint map using variation in 76,156 human genomes. *Nature*. PMID [38057664](https://pubmed.ncbi.nlm.nih.gov/38057664/)
- Nakano Y et al. (2024). Update on Recommendations for Cancer Screening and Surveillance in Children with Genomic Instability Disorders. *Clin Cancer Res*. PMID [39264246](https://pubmed.ncbi.nlm.nih.gov/39264246/)

## Other sources

- ClinVar VCV000533901.9, NM_001211.6(BUB1B):c.2210T>G (p.Leu737Ter), germline classification pathogenic/likely pathogenic, review status "criteria provided, multiple submitters, no conflicts", condition "Mosaic variegated aneuploidy syndrome 1", last evaluated 2024-10-09, read via NCBI E-utilities 2026-10-24: https://www.ncbi.nlm.nih.gov/clinvar/variation/533901/

- ClinVar VCV004600147.1, NM_001211.6(BUB1B):c.3006T>A (p.Asn1002Lys), uncertain significance, single submitter, last evaluated 2025-09-19, read 2026-10-24: https://www.ncbi.nlm.nih.gov/clinvar/variation/4600147/. The c.3006T>G change carried by the child has no ClinVar record.

- Genomic positions (GRCh38 chr15:40209701 and chr15:40220612) match the ClinVar location fields read on 2026-10-24.

- gnomAD v4, GraphQL API, dataset `gnomad_r4`, queried 2026-10-24: 15-40209701-T-G has 115 alleles in 1,461,846 exome alleles and 5 in 152,174 genome alleles (the 7.9e-05 in the table is the exome frequency, 115 / 1,461,846); 15-40220612-T-G has 1 allele in 1,461,878 exome alleles and none in genomes. The gnomAD v4 reference is Chen et al. (2024), listed above.

- UniProt O60566 (BUB1B_HUMAN, reviewed entry, sequence version 3), read 2026-10-24: https://www.uniprot.org/uniprotkb/O60566

- Formal diagnostic cut-off for the share of aneuploid cells (section 1.1): [UNVERIFIED: no primary source established]. The "more than 25% of cells" figure is a typical value quoted in PMID [23300461](https://pubmed.ncbi.nlm.nih.gov/23300461/).

- Track 1 report of the same submission (identification of the two variants, exon-depth check, phase limit, further heterozygous variants): see the Track 1 upload of this submission.
