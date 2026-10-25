# Zero drug counts in drug-target databases

## Claim as stated

Counts from drug-target and knowledge-graph resources show that no approved drug acts within one network step of BubR1, the spindle checkpoint protein encoded by *BUB1B*. A knowledge graph is a network in which genes, drugs and diseases are nodes joined by edges. The counts include 464 edges and zero drug edges in a biomedical knowledge graph, 0 of 35 spindle-checkpoint and anaphase-promoting complex/cyclosome (APC/C) proteins clinically drugged, and a 35-protein druggability map.

## Evidence for

- The deposited chemistry record for BubR1 holds 24 activity values over 15 molecules, best 9.67 µM, one approved drug (ceritinib) at 13 µM ([residue atlas](../residue-atlas.md), findings 3 and 4).

- A census of 16 cell-cycle nodes, namely cyclins, cyclin-dependent kinases (CDK), APC/C and phosphatases, found only inhibitors where an agent exists ([cell-cycle map](../cell-cycle-map.md), finding 6).

## Evidence against

1. **The count needs a base rate.** At the genome-wide rate of clinically drugged proteins (the Pharos Tclin class), the chance of zero drugged proteins among 35 random ones is about 0.29, which implies a rate of 3.5% (1 − 0.29^(1/35)) [UNVERIFIED: the 0.29 is taken from the project notes and not re-derived].

2. **A link-prediction model on a knowledge graph tied a drug-popularity baseline.** On PrimeKG (4.05 million edges; PMID [36732524](https://pubmed.ncbi.nlm.nih.gov/36732524/); 232 held-out diseases), mean reciprocal rank (the average of 1 divided by the rank of the first correct drug) was 0.0657 against 0.0658 (this report's analysis of a public graph). The model did worse in diseases with at most 5 gene edges (0.019 against 0.048). For this disease the shared-gene list equals the popularity list (corticosteroids). The method failed its pre-registered positive control.

3. **Only network proximity passed the pre-registered conditions for recovering known successes.** Recall at 20 (the share of known successes ranked in the top 20) was 0.111 on 45 label-read successes in 27 monogenic diseases (95% interval 0.02 to 0.21), and a signed two-hop search nominated 2 of 45. A post hoc audit found that the proximity hits were all direct neighbours of the causal gene and that recall fell to 0.044 on a different network.

4. **A census of the claim "no cyclin has an agent" showed it false** for cyclin D1 (palbociclib is approved against the complex; [cell-cycle map](../cell-cycle-map.md), Verification).

5. **A two-sided test of the claim that agents acting in the needed direction do not exist** returned 1 of 31 nodes with a fidelity readout in both directions, so it is inconclusive.

## Conclusion

A zero count shows the absence of a measured drug in the databases. A candidate can exist where no measured drug is deposited.

## Same weakness in this report

The report's own census used a gene list chosen without a pre-registered completeness rule, which is how the cyclin D1 counter-example was missed. The report treats the count as a statement about the databases.

## References

- Chandak P et al. (2023). Building a knowledge graph to enable precision medicine. *Sci Data*. PMID [36732524](https://pubmed.ncbi.nlm.nih.gov/36732524/)

## Other sources

- PrimeKG (4,050,249 relationships), the public biomedical knowledge graph used for the link-prediction test; Pharos target development levels (https://pharos.nih.gov); ChEMBL target CHEMBL4295998 (BUB1B), ChEMBL 37, queried 2026-10-24; Open Targets Platform v26.9.0.

- The link-prediction, recall and base-rate figures in items 1 to 3 are this report's analyses of public data [UNVERIFIED: the analyses are not published with this report].

- The zero-count claims are quoted from the proposals' public repositories and cited by claim only.
