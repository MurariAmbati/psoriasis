# Psoriasis Contrast Normalization Targets

Blocked normalization targets for the real matrix-backed psoriasis contrasts. The artifact locks the contrast, matrix asset, sample counts, downstream envelope bindings, required receipts, and QC targets before any normalized matrix or scientific result can be written.

- Field-ready contrasts: 25
- Sample membership receipts: 25
- Sample membership rows: 2674
- Feature-universe receipts: 12
- Feature IDs in feature-universe receipts: 540973
- Matrix scale audit receipts: 12
- Matrix value cells audited: 63607757
- Normalization method receipts: 12
- Normalization method review gates: 4
- Missingness/outlier receipts: 12
- Missingness/outlier review gates: 8
- Normalization targets: 24
- Direct GSM targets: 17
- Processed bridge targets: 7
- Inherited unavailable contrasts: 1
- Downstream result-envelope targets: 6408
- Selected feature rows across targets: 1072987
- Selected sample columns across targets: 3128
- Target digest: `79e3dddf3fefe8f158f53f01a160abd5f3d4e73a43764b6f77d2c0f5ded6757e`

## Matrix Status

| Status | Targets |
| --- | ---: |
| `contrast_matrix_ready_direct_gsm` | 17 |
| `contrast_matrix_ready_processed_bridge` | 7 |

## Downstream Queues

| Source queue | Envelope targets |
| --- | ---: |
| `anduril_rm` | 4752 |
| `artmethods_method` | 528 |
| `program_engine` | 240 |
| `rband_module` | 888 |

## Normalization Targets

| Target | Accession | Contrast | Status | Assets | Features | Samples | Envelopes |
| --- | --- | --- | --- | ---: | ---: | ---: | ---: |
| `psoriasis-contrast-normalization-target-0001` | `GSE117239` | `lesional_vs_nonlesional` | `contrast_matrix_ready_direct_gsm` | 1 | 33687 | 324 | 267 |
| `psoriasis-contrast-normalization-target-0002` | `GSE117239` | `pasi75_responder_vs_nonresponder` | `contrast_matrix_ready_direct_gsm` | 1 | 33687 | 324 | 267 |
| `psoriasis-contrast-normalization-target-0003` | `GSE121212` | `lesional_vs_nonlesional` | `contrast_matrix_ready_processed_bridge` | 1 | 31364 | 147 | 267 |
| `psoriasis-contrast-normalization-target-0004` | `GSE121212` | `lesional_vs_normal` | `contrast_matrix_ready_processed_bridge` | 1 | 31364 | 147 | 267 |
| `psoriasis-contrast-normalization-target-0005` | `GSE121212` | `psoriasis_vs_atopic_dermatitis` | `contrast_matrix_ready_processed_bridge` | 1 | 31364 | 147 | 267 |
| `psoriasis-contrast-normalization-target-0006` | `GSE121212` | `psoriasis_vs_healthy_or_normal` | `contrast_matrix_ready_processed_bridge` | 1 | 31364 | 147 | 267 |
| `psoriasis-contrast-normalization-target-0007` | `GSE13355` | `lesional_vs_nonlesional` | `contrast_matrix_ready_direct_gsm` | 1 | 54675 | 180 | 267 |
| `psoriasis-contrast-normalization-target-0008` | `GSE13355` | `lesional_vs_normal` | `contrast_matrix_ready_direct_gsm` | 1 | 54675 | 180 | 267 |
| `psoriasis-contrast-normalization-target-0009` | `GSE13355` | `psoriasis_vs_healthy_or_normal` | `contrast_matrix_ready_direct_gsm` | 1 | 54675 | 180 | 267 |
| `psoriasis-contrast-normalization-target-0010` | `GSE14905` | `lesional_vs_nonlesional` | `contrast_matrix_ready_direct_gsm` | 1 | 54675 | 82 | 267 |
| `psoriasis-contrast-normalization-target-0011` | `GSE14905` | `lesional_vs_normal` | `contrast_matrix_ready_direct_gsm` | 1 | 54675 | 82 | 267 |
| `psoriasis-contrast-normalization-target-0012` | `GSE14905` | `psoriasis_vs_healthy_or_normal` | `contrast_matrix_ready_direct_gsm` | 1 | 54675 | 82 | 267 |
| `psoriasis-contrast-normalization-target-0013` | `GSE30999` | `lesional_vs_nonlesional` | `contrast_matrix_ready_direct_gsm` | 1 | 54675 | 170 | 267 |
| `psoriasis-contrast-normalization-target-0014` | `GSE34248` | `lesional_vs_nonlesional` | `contrast_matrix_ready_direct_gsm` | 1 | 54675 | 28 | 267 |
| `psoriasis-contrast-normalization-target-0015` | `GSE41662` | `lesional_vs_nonlesional` | `contrast_matrix_ready_direct_gsm` | 1 | 54675 | 48 | 267 |
| `psoriasis-contrast-normalization-target-0016` | `GSE53552` | `baseline_or_predose_treatment_axis` | `contrast_matrix_ready_direct_gsm` | 1 | 54675 | 99 | 267 |
| `psoriasis-contrast-normalization-target-0017` | `GSE53552` | `lesional_vs_nonlesional` | `contrast_matrix_ready_direct_gsm` | 1 | 54675 | 99 | 267 |
| `psoriasis-contrast-normalization-target-0018` | `GSE54456` | `lesional_vs_normal` | `contrast_matrix_ready_processed_bridge` | 1 | 21510 | 174 | 267 |
| `psoriasis-contrast-normalization-target-0019` | `GSE54456` | `psoriasis_vs_healthy_or_normal` | `contrast_matrix_ready_processed_bridge` | 1 | 21510 | 174 | 267 |
| `psoriasis-contrast-normalization-target-0020` | `GSE66511` | `psoriasis_vs_healthy_or_normal` | `contrast_matrix_ready_processed_bridge` | 1 | 24364 | 36 | 267 |
| `psoriasis-contrast-normalization-target-0021` | `GSE78097` | `lesional_vs_nonlesional` | `contrast_matrix_ready_direct_gsm` | 1 | 54675 | 33 | 267 |
| `psoriasis-contrast-normalization-target-0022` | `GSE78097` | `mild_vs_severe_source_axis` | `contrast_matrix_ready_direct_gsm` | 1 | 54675 | 33 | 267 |
| `psoriasis-contrast-normalization-target-0023` | `GSE78097` | `psoriasis_vs_healthy_or_normal` | `contrast_matrix_ready_direct_gsm` | 1 | 54675 | 33 | 267 |
| `psoriasis-contrast-normalization-target-0024` | `GSE85034` | `lesional_vs_nonlesional` | `contrast_matrix_ready_direct_gsm` | 1 | 47323 | 179 | 267 |

