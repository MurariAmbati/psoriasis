# Psoriasis Matrix Scale Audit Receipts

Real-data numeric scale audits for matrix assets selected by psoriasis contrast normalization targets. The receipts summarize all matrix value cells, scale classes, missingness, and numeric structure while keeping normalization, matrix materialization, scientific execution, and claims blocked.

- Matrix scale audit receipts: 12
- Normalization target links: 24
- Audited feature rows: 540973
- Audited sample columns: 1500
- Audited value cells: 63607757
- Numeric values: 63607757
- Missing values: 0
- Non-numeric values: 0
- Receipt digest: `3826d7f12e952ef041d12a69b54187475edb87db2cbd1169ca0c22dbc8066ec8`

## Scale Classes

| Scale class | Receipts |
| --- | ---: |
| `centered_or_transformed_expression_matrix` | 2 |
| `mixed_or_review_required_scale_matrix` | 3 |
| `nonnegative_count_like_integer_matrix` | 2 |
| `positive_log_or_rpkm_expression_matrix` | 4 |
| `positive_raw_intensity_or_count_scale_matrix` | 1 |

## Matrix Kinds

| Matrix kind | Receipts |
| --- | ---: |
| `geo_series_matrix` | 9 |
| `processed_counts_matrix` | 2 |
| `processed_expression_matrix` | 1 |

## Receipts

| Receipt | Accession | Matrix | Scale class | Cells | Min | Max | Mean |
| --- | --- | --- | --- | ---: | ---: | ---: | ---: |
| `psoriasis-matrix-scale-audit-0001` | `GSE117239` | `GSE117239_series_matrix.txt.gz` | `centered_or_transformed_expression_matrix` | 10914588 | -2.61236519 | 16.45728069 | 7.20610665 |
| `psoriasis-matrix-scale-audit-0002` | `GSE121212` | `GSE121212_readcount.txt.gz` | `nonnegative_count_like_integer_matrix` | 4610508 | 0.0 | 1191298.0 | 573.20452779 |
| `psoriasis-matrix-scale-audit-0003` | `GSE13355` | `GSE13355_series_matrix.txt.gz` | `centered_or_transformed_expression_matrix` | 9841500 | -5.967644 | 7.355422 | 7.576e-05 |
| `psoriasis-matrix-scale-audit-0004` | `GSE14905` | `GSE14905_series_matrix.txt.gz` | `positive_log_or_rpkm_expression_matrix` | 4483350 | 0.78240963 | 15.95626076 | 4.61044678 |
| `psoriasis-matrix-scale-audit-0005` | `GSE30999` | `GSE30999_series_matrix.txt.gz` | `positive_log_or_rpkm_expression_matrix` | 9294750 | 1.54 | 16.1 | 5.28132535 |
| `psoriasis-matrix-scale-audit-0006` | `GSE34248` | `GSE34248_series_matrix.txt.gz` | `mixed_or_review_required_scale_matrix` | 1530900 | -1906.13 | 24347.91 | 659.30249747 |
| `psoriasis-matrix-scale-audit-0007` | `GSE41662` | `GSE41662_series_matrix.txt.gz` | `mixed_or_review_required_scale_matrix` | 2624400 | -1906.4 | 126793.02 | 696.3956162 |
| `psoriasis-matrix-scale-audit-0008` | `GSE53552` | `GSE53552_series_matrix.txt.gz` | `mixed_or_review_required_scale_matrix` | 5412825 | -1884.71 | 125350.67 | 683.97658279 |
| `psoriasis-matrix-scale-audit-0009` | `GSE54456` | `GSE54456_RPKM_samples.txt.gz` | `positive_raw_intensity_or_count_scale_matrix` | 3742740 | 0.0 | 35651.046 | 22.62311752 |
| `psoriasis-matrix-scale-audit-0010` | `GSE66511` | `GSE66511_Psoriasis_counts.txt.gz` | `nonnegative_count_like_integer_matrix` | 877104 | 0.0 | 144210.0 | 51.7282979 |
| `psoriasis-matrix-scale-audit-0011` | `GSE78097` | `GSE78097_series_matrix.txt.gz` | `positive_log_or_rpkm_expression_matrix` | 1804275 | 2.09180639 | 15.5717865 | 5.86849198 |
| `psoriasis-matrix-scale-audit-0012` | `GSE85034` | `GSE85034_series_matrix.txt.gz` | `positive_log_or_rpkm_expression_matrix` | 8470817 | 6.31507646 | 14.36194268 | 7.15558679 |

## Release Boundary

- consume matrix scale audit SHA-256 into contrast normalization targets
- write normalization method receipts
- write missingness and outlier receipts
- write batch or platform guard receipts
- bind completed normalization receipts back to result-envelope targets
