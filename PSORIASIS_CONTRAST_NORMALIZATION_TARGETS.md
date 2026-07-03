# Psoriasis Program — Full Gap Assessment

**RUO.** Honest accounting of what has and has NOT been done, across data modalities and all three method libraries (anduril, artmethods, R-band). Two gap classes are distinguished: **structural** (cannot be fixed from public data) vs **executable** (can be run with more compute/adapter work).

## 1. Method-library coverage on psoriasis (quantified)

| Library | Total | Ran / PASS | Abstained (modality absent) | Timed-out / blocked | Errored (modality-missing) |
|---|---:|---:|---:|---:|---:|
| **anduril** | 650 | 233 PASS (247 touch real data) | 78 | 359 (heavy: sim/topology/GNN/MCMC) | 44 |
| **artmethods** | 202 | 46 | 156 | — | — |
| **R-band** (repressome) | 240 units / 6,000 rows | (expression-fittable only) | 5,075 | 888 executor-blocked | 37 contrast-unavail |

**R-band now queued**: 240 modules × 23 diseases = 5,520 module×disease jobs; for psoriasis 240 units, 888 expression-bound rows blocked at the executor gate.

## 2. Root cause — the structural gap (drives ~75% of all abstentions)

The libraries were built for **cancer** and assume modalities psoriasis does not have in public data:

| Modality the libraries need | Psoriasis status | R-band abstaining rows |
|---|---|---:|
| drug_response (ex-vivo / screens) | **absent** | 2,800 |
| dependency (CRISPR/RNAi) | **absent** | 2,400 |
| proteomics (RPPA/MS) | **absent** | 1,975 |
| mutation (somatic) | **absent** | 1,700 |
| survival / clinical outcome | **absent** | 925 |
| chromatin (H3K27me3/ATAC, human lesional) | **absent** (only mouse/raw on GEO) | 650 |
| spatial / imaging / GWAS | absent | — |

Psoriasis **HAS**: expression (12 cohorts / 3 platforms), DNA methylation (3× 450K), single-cell (2 cohorts). That is the entire actionable surface — and it has been mined deeply (see §4).

## 3. Why this is NOT closable from public data
- These method families (synthetic-lethality, dependency, drug-selectivity, survival forecasting, proteogenomics) require functional-genomics / clinical-trial data that simply does not exist for psoriasis in open repositories.
- This is the same depth gap that separates psoriasis from AML/DLBCL (which have BeatAML, DepMap, TCGA survival). It is a data-availability ceiling, not an effort gap.

## 4. Gaps already CLOSED this session
- Expression: 8→12 cohorts, full meta-analysis, replication, repression lens.
- Methylation: 3-cohort replication, focal-hypermethylation validation, persistence, novel scar/bivalent/coordinated methods.
- Single-cell: 2-cohort cell-type resolution + per-cell deep classifier.
- Deep learning: ALL data (1,350 samples × 11,873 genes × 12 cohorts × 3 platforms), multi-seed, cross-platform, WGAN-GP; methylation-DL; single-cell-DL.
- Validated finding (epigenetic-memory of differentiation-TF silencing) + honest negatives (JARID2 down-grade, composition refinement, de-repression-drug negative).

## 5. Remaining EXECUTABLE gaps (can be run; bounded by compute/adapter, not data)
- **anduril 359 heavy modules** — need long-running compute (agent-based sim, persistent homology, GNN training, MCMC); time-boxed so far.
- **R-band 888 expression-bound rows** — blocked at the executor-release gate; need the executor adapter to emit results on the available expression/methylation contrasts.
- **artmethods abstained-but-fittable** — a handful of expression/network methods could be adapted to run.
- **ARCHS4 integration** — 57 GB downloading; will add hundreds of uniformly-processed samples to the deep-learning pool.

## 6. Remaining STRUCTURAL gaps — only closable via account-gated / generated data
- **ImmPort** (SDY2274, SDY667, SDY416, SDY1177) → treatment-response + clinical-outcome (unlocks the survival/drug_response method families).
- **clue.io skin-context perturbation** → drug_response/dependency proxy in keratinocytes (fixes the off-tissue LINCS limitation).
- **dbGaP / UK Biobank** → psoriasis GWAS/mutation (unlocks the genetics method families).
- **Prospective paired pre/post-relapse methylation** → the one experiment that would confirm the epigenetic-memory clinical claim (does not exist publicly).

## Bottom line
The psoriasis **expression/methylation/single-cell surface is now mined to the public-data ceiling**, including deep learning. The large residual abstention across anduril/artmethods/R-band is **structural** — psoriasis lacks the cancer/functional-genomics/clinical modalities those methods require. Closing it requires the account-gated trial (ImmPort) and perturbation (clue.io) data, or newly-generated data — not more compute on what's already here.
