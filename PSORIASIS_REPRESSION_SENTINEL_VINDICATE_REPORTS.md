# Psoriasis R-Band Deep Discovery

Deep psoriasis discovery report for `rband_module`. This is a real-data input and execution-readiness ledger, not a scientific result report.

- Units: 240
- Input rows: 6000
- Matrix-bound executor-blocked rows: 888
- Module abstention rows: 5075
- Contrast-unavailable abstention rows: 37
- Matrix-bound contrasts: 24
- Report digest: `6e9396c847a7f1fc9e5f42d76391a9ba564d16d07a7595a1ce6f04353d1ac0bb`

## Row States

| Row state | Rows |
| --- | ---: |
| `contrast_matrix_unavailable_abstention` | 37 |
| `matrix_bound_executor_blocked` | 888 |
| `module_abstention_record` | 5075 |

## Top Missing Modalities

| Modality | Rows |
| --- | ---: |
| `drug_response` | 2800 |
| `dependency` | 2400 |
| `proteomics` | 1975 |
| `mutation` | 1700 |
| `survival` | 925 |
| `chromatin` | 650 |
| `methylation` | 300 |

## Top Blockers

| Blocker | Rows |
| --- | ---: |
| scientific executor release is absent | 925 |
| matrix input is bound but matrix materialization is disabled | 888 |
| result envelope, null, falsifier, and certificate targets are absent | 888 |
| missing modalities: drug_response | 825 |
| missing modalities: dependency, proteomics | 500 |
| missing modalities: drug_response, survival | 475 |
| missing modalities: dependency, drug_response | 350 |
| missing modalities: proteomics | 325 |
| missing modalities: dependency, drug_response, proteomics | 275 |
| missing modalities: chromatin, dependency, mutation | 275 |
| missing modalities: dependency, mutation, proteomics | 250 |
| missing modalities: mutation, proteomics | 250 |

## Matrix-Bound Contrasts

| Accession | Contrast | Rows | Left | Right | Matrix status |
| --- | --- | --- | --- | --- | --- |
| GSE117239 | lesional_vs_nonlesional | 37 | 240 | 84 | contrast_matrix_ready_direct_gsm |
| GSE117239 | pasi75_responder_vs_nonresponder | 37 | 231 | 93 | contrast_matrix_ready_direct_gsm |
| GSE121212 | lesional_vs_nonlesional | 37 | 55 | 54 | contrast_matrix_ready_processed_bridge |
| GSE121212 | lesional_vs_normal | 37 | 55 | 38 | contrast_matrix_ready_processed_bridge |
| GSE121212 | psoriasis_vs_atopic_dermatitis | 37 | 55 | 54 | contrast_matrix_ready_processed_bridge |
| GSE121212 | psoriasis_vs_healthy_or_normal | 37 | 55 | 38 | contrast_matrix_ready_processed_bridge |
| GSE13355 | lesional_vs_nonlesional | 37 | 58 | 58 | contrast_matrix_ready_direct_gsm |
| GSE13355 | lesional_vs_normal | 37 | 58 | 64 | contrast_matrix_ready_direct_gsm |
| GSE13355 | psoriasis_vs_healthy_or_normal | 37 | 116 | 64 | contrast_matrix_ready_direct_gsm |
| GSE14905 | lesional_vs_nonlesional | 37 | 33 | 28 | contrast_matrix_ready_direct_gsm |
| GSE14905 | lesional_vs_normal | 37 | 33 | 21 | contrast_matrix_ready_direct_gsm |
| GSE14905 | psoriasis_vs_healthy_or_normal | 37 | 61 | 21 | contrast_matrix_ready_direct_gsm |
| GSE30999 | lesional_vs_nonlesional | 37 | 85 | 85 | contrast_matrix_ready_direct_gsm |
| GSE34248 | lesional_vs_nonlesional | 37 | 14 | 14 | contrast_matrix_ready_direct_gsm |
| GSE41662 | lesional_vs_nonlesional | 37 | 24 | 24 | contrast_matrix_ready_direct_gsm |
| GSE53552 | baseline_or_predose_treatment_axis | 37 | 49 | 50 | contrast_matrix_ready_direct_gsm |
| GSE53552 | lesional_vs_nonlesional | 37 | 75 | 24 | contrast_matrix_ready_direct_gsm |
| GSE54456 | lesional_vs_normal | 37 | 92 | 82 | contrast_matrix_ready_processed_bridge |
| GSE54456 | psoriasis_vs_healthy_or_normal | 37 | 92 | 82 | contrast_matrix_ready_processed_bridge |
| GSE66511 | psoriasis_vs_healthy_or_normal | 37 | 24 | 12 | contrast_matrix_ready_processed_bridge |
| GSE78097 | lesional_vs_nonlesional | 37 | 27 | 6 | contrast_matrix_ready_direct_gsm |
| GSE78097 | mild_vs_severe_source_axis | 37 | 14 | 13 | contrast_matrix_ready_direct_gsm |
| GSE78097 | psoriasis_vs_healthy_or_normal | 37 | 27 | 6 | contrast_matrix_ready_direct_gsm |
| GSE85034 | lesional_vs_nonlesional | 37 | 29 | 29 | contrast_matrix_ready_direct_gsm |