## Method Families

| Method family | Receipts |
| --- | ---: |
| `centered_transformed_expression_lock` | 2 |
| `count_depth_normalization` | 2 |
| `mixed_scale_review_gate` | 3 |
| `pretransformed_expression_scale_lock` | 4 |
| `processed_rpkm_or_raw_positive_expression_review` | 1 |

## Missingness And Outlier Gates

| Gate status | Receipts |
| --- | ---: |
| `extreme_outlier_profile_review_required` | 4 |
| `method_review_required_before_outlier_release` | 4 |
| `missingness_outlier_profile_ready_no_release` | 4 |

## Required Receipts

| Receipt | Status across targets |
| --- | --- |
| `matrix_asset_sha256` | `present_materialization_still_blocked`=24 |
| `field_mapping_sha256` | `present_materialization_still_blocked`=24 |
| `sample_membership_sha256` | `present_materialization_still_blocked`=24 |
| `feature_universe_sha256` | `present_materialization_still_blocked`=24 |
| `matrix_scale_audit_receipt` | `present_materialization_still_blocked`=24 |
| `normalization_method_receipt` | `present_materialization_still_blocked`=24 |
| `missingness_and_outlier_receipt` | `present_materialization_still_blocked`=24 |
| `batch_or_platform_guard_receipt` | `required_not_present`=24 |
| `processed_bridge_receipt_when_needed` | `not_applicable_direct_gsm`=17, `present_materialization_still_blocked`=7 |
| `downstream_envelope_binding_receipt` | `required_not_present`=24 |

## Release Boundary

- write batch or platform guard receipts without biological claims
- bind completed normalization receipts back to all downstream result-envelope targets
