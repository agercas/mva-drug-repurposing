# Hypotheses for BUB1B-related mosaic variegated aneuploidy

**"Rare Disease, Real Kid" MVA Hackathon 2026**

This report proposes testable hypotheses for a child with mosaic variegated aneuploidy (MVA), a recessive condition in which cells carry varying numbers of chromosomes. Two variants in *BUB1B*, the gene for the spindle checkpoint protein BubR1, are the proposed cause of the condition in this child: a stop-gain (likely pathogenic) and a missense change (a variant of uncertain significance). Which copy of the gene carries each is undetermined, and the report treats them as compound heterozygous. Every hypothesis names a mechanism, the evidence for and against it, and the experiment that would confirm or stop it. The hypotheses are for confirmation in an accredited laboratory, and clinical decisions rest with the treating team ([disclaimer](07-disclaimer-and-ai-use.md)).

## Workstreams

| Workstream | Subject | Section |
|---|---|---|
| Approved drugs | Three approved or widely available agents with a mechanistic reason to affect the BubR1 pathway, each with a laboratory test | [3](03-approved-drugs/README.md) |
| Non-approved therapies | Two gene-level routes, ex vivo prime editing and lentiviral add-back, each with a feasibility estimate | [4](04-non-approved-therapies/README.md) |

## Inclusion rule

A candidate has a card when four conditions hold: its mechanism chain starts from the two variants; its safety-screen flags (section 3) are recorded on the card; at least one step of the chain has a result in a related disease or a model system; and a cell-based assay with a written stopping criterion can falsify it. Gates 1 and 2 disqualify a candidate in the screen as written. Where a card records a flag at those gates (the N-acetylcysteine card, and both section 4 routes), the report states the flag and keeps the candidate as a hypothesis for laboratory test without arguing the flag away; both section 4 routes also have an open gate 4 (cancer direction). The appendix assesses alternative approaches to the candidates in sections 3 and 4.

## No lead candidate

The report names no lead hypothesis and no lead molecule. The evidence is insufficient to rank one candidate above the others, for three reasons:

- The residual activity of the missense allele (the copy with a single amino-acid change) is unmeasured ([section 1.7](01-disease-and-case.md#17-unmeasured-quantities-that-bear-on-every-candidate)).
- One research group reports the best-developed mechanism ([section 2.2](02-reported-research.md#22-authorship-and-independent-groups)).
- No candidate has human efficacy data in MVA ([section 2.8](02-reported-research.md#28-clinical-and-preclinical-data)).

A comparison table closes sections 3 and 4.

## Contents

| File | Content |
|---|---|
| [1. Disease and case](01-disease-and-case.md) | MVA, *BUB1B*, the two variants, the mechanism, the further genetic findings |
| [2. Reported research](02-reported-research.md) | Paper counts by topic, independent groups per claim, findings checked against full text, open mechanistic questions |
| [3. Approved drugs with mechanistic hypotheses](03-approved-drugs/README.md) | Registry searches, screening criteria, three candidate cards, comparison |
| [4. Non-approved therapies with hypotheses](04-non-approved-therapies/README.md) | Feasibility frame, two candidate cards, comparison, conditioning and malignancy precedents |
| [5. Computational findings](05-computational-findings.md) | Structure, folding, stability and quantitative-model results with their controls; shared experimental platform; generalisation |
| [6. References and tools](06-references-and-tools.md) | Databases, programming interfaces, software and models used |
| [7. Disclaimer and AI-use disclosure](07-disclaimer-and-ai-use.md) | Disclaimer, AI assistance, licence |
| [Appendix](appendix/README.md) | Error-free division estimate, pathogenicity prediction, three supporting analyses, ten alternative approaches assessed |

## Candidates

Each candidate has one card with nine fields: Candidate, Hypothesis, Delivery and exposure, Evidence for, Evidence against, Safety, Expected effect, Test and Outcome if confirmed.

| Candidate | Status | Acts on | Section |
|---|---|---|---|
| [NAD+ precursors](03-approved-drugs/nad-precursors.md) | Approved or widely available | Acetylation-controlled turnover of BubR1 | 3 |
| [IL-1 blockade with anakinra](03-approved-drugs/il1-blockade.md) | Approved | The inflammatory secretome of aneuploid cells | 3 |
| [N-acetylcysteine and ascorbate](03-approved-drugs/n-acetylcysteine.md) | Approved or widely available | Oxidative stress at the kinetochore | 3 |
| [Ex vivo prime-editing reversion of the stop allele](04-non-approved-therapies/prime-editing-reversion.md) | Investigational | The stop allele, rewritten to wild type in blood stem cells | 4 |
| [Ex vivo lentiviral add-back of BUB1B](04-non-approved-therapies/lentiviral-add-back.md) | Investigational | A working copy of the gene added to blood stem cells | 4 |

## Licence

Submissions are released under CC BY 4.0 (LICENSE), as the competition rules require. The dataset keeps its own terms, which prohibit redistribution.
