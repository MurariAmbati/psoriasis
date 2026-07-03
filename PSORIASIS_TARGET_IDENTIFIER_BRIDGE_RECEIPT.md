# Psoriasis Anduril RM Deep Discovery

Deep psoriasis discovery report for `anduril_rm`. This is a real-data input and execution-readiness ledger, not a scientific result report.

- Units: 650
- Input rows: 16250
- Matrix-bound executor-blocked rows: 4752
- Module abstention rows: 11300
- Contrast-unavailable abstention rows: 198
- Matrix-bound contrasts: 24
- Report digest: `7c87bc7bac5c02583841c40a33602b8f83a81f8843caf60593eccb0b18d012ea`

## Row States

| Row state | Rows |
| --- | ---: |
| `contrast_matrix_unavailable_abstention` | 198 |
| `matrix_bound_executor_blocked` | 4752 |
| `module_abstention_record` | 11300 |

## Top Missing Modalities

| Modality | Rows |
| --- | ---: |
| `mutation` | 3525 |
| `drug_response` | 2875 |
| `dependency` | 2775 |
| `chromatin` | 1650 |
| `imaging_pathology` | 850 |
| `subtype` | 775 |
| `spatial` | 775 |
| `liquid_biopsy` | 650 |
| `survival` | 575 |
| `methylation` | 575 |
| `proteomics` | 475 |

## Top Blockers

| Blocker | Rows |
| --- | ---: |
| scientific executor release is absent | 4950 |
| matrix input is bound but matrix materialization is disabled | 4752 |
| result envelope, null, falsifier, and certificate targets are absent | 4752 |
| missing modalities: mutation | 2025 |
| missing modalities: drug_response | 1650 |
| missing modalities: dependency | 1400 |
| missing modalities: chromatin | 750 |
| missing modalities: imaging_pathology | 500 |
| missing modalities: subtype | 425 |
| missing modalities: dependency, drug_response | 425 |
| missing modalities: spatial | 425 |
| missing modalities: liquid_biopsy, mutation | 375 |

## Matrix-Bound Contrasts

| Accession | Contrast | Rows | Left | Right | Matrix status |
| --- | --- | --- | --- | --- | --- |
| GSE117239 | lesional_vs_nonlesional | 198 | 240 | 84 | contrast_matrix_ready_direct_gsm |
| GSE117239 | pasi75_responder_vs_nonresponder | 198 | 231 | 93 | contrast_matrix_ready_direct_gsm |
| GSE121212 | lesional_vs_nonlesional | 198 | 55 | 54 | contrast_matrix_ready_processed_bridge |
| GSE121212 | lesional_vs_normal | 198 | 55 | 38 | contrast_matrix_ready_processed_bridge |
| GSE121212 | psoriasis_vs_atopic_dermatitis | 198 | 55 | 54 | contrast_matrix_ready_processed_bridge |
| GSE121212 | psoriasis_vs_healthy_or_normal | 198 | 55 | 38 | contrast_matrix_ready_processed_bridge |
| GSE13355 | lesional_vs_nonlesional | 198 | 58 | 58 | contrast_matrix_ready_direct_gsm |
| GSE13355 | lesional_vs_normal | 198 | 58 | 64 | contrast_matrix_ready_direct_gsm |
| GSE13355 | psoriasis_vs_healthy_or_normal | 198 | 116 | 64 | contrast_matrix_ready_direct_gsm |
| GSE14905 | lesional_vs_nonlesional | 198 | 33 | 28 | contrast_matrix_ready_direct_gsm |
| GSE14905 | lesional_vs_normal | 198 | 33 | 21 | contrast_matrix_ready_direct_gsm |
| GSE14905 | psoriasis_vs_healthy_or_normal | 198 | 61 | 21 | contrast_matrix_ready_direct_gsm |
| GSE30999 | lesional_vs_nonlesional | 198 | 85 | 85 | contrast_matrix_ready_direct_gsm |
| GSE34248 | lesional_vs_nonlesional | 198 | 14 | 14 | contrast_matrix_ready_direct_gsm |
| GSE41662 | lesional_vs_nonlesional | 198 | 24 | 24 | contrast_matrix_ready_direct_gsm |
| GSE53552 | baseline_or_predose_treatment_axis | 198 | 49 | 50 | contrast_matrix_ready_direct_gsm |
| GSE53552 | lesional_vs_nonlesional | 198 | 75 | 24 | contrast_matrix_ready_direct_gsm |
| GSE54456 | lesional_vs_normal | 198 | 92 | 82 | contrast_matrix_ready_processed_bridge |
| GSE54456 | psoriasis_vs_healthy_or_normal | 198 | 92 | 82 | contrast_matrix_ready_processed_bridge |
| GSE66511 | psoriasis_vs_healthy_or_normal | 198 | 24 | 12 | contrast_matrix_ready_processed_bridge |
| GSE78097 | lesional_vs_nonlesional | 198 | 27 | 6 | contrast_matrix_ready_direct_gsm |
| GSE78097 | mild_vs_severe_source_axis | 198 | 14 | 13 | contrast_matrix_ready_direct_gsm |
| GSE78097 | psoriasis_vs_healthy_or_normal | 198 | 27 | 6 | contrast_matrix_ready_direct_gsm |
| GSE85034 | lesional_vs_nonlesional | 198 | 29 | 29 | contrast_matrix_ready_direct_gsm |

