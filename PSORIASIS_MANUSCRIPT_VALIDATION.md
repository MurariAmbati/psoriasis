# Psoriasis Processed-Matrix Sample Bridge Receipt

Real-data bridge from processed psoriasis matrix columns to GEO sample units. Exact title bridges and ordinal series-order bridges are recorded separately, while matrix materialization and scientific execution remain blocked.

- Processed matrices: 4
- Bridge-ready matrices: 4
- Bridged sample columns: 536
- Bridge abstentions: 0
- Detect-pvalue columns: 179
- Numeric label gaps: 1
- Processed bridge contrasts: 8
- Bridge digest: `b10562250c9531ed0ac7d2326920915cf0bf3e57aa9e0ba4fde27434e2dc862d`

## Bridge Status

| Status | Count |
| --- | ---: |
| `exact_title_bridge_ready` | 3 |
| `ordinal_series_order_bridge_ready` | 1 |

## Evidence Counts

| Evidence | Count |
| --- | ---: |
| `exact_title_bridge` | 357 |
| `ordinal_series_order_bridge` | 179 |

## Matrix Bridges

| Accession | Matrix | Policy | Samples | Features | Numeric gaps |
| --- | --- | --- | ---: | ---: | --- |
| `GSE54456` | `GSE54456_RPKM_samples.txt.gz` | `exact_processed_header_to_geo_sample_title` | 174 | 21510 |  |
| `GSE66511` | `GSE66511_Psoriasis_counts.txt.gz` | `exact_processed_header_to_geo_sample_title` | 36 | 24364 |  |
| `GSE85034` | `GSE85034_non_normalized.txt.gz` | `ordered_processed_columns_to_geo_series_samples` | 179 | 47323 | 108 |
| `GSE121212` | `GSE121212_readcount.txt.gz` | `exact_processed_header_to_geo_sample_title` | 147 | 31364 |  |

## Processed-Bridge Contrasts

| Accession | Contrast | Matrix | Bridge status |
| --- | --- | --- | --- |
| `GSE121212` | `lesional_vs_nonlesional` | `GSE121212_readcount.txt.gz` | `exact_title_bridge_ready` |
| `GSE121212` | `lesional_vs_normal` | `GSE121212_readcount.txt.gz` | `exact_title_bridge_ready` |
| `GSE121212` | `psoriasis_vs_atopic_dermatitis` | `GSE121212_readcount.txt.gz` | `exact_title_bridge_ready` |
| `GSE121212` | `psoriasis_vs_healthy_or_normal` | `GSE121212_readcount.txt.gz` | `exact_title_bridge_ready` |
| `GSE54456` | `lesional_vs_normal` | `GSE54456_RPKM_samples.txt.gz` | `exact_title_bridge_ready` |
| `GSE54456` | `psoriasis_vs_healthy_or_normal` | `GSE54456_RPKM_samples.txt.gz` | `exact_title_bridge_ready` |
| `GSE66511` | `psoriasis_vs_healthy_or_normal` | `GSE66511_Psoriasis_counts.txt.gz` | `exact_title_bridge_ready` |
| `GSE85034` | `lesional_vs_nonlesional` | `GSE85034_non_normalized.txt.gz` | `ordinal_series_order_bridge_ready` |

## Release Boundary

- bind bridge rows into accession-specific matrix materialization ledgers
- validate processed-matrix scale and normalization metadata before cross-study comparison
- keep ordinal sample-order bridges review-gated until executor release records the order policy
- attach bridge SHA-256 to every downstream module input receipt
