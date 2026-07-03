# Psoriasis Matrix Availability Receipt

Structural availability receipt for downloaded real GEO psoriasis matrices. It verifies local payload hashes and table shape, binds field-ready contrasts to matrix assets, and still blocks matrix materialization and scientific execution.

- Download run: `rdq-20260626-psoriasis-deep-disease-psoriasis-geo-small-files`
- Downloaded payloads: 38
- Downloaded bytes: 486993897
- Payload SHA matches: 38
- Matrix assets: 17
- Matrix-ready accessions: 12
- Matrix feature rows scanned: 588296
- Matrix sample columns scanned: 1679
- Field-ready contrasts: 25
- Processed bridge contrasts: 8
- Matrix availability digest: `0c083e51b6d62c7047e7b8ca3338279da8bb248bc0b4de35318b70b9a9f46c68`

## Asset Counts

| Class | Count |
| --- | ---: |
| `geo_filelist` | 10 |
| `miniml_family_metadata` | 10 |
| `processed_counts_matrix` | 2 |
| `processed_expression_matrix` | 2 |
| `processed_overlap_sidecar` | 1 |
| `series_matrix` | 13 |

## Matrix Status

| Status | Count |
| --- | ---: |
| `matrix_payload_review_gated` | 4 |
| `matrix_payload_verified` | 13 |

## Contrast Matrix Binding

| Status | Count |
| --- | ---: |
| `contrast_matrix_ready_direct_gsm` | 17 |
| `contrast_matrix_ready_processed_bridge` | 7 |
| `contrast_matrix_unavailable` | 1 |

## Matrix Assets

| Accession | Asset | Kind | Features | Samples | Direct GSM |
| --- | --- | --- | ---: | ---: | --- |
| `GSE13355` | `GSE13355_series_matrix.txt.gz` | `geo_series_matrix` | 54675 | 180 | true |
| `GSE30999` | `GSE30999_series_matrix.txt.gz` | `geo_series_matrix` | 54675 | 170 | true |
| `GSE41662` | `GSE41662_series_matrix.txt.gz` | `geo_series_matrix` | 54675 | 48 | true |
| `GSE53552` | `GSE53552_series_matrix.txt.gz` | `geo_series_matrix` | 54675 | 99 | true |
| `GSE54456` | `GSE54456_series_matrix.txt.gz` | `geo_series_matrix` | 0 | 174 | true |
| `GSE54456` | `GSE54456_RPKM_samples.txt.gz` | `processed_expression_matrix` | 21510 | 174 | false |
| `GSE78097` | `GSE78097_series_matrix.txt.gz` | `geo_series_matrix` | 54675 | 33 | true |
| `GSE117239` | `GSE117239_series_matrix.txt.gz` | `geo_series_matrix` | 33687 | 324 | true |
| `GSE14905` | `GSE14905_series_matrix.txt.gz` | `geo_series_matrix` | 54675 | 82 | true |
| `GSE34248` | `GSE34248_series_matrix.txt.gz` | `geo_series_matrix` | 54675 | 28 | true |
| `GSE66511` | `GSE66511_series_matrix.txt.gz` | `geo_series_matrix` | 0 | 36 | true |
| `GSE66511` | `GSE66511_Psoriasis_counts.txt.gz` | `processed_counts_matrix` | 24364 | 36 | false |
| `GSE67785` | `GSE67785_series_matrix.txt.gz` | `geo_series_matrix` | 0 | 28 | true |
| `GSE85034` | `GSE85034_series_matrix.txt.gz` | `geo_series_matrix` | 47323 | 179 | true |
| `GSE85034` | `GSE85034_non_normalized.txt.gz` | `processed_expression_matrix` | 47323 | 179 | false |
| `GSE121212` | `GSE121212_series_matrix.txt.gz` | `geo_series_matrix` | 0 | 147 | true |
| `GSE121212` | `GSE121212_readcount.txt.gz` | `processed_counts_matrix` | 31364 | 147 | false |