## RM Readiness Detail

| Unit | Title | Bound | Abstain | Contrasts | Top missing |
| --- | --- | --- | --- | --- | --- |
| RM0001 | Matched-decoy manifold via model-X knockoffs for repression features | 0 | 25 | 0 | chromatin |
| RM0002 | Negative-control outcome calibration (proximal inference) for omics endpoints | 0 | 25 | 0 | survival |
| RM0003 | Cohort-blocked permutation null with exchangeability certification | 0 | 25 | 0 | mutation |
| RM0004 | Conditional knockoff FDR for genome-wide regulatory feature selection | 24 | 1 | 24 |  |
| RM0005 | LOCO transfer-gap estimator with a PAC-Bayes portability bound | 24 | 1 | 24 |  |
| RM0006 | Site-confounding variance decomposition (2) and leave-one-site-out collapse | 0 | 25 | 0 | imaging_pathology |
| RM0007 | Incremental-information bootstrap with C-index covariance correction | 0 | 25 | 0 | survival |
| RM0008 | Plain-baseline dominance test (DeLong + reclassification) as an earned-complexity gate | 0 | 25 | 0 | proteomics, subtype |
| RM0009 | Purity-deconfounding by instrumental residualization | 24 | 1 | 24 |  |
| RM0010 | Transfer-preserving batch harmonization with known-marker recovery gate | 24 | 1 | 24 |  |
| RM0011 | Patient-level replication graph and donor-reuse deflation | 0 | 25 | 0 | chromatin |
| RM0012 | Calibration manifold and decision-curve net-benefit certification | 24 | 1 | 24 |  |
| RM0013 | Power and event-count audit separating certified from underpowered negatives | 24 | 1 | 24 |  |
| RM0014 | Context-of-use type system: a biomarker-category lattice | 24 | 1 | 24 |  |
| RM0015 | Polyhedral selective inference for post-selection valid p-values | 24 | 1 | 24 |  |
| RM0016 | Anytime-valid e-values for streaming and accumulating cohorts | 24 | 1 | 24 |  |
| RM0017 | Conformal selective prediction with distribution-free coverage | 24 | 1 | 24 |  |
| RM0018 | Hierarchical FDR across the experiment tree | 24 | 1 | 24 |  |
| RM0019 | Specification-curve / multiverse analysis engine | 24 | 1 | 24 |  |
| RM0020 | Decoy-survival ROC: feature-versus-its-own-decoy discrimination | 0 | 25 | 0 | survival |
| RM0021 | Mendelian-randomization identifiability for methylationexpressionstate | 0 | 25 | 0 | methylation, mutation |
| RM0022 | Front-door adjustment through chromatin mediators | 0 | 25 | 0 | chromatin, mutation |
| RM0023 | Sensitivity-to-unmeasured-confounding battery (E-value + Rosenbaum bounds) | 24 | 1 | 24 |  |
| RM0024 | Transportability calculus across cohorts via selection diagrams | 24 | 1 | 24 |  |
| RM0025 | Positivity/overlap diagnostics with principled abstain | 0 | 25 | 0 | drug_response |
| RM0026 | Double-negative-control (proximal g-computation) treatment effects | 0 | 25 | 0 | drug_response |
| RM0027 | Conditional permutation importance without correlation leakage | 0 | 25 | 0 | mutation |
| RM0028 | Stability selection across subsamples with per-feature error control | 24 | 1 | 24 |  |
| RM0029 | Reproducibility (IDR) for peak and feature calls | 24 | 1 | 24 |  |
| RM0030 | Double machine learning with cross-fitting for nuisance orthogonalization | 0 | 25 | 0 | drug_response |
| RM0031 | Targeted minimum-loss estimation (TMLE) wrapper for any plug-in feature | 0 | 25 | 0 | drug_response |
| RM0032 | Influence-function variance for arbitrary plug-in features | 24 | 1 | 24 |  |
| RM0033 | Whole-pipeline bootstrap (uncertainty of the analysis itself) | 24 | 1 | 24 |  |
| RM0034 | Target-leakage graph scanner | 24 | 1 | 24 |  |
| RM0035 | Nested cross-validation for unbiased performance with selection | 24 | 1 | 24 |  |
| RM0036 | Temporal calibration-drift monitor | 24 | 1 | 24 |  |
| RM0037 | Fairness/subgroup calibration audit as a clinical-safety surface | 24 | 1 | 24 |  |
| RM0038 | Under-measurement as a first-class predictive axis | 24 | 1 | 24 |  |
| RM0039 | Collider/selection-bias detector in cohort assembly | 0 | 25 | 0 | chromatin |
| RM0040 | Immortal-time-bias guard for treatment/exposure cohorts | 0 | 25 | 0 | drug_response |
| RM0041 | Rotation/self-contained gene-set null for pathway claims | 24 | 1 | 24 |  |
| RM0042 | Empirical-Bayes / James-Stein shrinkage for multi-subgroup effects | 24 | 1 | 24 |  |
| RM0043 | Replication Bayes factor and prior-predictive checking | 24 | 1 | 24 |  |
| RM0044 | Sign-consistency random-effects meta with Cochran-Q | 24 | 1 | 24 |  |
| RM0045 | Heterogeneity-of-effect (I2/2) cartography | 24 | 1 | 24 |  |
| RM0046 | Locked-panel held-out certification protocol | 24 | 1 | 24 |  |
| RM0047 | Adversarial covariate-shift stress test | 24 | 1 | 24 |  |
| RM0048 | Hash-locked data-version provenance and exact reproducibility | 24 | 1 | 24 |  |
| RM0049 | Honest-funnel ledger (experiments replicated over-identified stable) | 24 | 1 | 24 |  |
| RM0050 | Evidence-ladder auto-tiering classifier (the claim firewall) | 24 | 1 | 24 |  |
| RM0051 | Mimic-adversarial diagnostic classifier with hard-negative mining | 0 | 25 | 0 | imaging_pathology |
| RM0052 | Methylation nearest-centroid classifier with calibrated rejection | 0 | 25 | 0 | liquid_biopsy, methylation, mutation |
| RM0053 | Cross-platform lineage-axis transfer (cell-of-origin generalized) | 0 | 25 | 0 | subtype |
| RM0054 | Within-subtype residual-state splitter | 0 | 25 | 0 | subtype |
| RM0055 | Genotypephenotype convergence map (many-to-one) | 0 | 25 | 0 | chromatin, mutation |
| RM0056 | Composite/admixed-subtype topic model | 0 | 25 | 0 | subtype |
| RM0057 | Immunoglobulin/TCR clonality from bulk and single-cell RNA | 0 | 25 | 0 | mutation |
| RM0058 | Low-purity diagnostic rescue via purity-aware deconvolution | 24 | 1 | 24 |  |
| RM0059 | Digital-histology triage with conformal abstain | 0 | 25 | 0 | imaging_pathology |
| RM0060 | cfDNA-methylation tissue-of-origin and class classifier | 0 | 25 | 0 | liquid_biopsy, methylation, mutation |
| RM0061 | Ambiguous-case entropy router | 0 | 25 | 0 | mutation |
| RM0062 | Entity-boundary geometry and gray-zone cartography | 0 | 25 | 0 | mutation |
| RM0063 | Morphologymolecular correspondence (vision-omics alignment) | 0 | 25 | 0 | imaging_pathology |
| RM0064 | Blinded expert-concordance diagnostic protocol | 0 | 25 | 0 | imaging_pathology |
| RM0065 | Taxonomy-aware hierarchical diagnostic classifier | 0 | 25 | 0 | subtype |
| RM0066 | Reactive-versus-malignant discriminator with benign-mimic priors | 0 | 25 | 0 | mutation |
| RM0067 | Transformation-versus-de-novo discriminator | 0 | 25 | 0 | mutation |
| RM0068 | Site-defined-variant classifier (CNS/testicular/cutaneous/etc.) | 0 | 25 | 0 | mutation |
| RM0069 | Virus-status-aware diagnostic stratification | 24 | 1 | 24 |  |
| RM0070 | Open-set diagnosis with novel-entity detection | 24 | 1 | 24 |  |
| RM0071 | Few-shot diagnosis for rare entities via prototype networks | 24 | 1 | 24 |  |
| RM0072 | Diagnostic uncertainty decomposition (aleatoric vs epistemic) | 24 | 1 | 24 |  |
| RM0073 | Multi-omics factor endotype (sparse MOFA+) | 0 | 25 | 0 | subtype |
| RM0074 | Endotype modality-dropout stability | 0 | 25 | 0 | subtype |
| RM0075 | Dependency-anchored endotype | 0 | 25 | 0 | dependency, subtype |
| RM0076 | Reference-based bulk state-mixture deconvolution | 24 | 1 | 24 |  |
| RM0077 | Reference-free archetypal analysis of states | 24 | 1 | 24 |  |
| RM0078 | Rare malignant-state (minority population) detector | 24 | 1 | 24 |  |
| RM0079 | Inter-lesion discordance metric | 0 | 25 | 0 | liquid_biopsy, mutation |
| RM0080 | Subclone-to-state coupling (joint single-cell DNA-RNA/ATAC) | 24 | 1 | 24 |  |

The JSON companion contains all 650 rm rows with gates, routes, blockers, bound contrasts, and modality gaps.

## Release Boundary

- batch_or_platform_guard_receipts
- downstream_envelope_binding_receipts
- scientific_executor_release_ledger
- per-unit null_falsifier_certificate_vectors
