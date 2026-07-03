# Psoriasis Feature Universe Receipts

Real-data feature universe receipts for matrix assets selected by psoriasis contrast normalization targets. Each receipt hashes the complete feature identifier list and links it back to every contrast target that consumes the asset; normalization, materialization, scientific execution, and claims remain blocked.

- Feature-universe receipts: 12
- Normalization target links: 24
- Parsed feature IDs: 540973
- Unique feature IDs within assets: 539705
- Duplicate feature IDs within assets: 322
- Blank feature IDs: 0
- Receipt digest: `a663338140ee84fb8128c3f6dfc0da57b24ca26032c42263c3b38c1d42f57327`

## Feature Namespaces

| Namespace | Receipts |
| --- | ---: |
| `gene_symbol` | 1 |
| `gene_symbol_or_processed_feature` | 2 |
| `geo_id_ref_probe_or_platform_feature` | 9 |

## Matrix Kinds

| Matrix kind | Receipts |
| --- | ---: |
| `geo_series_matrix` | 9 |
| `processed_counts_matrix` | 2 |
| `processed_expression_matrix` | 1 |

## Receipts

| Receipt | Accession | Matrix | Features | Unique | Links | Namespace |
| --- | --- | --- | ---: | ---: | ---: | --- |
| `psoriasis-feature-universe-0001` | `GSE117239` | `GSE117239_series_matrix.txt.gz` | 33687 | 33687 | 2 | `geo_id_ref_probe_or_platform_feature` |
| `psoriasis-feature-universe-0002` | `GSE121212` | `GSE121212_readcount.txt.gz` | 31364 | 31362 | 4 | `gene_symbol_or_processed_feature` |
| `psoriasis-feature-universe-0003` | `GSE13355` | `GSE13355_series_matrix.txt.gz` | 54675 | 54675 | 3 | `geo_id_ref_probe_or_platform_feature` |
| `psoriasis-feature-universe-0004` | `GSE14905` | `GSE14905_series_matrix.txt.gz` | 54675 | 54675 | 3 | `geo_id_ref_probe_or_platform_feature` |
| `psoriasis-feature-universe-0005` | `GSE30999` | `GSE30999_series_matrix.txt.gz` | 54675 | 54675 | 1 | `geo_id_ref_probe_or_platform_feature` |
| `psoriasis-feature-universe-0006` | `GSE34248` | `GSE34248_series_matrix.txt.gz` | 54675 | 54675 | 1 | `geo_id_ref_probe_or_platform_feature` |
| `psoriasis-feature-universe-0007` | `GSE41662` | `GSE41662_series_matrix.txt.gz` | 54675 | 54675 | 1 | `geo_id_ref_probe_or_platform_feature` |
| `psoriasis-feature-universe-0008` | `GSE53552` | `GSE53552_series_matrix.txt.gz` | 54675 | 54675 | 2 | `geo_id_ref_probe_or_platform_feature` |
| `psoriasis-feature-universe-0009` | `GSE54456` | `GSE54456_RPKM_samples.txt.gz` | 21510 | 21510 | 2 | `gene_symbol_or_processed_feature` |
| `psoriasis-feature-universe-0010` | `GSE66511` | `GSE66511_Psoriasis_counts.txt.gz` | 24364 | 23098 | 1 | `gene_symbol` |
| `psoriasis-feature-universe-0011` | `GSE78097` | `GSE78097_series_matrix.txt.gz` | 54675 | 54675 | 3 | `geo_id_ref_probe_or_platform_feature` |
| `psoriasis-feature-universe-0012` | `GSE85034` | `GSE85034_series_matrix.txt.gz` | 47323 | 47323 | 1 | `geo_id_ref_probe_or_platform_feature` |

## Release Boundary

- consume feature-universe SHA-256 into contrast normalization targets
- write matrix scale audit receipts
- write normalization method receipts
- write missingness and outlier receipts
- bind completed normalization receipts back to result-envelope targets