## Ready Contrast Bindings

| Accession | Contrast | Status | Direct assets | Processed assets |
| --- | --- | --- | ---: | ---: |
| `GSE117239` | `lesional_vs_nonlesional` | `contrast_matrix_ready_direct_gsm` | 1 | 0 |
| `GSE117239` | `pasi75_responder_vs_nonresponder` | `contrast_matrix_ready_direct_gsm` | 1 | 0 |
| `GSE121212` | `lesional_vs_nonlesional` | `contrast_matrix_ready_processed_bridge` | 0 | 1 |
| `GSE121212` | `lesional_vs_normal` | `contrast_matrix_ready_processed_bridge` | 0 | 1 |
| `GSE121212` | `psoriasis_vs_atopic_dermatitis` | `contrast_matrix_ready_processed_bridge` | 0 | 1 |
| `GSE121212` | `psoriasis_vs_healthy_or_normal` | `contrast_matrix_ready_processed_bridge` | 0 | 1 |
| `GSE13355` | `lesional_vs_nonlesional` | `contrast_matrix_ready_direct_gsm` | 1 | 0 |
| `GSE13355` | `lesional_vs_normal` | `contrast_matrix_ready_direct_gsm` | 1 | 0 |
| `GSE13355` | `psoriasis_vs_healthy_or_normal` | `contrast_matrix_ready_direct_gsm` | 1 | 0 |
| `GSE14905` | `lesional_vs_nonlesional` | `contrast_matrix_ready_direct_gsm` | 1 | 0 |
| `GSE14905` | `lesional_vs_normal` | `contrast_matrix_ready_direct_gsm` | 1 | 0 |
| `GSE14905` | `psoriasis_vs_healthy_or_normal` | `contrast_matrix_ready_direct_gsm` | 1 | 0 |
| `GSE30999` | `lesional_vs_nonlesional` | `contrast_matrix_ready_direct_gsm` | 1 | 0 |
| `GSE34248` | `lesional_vs_nonlesional` | `contrast_matrix_ready_direct_gsm` | 1 | 0 |
| `GSE41662` | `lesional_vs_nonlesional` | `contrast_matrix_ready_direct_gsm` | 1 | 0 |
| `GSE53552` | `lesional_vs_nonlesional` | `contrast_matrix_ready_direct_gsm` | 1 | 0 |
| `GSE53552` | `baseline_or_predose_treatment_axis` | `contrast_matrix_ready_direct_gsm` | 1 | 0 |
| `GSE54456` | `lesional_vs_normal` | `contrast_matrix_ready_processed_bridge` | 0 | 1 |
| `GSE54456` | `psoriasis_vs_healthy_or_normal` | `contrast_matrix_ready_processed_bridge` | 0 | 1 |
| `GSE66511` | `psoriasis_vs_healthy_or_normal` | `contrast_matrix_ready_processed_bridge` | 0 | 1 |
| `GSE67785` | `lesional_vs_nonlesional` | `contrast_matrix_unavailable` | 0 | 0 |
| `GSE78097` | `lesional_vs_nonlesional` | `contrast_matrix_ready_direct_gsm` | 1 | 0 |
| `GSE78097` | `psoriasis_vs_healthy_or_normal` | `contrast_matrix_ready_direct_gsm` | 1 | 0 |
| `GSE78097` | `mild_vs_severe_source_axis` | `contrast_matrix_ready_direct_gsm` | 1 | 0 |
| `GSE85034` | `lesional_vs_nonlesional` | `contrast_matrix_ready_direct_gsm` | 1 | 1 |

## Release Boundary

- write accession-specific sample-id bridge receipts for processed matrices without GSM headers
- consume processed-matrix sample bridges into materialization ledgers
- materialize normalized expression matrices under an executor release gate
- bind every module input to matrix asset SHA-256 and field mapping SHA-256
- write result envelopes with null, falsifier, and abstention certificates before claims
