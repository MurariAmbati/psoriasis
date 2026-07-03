# Psoriasis Normalization Method Receipts

Blocked normalization-method receipts selected from real psoriasis matrix scale audits. The receipts choose method families and release requirements but do not materialize normalized matrices or permit scientific execution.

- Normalization method receipts: 12
- Normalization target links: 24
- Review-required receipts: 4
- Receipt digest: `a164b6edc7389f3d4308ffecf81c65113baabd3202f42de3c9a2b805a272f4a9`

## Method Families

| Method family | Receipts |
| --- | ---: |
| `centered_transformed_expression_lock` | 2 |
| `count_depth_normalization` | 2 |
| `mixed_scale_review_gate` | 3 |
| `pretransformed_expression_scale_lock` | 4 |
| `processed_rpkm_or_raw_positive_expression_review` | 1 |

## Method Status

| Status | Receipts |
| --- | ---: |
| `planned_not_executed` | 8 |
| `review_required_not_executed` | 4 |

## Receipts

| Receipt | Accession | Matrix | Scale class | Method | Review | Links |
| --- | --- | --- | --- | --- | --- | ---: |
| `psoriasis-normalization-method-0001` | `GSE117239` | `GSE117239_series_matrix.txt.gz` | `centered_or_transformed_expression_matrix` | `identity_centered_expression_scale_lock_plan_blocked` | false | 2 |
| `psoriasis-normalization-method-0002` | `GSE121212` | `GSE121212_readcount.txt.gz` | `nonnegative_count_like_integer_matrix` | `count_matrix_size_factor_or_tmm_plan_blocked` | false | 4 |
| `psoriasis-normalization-method-0003` | `GSE13355` | `GSE13355_series_matrix.txt.gz` | `centered_or_transformed_expression_matrix` | `identity_centered_expression_scale_lock_plan_blocked` | false | 3 |
| `psoriasis-normalization-method-0004` | `GSE14905` | `GSE14905_series_matrix.txt.gz` | `positive_log_or_rpkm_expression_matrix` | `identity_log_expression_scale_lock_plan_blocked` | false | 3 |
| `psoriasis-normalization-method-0005` | `GSE30999` | `GSE30999_series_matrix.txt.gz` | `positive_log_or_rpkm_expression_matrix` | `identity_log_expression_scale_lock_plan_blocked` | false | 1 |
| `psoriasis-normalization-method-0006` | `GSE34248` | `GSE34248_series_matrix.txt.gz` | `mixed_or_review_required_scale_matrix` | `mixed_scale_review_required_no_release_plan` | true | 1 |
| `psoriasis-normalization-method-0007` | `GSE41662` | `GSE41662_series_matrix.txt.gz` | `mixed_or_review_required_scale_matrix` | `mixed_scale_review_required_no_release_plan` | true | 1 |
| `psoriasis-normalization-method-0008` | `GSE53552` | `GSE53552_series_matrix.txt.gz` | `mixed_or_review_required_scale_matrix` | `mixed_scale_review_required_no_release_plan` | true | 2 |
| `psoriasis-normalization-method-0009` | `GSE54456` | `GSE54456_RPKM_samples.txt.gz` | `positive_raw_intensity_or_count_scale_matrix` | `log2_plus_distribution_review_plan_blocked` | true | 2 |
| `psoriasis-normalization-method-0010` | `GSE66511` | `GSE66511_Psoriasis_counts.txt.gz` | `nonnegative_count_like_integer_matrix` | `count_matrix_size_factor_or_tmm_plan_blocked` | false | 1 |
| `psoriasis-normalization-method-0011` | `GSE78097` | `GSE78097_series_matrix.txt.gz` | `positive_log_or_rpkm_expression_matrix` | `identity_log_expression_scale_lock_plan_blocked` | false | 3 |
| `psoriasis-normalization-method-0012` | `GSE85034` | `GSE85034_series_matrix.txt.gz` | `positive_log_or_rpkm_expression_matrix` | `identity_log_expression_scale_lock_plan_blocked` | false | 1 |

## Release Boundary

- write missingness and outlier receipts
- write batch or platform guard receipts
- write downstream envelope binding receipts
- only then materialize normalized matrices under executor release
