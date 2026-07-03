# Psoriasis Repression Program

Disease-pack Repression discovery run over the psoriasis real-data receipt chain. This report binds real GEO sample, contrast, matrix, normalization, and module-input receipts; it does not execute scientific modules or promote biological claims.

- Program status: `repression_inputs_bound_executor_blocked`
- Samples: 1528
- Field-ready contrasts: 25
- Matrix-backed contrasts: 24
- Matrix value cells audited: 63607757
- Missingness/outlier cells profiled: 63607757
- Matrix-bound module rows: 6408
- Result-envelope targets: 6408
- Report digest: `dffc045926550605e5ba45fba9d71c02d9a9e1e8ecc00279ce5c08a2639395b7`

## Contrast Axes

| Axis | Ready contrasts |
| --- | ---: |
| `lesional_vs_nonlesional` | 11 |
| `lesional_vs_normal` | 4 |
| `psoriasis_vs_atopic_dermatitis` | 1 |
| `psoriasis_vs_healthy_or_normal` | 6 |
| `severity_source_axis` | 1 |
| `treatment_or_response` | 2 |

## Ready Contrasts

| Accession | Contrast | Left | Right | Paired possible |
| --- | --- | ---: | ---: | --- |
| `GSE117239` | `lesional_vs_nonlesional` | 240 | 84 | true |
| `GSE117239` | `pasi75_responder_vs_nonresponder` | 231 | 93 | false |
| `GSE121212` | `lesional_vs_nonlesional` | 55 | 54 | true |
| `GSE121212` | `lesional_vs_normal` | 55 | 38 | false |
| `GSE121212` | `psoriasis_vs_atopic_dermatitis` | 55 | 54 | false |
| `GSE121212` | `psoriasis_vs_healthy_or_normal` | 55 | 38 | false |
| `GSE13355` | `lesional_vs_nonlesional` | 58 | 58 | true |
| `GSE13355` | `lesional_vs_normal` | 58 | 64 | false |
| `GSE13355` | `psoriasis_vs_healthy_or_normal` | 116 | 64 | false |
| `GSE14905` | `lesional_vs_nonlesional` | 33 | 28 | true |
| `GSE14905` | `lesional_vs_normal` | 33 | 21 | false |
| `GSE14905` | `psoriasis_vs_healthy_or_normal` | 61 | 21 | false |
| `GSE30999` | `lesional_vs_nonlesional` | 85 | 85 | true |
| `GSE34248` | `lesional_vs_nonlesional` | 14 | 14 | true |
| `GSE41662` | `lesional_vs_nonlesional` | 24 | 24 | true |
| `GSE53552` | `baseline_or_predose_treatment_axis` | 49 | 50 | false |
| `GSE53552` | `lesional_vs_nonlesional` | 75 | 24 | true |
| `GSE54456` | `lesional_vs_normal` | 92 | 82 | false |
| `GSE54456` | `psoriasis_vs_healthy_or_normal` | 92 | 82 | false |
| `GSE66511` | `psoriasis_vs_healthy_or_normal` | 24 | 12 | false |
| `GSE67785` | `lesional_vs_nonlesional` | 14 | 14 | true |
| `GSE78097` | `lesional_vs_nonlesional` | 27 | 6 | true |
| `GSE78097` | `mild_vs_severe_source_axis` | 14 | 13 | false |
| `GSE78097` | `psoriasis_vs_healthy_or_normal` | 27 | 6 | false |
| `GSE85034` | `lesional_vs_nonlesional` | 29 | 29 | true |

## Module Binding

| Source queue | Units | Matrix-bound rows | Abstentions |
| --- | ---: | ---: | ---: |
| `anduril_rm` | 650 | 4752 | 11498 |
| `artmethods_method` | 202 | 528 | 4522 |
| `program_engine` | 16 | 240 | 160 |
| `rband_module` | 240 | 888 | 5112 |

## Receipt Chain

| Receipt | Count |
| --- | ---: |
| `sample_membership_receipts` | 25 |
| `feature_universe_receipts` | 12 |
| `matrix_scale_audit_receipts` | 12 |
| `normalization_method_receipts` | 12 |
| `missingness_outlier_receipts` | 12 |
| `contrast_normalization_targets` | 24 |
| `result_envelope_targets` | 6408 |

## Missingness And Method Gates

| Gate | Count |
| --- | ---: |
| `extreme_outlier_profile_review_required` | 4 |
| `method_review_required_before_outlier_release` | 4 |
| `missingness_outlier_profile_ready_no_release` | 4 |

## Normalization Method Families

| Family | Receipts |
| --- | ---: |
| `centered_transformed_expression_lock` | 2 |
| `count_depth_normalization` | 2 |
| `mixed_scale_review_gate` | 3 |
| `pretransformed_expression_scale_lock` | 4 |
| `processed_rpkm_or_raw_positive_expression_review` | 1 |

## Next Required Receipts

- batch_or_platform_guard_receipts
- downstream_envelope_binding_receipts
- scientific_executor_release_ledger
- null_falsifier_certificate_vectors
