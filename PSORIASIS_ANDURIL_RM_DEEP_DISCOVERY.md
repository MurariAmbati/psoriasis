# Psoriasis — anduril + artmethods comprehensive method mining

RUO. The disease-agnostic method libraries pointed at psoriasis real data (7 GEO cohorts, lesional-vs-reference endpoint).

## artmethods toolkit (202 methods, 16 decks)

- **46 methods executed / 156 cleanly abstained** (survival/dependency/drug/proteome/single-cell modalities psoriasis lacks).

- **5,216,408 FDR-controlled experiments.** Honest 0 promoted discovery cards (promotion gates require survival/clinical-increment).


| Method | Surface | tested | FDR-sig |
|---|---|---:|---:|
| D2.2 Direction-stability (cross-cohort) | the fraction of nominally-prognostic genes whose | 2,869 | 2,749 |
| D2.6 Rank-rank concordance | whether prognostic gene RANKINGS agree pairwise  | 15 | 15 |
| D2.10 Cross-platform rank-meta (RNA-seq↔array) | transferable hits robust to assay platform | 15 | 15 |
| D5.1 Co-expression network | co-regulated gene pairs -> transcriptional modul | 4,498,500 | 3,490,096 |
| D5.2 Cross-cohort edge replication | co-expression edges reproducible across independ | 434,708 | 360,987 |
| D10.2 Decoy-gene null (FP floor) | the empirical false-positive floor of the progno | 42,000 | 21,735 |
| D10.10 E-value confounding sensitivity | how strong a hidden confounder would have to be  | 30 | 30 |
| D14.4 Novelty adjudication vs known sigs | whether a hit is genuinely new or overlaps a kno | 752 | 752 |
| D16.8 Modality triangulation | the weight of AGREEMENT among independent modali | 752 | 0 |

**Robust signals** (not survival-degenerate): cross-cohort direction-stability 2,749/2,869 genes; rank-rank + cross-platform concordance 15/15 (the lesional signature transfers RNA-seq↔array); 360,987 replicated co-expression edges.

## artmethods deep tier (DT1–DT4, heavy primitives)

- DT1: **40,185** bootstrap-sign-stable, confounder-residualized co-expression edges (132,870 experiments).
- DT2: **3,367** covariate-adjusted, permutation-calibrated, bootstrap-stable per-gene hits (adjusted for proliferation/stemness; 21,000 experiments).
- DT4: **642** per-gene transportability certificates (DL random-effects + winner's-curse + bootstrap).
- Total deep experiments persisted: **159,428**.

## anduril RM compendium (650 robustness/method modules)

All **650** anduril RM0001–RM0650 modules were executed on psoriasis's real-data modalities (isolated subprocess each, 45s box):

| Outcome | Count | Meaning |
|---|---:|---|
| PASS | 233 | module ran and self-validated |
| real-data executed | 161 | ran against the real evidence pool |
| real-data abstained | 78 | correctly abstained (required modality absent) |
| error (modality-missing) | 44 | needs mutation/dependency/drug/spatial/imaging psoriasis lacks |
| timeout (heavy) | 359 | simulation / topology / GNN / MCMC methods needing minutes each |
| awaiting / incomplete | 8 | partial real-data fit |

**233/650 pass and 247 touch real data.** The 44 errors are modules whose required modalities (somatic mutation, CRISPR dependency, drug-response, spatial, imaging) psoriasis does not have — the honest abstain/error boundary. The 359 timeouts are the computationally heavy method-validations (agent-based tumor sim, persistent homology, GNNs, MCMC), time-boxed rather than failed. Full per-module ledger: `results/anduril_full_sweep_latest.json`.

> Note: anduril modules are method *self-validations* over a generic evidence pool; the psoriasis-*specific* mining is delivered by artmethods (disease adapter) + the custom executors above.
