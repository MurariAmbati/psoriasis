# Psoriasis Missingness And Outlier Receipts

Real-data missingness and outlier profiles for every matrix asset selected by psoriasis normalization targets. The receipts scan matrix values and record release gates without writing normalized matrices or biological claims.

- Missingness/outlier receipts: 12
- Normalization target links: 24
- Profiled value cells: 63607757
- Missing values: 0
- Non-numeric values: 0
- Z-score >= 3 outliers: 657357
- Z-score >= 5 outliers: 165724
- Review-required receipts: 8
- Receipt digest: `9df136ec4e0f51a9015830f6a22a07a4406ff6e4202a4048c00ce98dd16138ec`

## Gate Status

| Gate status | Receipts |
| --- | ---: |
| `extreme_outlier_profile_review_required` | 4 |
| `method_review_required_before_outlier_release` | 4 |
| `missingness_outlier_profile_ready_no_release` | 4 |

## Method Families

| Method family | Receipts |
| --- | ---: |
| `centered_transformed_expression_lock` | 2 |
| `count_depth_normalization` | 2 |
| `mixed_scale_review_gate` | 3 |
| `pretransformed_expression_scale_lock` | 4 |
| `processed_rpkm_or_raw_positive_expression_review` | 1 |

## Receipts

| Receipt | Accession | Matrix | Gate | Cells | Z>=3 | Z>=5 | Max abs z |
| --- | --- | --- | --- | ---: | ---: | ---: | ---: |
| `psoriasis-missingness-outlier-0001` | `GSE117239` | `GSE117239_series_matrix.txt.gz` | `missingness_outlier_profile_ready_no_release` | 10914588 | 0 | 0 | 2.64961493 |
| `psoriasis-missingness-outlier-0002` | `GSE121212` | `GSE121212_readcount.txt.gz` | `extreme_outlier_profile_review_required` | 4610508 | 13164 | 6631 | 217.70729208 |
| `psoriasis-missingness-outlier-0003` | `GSE13355` | `GSE13355_series_matrix.txt.gz` | `extreme_outlier_profile_review_required` | 9841500 | 160188 | 32224 | 23.45200159 |
| `psoriasis-missingness-outlier-0004` | `GSE14905` | `GSE14905_series_matrix.txt.gz` | `missingness_outlier_profile_ready_no_release` | 4483350 | 33984 | 0 | 4.3058106 |
| `psoriasis-missingness-outlier-0005` | `GSE30999` | `GSE30999_series_matrix.txt.gz` | `missingness_outlier_profile_ready_no_release` | 9294750 | 0 | 0 | 2.84379838 |
| `psoriasis-missingness-outlier-0006` | `GSE34248` | `GSE34248_series_matrix.txt.gz` | `method_review_required_before_outlier_release` | 1530900 | 37671 | 11872 | 16.94989606 |
| `psoriasis-missingness-outlier-0007` | `GSE41662` | `GSE41662_series_matrix.txt.gz` | `method_review_required_before_outlier_release` | 2624400 | 58222 | 19624 | 85.14081932 |
| `psoriasis-missingness-outlier-0008` | `GSE53552` | `GSE53552_series_matrix.txt.gz` | `method_review_required_before_outlier_release` | 5412825 | 119752 | 40024 | 86.51420925 |
| `psoriasis-missingness-outlier-0009` | `GSE54456` | `GSE54456_RPKM_samples.txt.gz` | `method_review_required_before_outlier_release` | 3742740 | 14731 | 7306 | 151.26522607 |
| `psoriasis-missingness-outlier-0010` | `GSE66511` | `GSE66511_Psoriasis_counts.txt.gz` | `extreme_outlier_profile_review_required` | 877104 | 1080 | 608 | 226.63760674 |
| `psoriasis-missingness-outlier-0011` | `GSE78097` | `GSE78097_series_matrix.txt.gz` | `missingness_outlier_profile_ready_no_release` | 1804275 | 0 | 0 | 2.60624818 |
| `psoriasis-missingness-outlier-0012` | `GSE85034` | `GSE85034_series_matrix.txt.gz` | `extreme_outlier_profile_review_required` | 8470817 | 218565 | 47435 | 6.78189556 |

## Release Boundary

- consume missingness and outlier SHA-256 into contrast normalization targets
- write batch or platform guard receipts
- write downstream envelope binding receipts
- only then materialize normalized matrices under executor release