## R-band module Readiness Detail

| Unit | Title | Bound | Abstain | Contrasts | Top missing |
| --- | --- | --- | --- | --- | --- |
| AX00 | RepressionOperator contract | 24 | 1 | 24 |  |
| AX01 | DiseaseState object | 24 | 1 | 24 |  |
| AX02 | HealthyReference manifold | 24 | 1 | 24 |  |
| AX03 | RepressionHandle object | 0 | 25 | 0 | chromatin, proteomics |
| AX04 | InterventionObject | 0 | 25 | 0 | drug_response |
| AX05 | RepressionTrajectory | 0 | 25 | 0 | survival |
| AX06 | Vector RepressionCertificate | 24 | 1 | 24 |  |
| AX07 | Support and uncertainty contract | 24 | 1 | 24 |  |
| AX08 | Modality eligibility compiler | 0 | 25 | 0 | proteomics |
| AX09 | RepressionBench task schema | 0 | 25 | 0 | drug_response |
| CC00 | Repression-operator embedding | 0 | 25 | 0 | dependency, drug_response |
| CC01 | Cross-disease state equivalence | 0 | 25 | 0 | drug_response |
| CC02 | Conserved/inverted/private classifier | 24 | 1 | 24 |  |
| CC03 | Hierarchical transfer model | 24 | 1 | 24 |  |
| CC04 | Rare-disease borrowing gate | 24 | 1 | 24 |  |
| CC05 | Mechanism-convergence detector | 24 | 1 | 24 |  |
| CC06 | Cross-modality intervention transfer | 0 | 25 | 0 | drug_response |
| CC07 | Boundary-condition mapper | 0 | 25 | 0 | drug_response, mutation |
| CC08 | Repression periodic table | 24 | 1 | 24 |  |
| CC09 | Pan-disease atlas certificate | 24 | 1 | 24 |  |
| CF00 | Target structural ensemble | 0 | 25 | 0 | dependency, drug_response, mutation |
| CF01 | Pocket, cryptic-pocket and allostery map | 0 | 25 | 0 | dependency, drug_response, mutation |
| CF02 | Seed, fragment and pharmacophore compiler | 0 | 25 | 0 | dependency, drug_response |
| CF03 | Generative molecule design | 0 | 25 | 0 | dependency, drug_response |
| CF04 | Consensus docking | 0 | 25 | 0 | dependency, drug_response |
| CF05 | Structure/affinity consensus | 0 | 25 | 0 | dependency, drug_response, proteomics |
| CF06 | Physics refinement and stability | 0 | 25 | 0 | dependency, drug_response |
| CF07 | Selectivity and off-target panel | 0 | 25 | 0 | dependency, drug_response |
| CF08 | Developability and synthesis screen | 0 | 25 | 0 | dependency, drug_response |
| CF09 | Closed-loop molecule adjudicator | 0 | 25 | 0 | dependency, drug_response |
| CI00 | Phosphosignaling network compiler | 0 | 25 | 0 | dependency, mutation, proteomics |
| CI01 | Latent kinase/phosphatase activity | 0 | 25 | 0 | dependency, mutation, proteomics |
| CI02 | Feedback-motif detector | 0 | 25 | 0 | dependency, mutation, proteomics |
| CI03 | Dynamic signaling state-space | 0 | 25 | 0 | dependency, drug_response, mutation, proteomics |
| CI04 | Pathway-crosstalk hypergraph | 0 | 25 | 0 | dependency, mutation, proteomics |
| CI05 | Causal intervention simulator | 0 | 25 | 0 | dependency, mutation, proteomics |
| CI06 | Single-cell signaling heterogeneity | 0 | 25 | 0 | dependency, mutation, proteomics |
| CI07 | Rescue and compensation predictor | 0 | 25 | 0 | dependency, drug_response, mutation, proteomics |
| CI08 | Minimal control-point finder | 0 | 25 | 0 | dependency, mutation, proteomics |
| CI09 | Circuit repression certificate | 0 | 25 | 0 | dependency, mutation, proteomics |
| CT00 | Disease-program decomposition | 0 | 25 | 0 | chromatin, dependency, mutation |
| CT01 | Signed regulatory graph | 0 | 25 | 0 | chromatin, dependency, mutation |
| CT02 | Drivermaintenance hierarchy | 0 | 25 | 0 | dependency, drug_response, mutation, survival |
| CT03 | Feedback and compensation compiler | 0 | 25 | 0 | dependency, drug_response, mutation |
| CT04 | Redundancy and synthetic-repression map | 0 | 25 | 0 | dependency, mutation |
| CT05 | Repression-handle atlas | 0 | 25 | 0 | dependency, mutation |
| CT06 | Normal-tissue contrast | 0 | 25 | 0 | dependency, mutation |
| CT07 | Context stratifier | 0 | 25 | 0 | dependency, drug_response, mutation |
| CT08 | Cross-disease repression motifs | 0 | 25 | 0 | dependency, mutation |
| CT09 | Causal confidence and rival explanations | 0 | 25 | 0 | dependency, mutation |
| CX00 | Rival-hypothesis graph | 0 | 25 | 0 | drug_response |
| CX01 | Experiment grammar | 0 | 25 | 0 | dependency |
| CX02 | Active-learning selector | 24 | 1 | 24 |  |
| CX03 | Dataset/modality acquisition planner | 24 | 1 | 24 |  |
| CX04 | Perturbation-panel optimizer | 0 | 25 | 0 | dependency |
| CX05 | Model-system selector | 24 | 1 | 24 |  |
| CX06 | Readout and power compiler | 24 | 1 | 24 |  |
| CX07 | Randomization, blocking and blinding | 24 | 1 | 24 |  |
| CX08 | Preregistration and analysis lock | 24 | 1 | 24 |  |
| CX09 | Outcome adjudicator | 24 | 1 | 24 |  |
| DG00 | Inhibition-versus-degradation triage | 0 | 25 | 0 | dependency, drug_response, proteomics |
| DG01 | E3 ligase context atlas | 0 | 25 | 0 | dependency, drug_response, proteomics |
| DG02 | Warheadligaselinker object compiler | 0 | 25 | 0 | dependency, drug_response, proteomics |
| DG03 | Linker generation and conformer enumeration | 0 | 25 | 0 | dependency, drug_response, proteomics |
| DG04 | Ternary-complex structure generation | 0 | 25 | 0 | dependency, drug_response, proteomics |
| DG05 | Cooperativity and ensemble scoring | 0 | 25 | 0 | dependency, drug_response, proteomics |
| DG06 | Degradation kinetics model | 0 | 25 | 0 | dependency, drug_response, proteomics |
| DG07 | Molecular-glue opportunity scanner | 0 | 25 | 0 | dependency, drug_response, proteomics |
| DG08 | Cell exposure and developability | 0 | 25 | 0 | dependency, drug_response, proteomics |
| DG09 | Degrader resistance, safety and certificate | 0 | 25 | 0 | dependency, drug_response, mutation, proteomics |
| EG00 | Chromatin-state compiler | 0 | 25 | 0 | chromatin, methylation, mutation |
| EG01 | Enhancerpromoter regulatory graph | 0 | 25 | 0 | chromatin, dependency, methylation, mutation |
| EG02 | 3D-genome repression architecture | 0 | 25 | 0 | chromatin, methylation, mutation |
| EG03 | DNA-methylation dynamics | 0 | 25 | 0 | chromatin, drug_response, methylation, mutation |
| EG04 | Histone and repressive-machinery model | 0 | 25 | 0 | chromatin, dependency, methylation, mutation |
| EG05 | Poised and bivalent-state detector | 0 | 25 | 0 | chromatin, methylation, mutation, survival |
| EG06 | Epitranscriptomic repression layer | 0 | 25 | 0 | chromatin, dependency, methylation, mutation |
| EG07 | Chromatin perturbation-response model | 0 | 25 | 0 | chromatin, dependency, drug_response, methylation |
| EG08 | Epigenetic memory and hysteresis | 0 | 25 | 0 | chromatin, drug_response, methylation, mutation |
| EG09 | Epigenetic repression certificate | 0 | 25 | 0 | chromatin, methylation, mutation |

The JSON companion contains all 240 r-band module rows with gates, routes, blockers, bound contrasts, and modality gaps.

## Release Boundary

- batch_or_platform_guard_receipts
- downstream_envelope_binding_receipts
- scientific_executor_release_ledger
- per-unit null_falsifier_certificate_vectors
