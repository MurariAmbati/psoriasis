# Psoriasis Real-Data Discovery Start

This starts the psoriasis discovery process from admitted real GEO payloads and sample metadata. It records preflight/null/falsifier/novelty work, but does not write biological result claims until field-mapping, matrix materialization, and executor release gates are satisfied.

- Run id: `rdq-20260626-psoriasis-full-depth-preflight`
- GEO accessions: 13
- Admitted GEO files: 38
- Real sample units: 1528
- Module jobs: 1108
- Ready jobs: 267
- Explicit abstentions: 841
- Primary preflight rows: 8465120
- Factorized operations: 383207120
- Field-mapped samples: 1407
- Field-ready contrasts: 25
- Matrix assets: 17
- Matrix-backed contrasts: 24
- Processed matrix bridged columns: 536
- Contrast sample membership rows: 2674
- Feature-universe parsed feature IDs: 540973
- Matrix scale audit value cells: 63607757
- Normalization method receipts: 12
- Normalization method review gates: 4
- Missingness/outlier profiled cells: 63607757
- Missingness/outlier review gates: 8
- Contrast normalization targets: 24
- Module input rows: 27700
- Module input matrix-bound rows: 6408
- Result-envelope targets: 6408
- Scientific result rows written: 0

## Discovery Processes

| Process | Status | Real-data units | Blocked next |
| --- | --- | ---: | --- |
| `psoriasis_geo_payload_admission` | `started_and_payloads_present` | 38 | raw GEO tar archives; bulk MINiML files; scientific result execution |
| `psoriasis_geo_sample_identity` | `sample_adapter_artifact_ready` | 1528 | label inference; matrix materialization; claim promotion |
| `psoriasis_phenotype_comparator_mapping` | `field_mapping_receipt_ready` | 1407 | matrix materialization; result envelopes; claim promotion |
| `psoriasis_lesion_severity_mapping` | `field_mapping_receipt_ready` | 25 | treating lesion/nonlesion contrast as severity; PASI/severity claim promotion; matrix materialization |
| `psoriasis_treatment_exposure_mapping` | `field_mapping_receipt_ready` | 193 | therapy-response claims; dose/timepoint mechanism claims; matrix materialization |
| `psoriasis_matrix_availability_mapping` | `matrix_availability_receipt_ready` | 17 | processed-matrix sample-id bridge receipts; normalized matrix materialization; scientific executor release |
| `psoriasis_processed_matrix_sample_bridge` | `processed_matrix_bridge_receipt_ready` | 536 | ordinal bridge executor review; normalized matrix materialization; per-module input receipts |
| `psoriasis_contrast_sample_membership_receipts` | `contrast_sample_membership_receipts_ready` | 2674 | feature universe receipts; matrix scale audits; normalization method receipts; scientific executor release |
| `psoriasis_feature_universe_receipts` | `feature_universe_receipts_ready` | 540973 | matrix scale audits; normalization method receipts; missingness and outlier receipts; scientific executor release |
| `psoriasis_matrix_scale_audit_receipts` | `matrix_scale_audit_receipts_ready` | 63607757 | normalization method receipts; missingness and outlier receipts; batch/platform guard receipts; scientific executor release |
| `psoriasis_normalization_method_receipts` | `normalization_method_receipts_ready` | 12 | missingness and outlier receipts; batch/platform guard receipts; normalized matrix materialization; scientific executor release |
| `psoriasis_missingness_outlier_receipts` | `missingness_outlier_receipts_ready` | 63607757 | batch/platform guard receipts; downstream envelope binding receipts; normalized matrix materialization; scientific executor release |
| `psoriasis_contrast_normalization_targets` | `contrast_normalization_targets_ready` | 24 | batch/platform guard receipts; downstream envelope binding receipts |
| `psoriasis_module_input_queue` | `module_input_queue_ready` | 27700 | matrix normalization ledgers; per-module output envelope targets; scientific executor release |
| `psoriasis_result_envelope_targets` | `result_envelope_targets_ready` | 6408 | matrix normalization receipts; null and falsifier execution; certificate vectors; claim promotion |
| `psoriasis_full_depth_module_preflight` | `executed_preflight_only` | 8465120 | sample adapter candidates are still blocked until reviewed field-mapping receipts exist; matrix materialization is disabled by the psoriasis GEO sample adapter manifest; scientific module executor release is absent; claim promotion is forbidden until result envelopes and certificate vectors exist |
| `psoriasis_anduril_rm_module_discovery` | `started_preflight_only` | 650 | blocked_until_adapter_release_and_result_ledgers |
| `psoriasis_artmethods_method_module_discovery` | `started_preflight_only` | 202 | blocked_until_adapter_release_and_result_ledgers |
| `psoriasis_program_engine_module_discovery` | `started_preflight_only` | 16 | blocked_until_adapter_release_and_result_ledgers |
| `psoriasis_rband_module_module_discovery` | `started_preflight_only` | 240 | blocked_until_adapter_release_and_result_ledgers |

## Sample Field Coverage

| Field category | Samples |
| --- | ---: |
| `age` | 36 |
| `lesion_or_severity` | 503 |
| `phenotype_or_diagnosis` | 898 |
| `sex` | 92 |
| `subject_identity` | 804 |
| `technical_or_batch` | 324 |
| `tissue_or_region` | 1528 |
| `treatment_or_exposure` | 635 |

## Field Mapping Receipt

- Digest: `b91c4c3c4d7516740e7189bc2bcd4a271e4d79a5612f182424dac39b84a4458f`
- Ready contrasts: 25
- Contrast abstentions: 66
- Skin regions: `lesional`=746, `nonlesional`=420, `normal_or_healthy_skin`=205, `skin_unspecified`=157
- Severity: `mild_explicit`=14, `pasi_numeric_available`=307, `severe_explicit`=183, `unmapped`=1024
- Response: `pasi75_nonresponder`=93, `pasi75_responder`=231, `unmapped`=1204

## Matrix Availability Receipt

- Digest: `0c083e51b6d62c7047e7b8ca3338279da8bb248bc0b4de35318b70b9a9f46c68`
- Download run: `rdq-20260626-psoriasis-deep-disease-psoriasis-geo-small-files`
- Downloaded payloads: 38
- Payload SHA matches: 38
- Matrix assets: 17
- Matrix-ready accessions: 12
- Contrast matrix status: `contrast_matrix_ready_direct_gsm`=17, `contrast_matrix_ready_processed_bridge`=7, `contrast_matrix_unavailable`=1
- Processed bridge: 536 sample columns, 8 contrasts

## Contrast Sample Membership Receipts

- Digest: `5393bac445befe44b774f7cd9bd50a91587b51c9b7be7e6aec9db92d8c4c956c`
- Receipts: 25
- Sample membership rows: 2674
- Normalization-ready receipts: 24
- Matrix-unavailable abstentions: 1
- Paired subject pairs: 314
- Matrix column bindings: `direct_gsm_table_header_bound`=1858, `no_selected_matrix_asset`=28, `processed_bridge_column_bound`=788

## Feature Universe Receipts

- Digest: `a663338140ee84fb8128c3f6dfc0da57b24ca26032c42263c3b38c1d42f57327`
- Receipts: 12
- Normalization target links: 24
- Parsed feature IDs: 540973
- Unique feature IDs within assets: 539705
- Duplicate feature IDs within assets: 322
- Duplicate feature rows within assets: 1268
- Feature namespaces: `gene_symbol`=1, `gene_symbol_or_processed_feature`=2, `geo_id_ref_probe_or_platform_feature`=9

## Matrix Scale Audit Receipts

- Digest: `3826d7f12e952ef041d12a69b54187475edb87db2cbd1169ca0c22dbc8066ec8`
- Receipts: 12
- Normalization target links: 24
- Audited value cells: 63607757
- Numeric values: 63607757
- Missing values: 0
- Non-numeric values: 0
- Scale classes: `centered_or_transformed_expression_matrix`=2, `mixed_or_review_required_scale_matrix`=3, `nonnegative_count_like_integer_matrix`=2, `positive_log_or_rpkm_expression_matrix`=4, `positive_raw_intensity_or_count_scale_matrix`=1

## Normalization Method Receipts

- Digest: `a164b6edc7389f3d4308ffecf81c65113baabd3202f42de3c9a2b805a272f4a9`
- Receipts: 12
- Normalization target links: 24
- Review-required receipts: 4
- Method families: `centered_transformed_expression_lock`=2, `count_depth_normalization`=2, `mixed_scale_review_gate`=3, `pretransformed_expression_scale_lock`=4, `processed_rpkm_or_raw_positive_expression_review`=1
- Method statuses: `planned_not_executed`=8, `review_required_not_executed`=4

## Missingness And Outlier Receipts

- Digest: `9df136ec4e0f51a9015830f6a22a07a4406ff6e4202a4048c00ce98dd16138ec`
- Receipts: 12
- Normalization target links: 24
- Profiled value cells: 63607757
- Missing values: 0
- Non-numeric values: 0
- Z-score >= 3 outliers: 657357
- Z-score >= 5 outliers: 165724
- Review-required receipts: 8
- Gate statuses: `extreme_outlier_profile_review_required`=4, `method_review_required_before_outlier_release`=4, `missingness_outlier_profile_ready_no_release`=4

## Contrast Normalization Targets

- Digest: `79e3dddf3fefe8f158f53f01a160abd5f3d4e73a43764b6f77d2c0f5ded6757e`
- Targets: 24
- Direct GSM targets: 17
- Processed bridge targets: 7
- Inherited unavailable contrasts: 1
- Downstream envelope targets: 6408
- Required receipts per target: 10
- QC targets per target: 9

## Module Input Queue

- Digest: `e507f8367f7d43d87a10038a76749b52497f4457fe3c850f5b57d444aba638f4`
- Input rows: 27700
- Matrix-bound executor-blocked rows: 6408
- Module abstention rows: 21025
- Contrast-unavailable abstention rows: 267
- Row states: `contrast_matrix_unavailable_abstention`=267, `matrix_bound_executor_blocked`=6408, `module_abstention_record`=21025

## Result-Envelope Targets

- Digest: `7d48f976210424a8893eea7ec3d162b35fe8c32ca788684c208ff6373cc6cfce`
- Targets: 6408
- Matrix-bound source inputs: 6408
- Inherited module abstentions: 21025
- Inherited contrast-unavailable abstentions: 267
- Certificates per target: 11
- Null models per target: 6
- Falsifiers per target: 8

## Accession Support Domains

| Accession | Samples | Support domain |
| --- | ---: | --- |
| `GSE117239` | 324 | ustekinumab responder and nonresponder source view for longitudinal lesion biology |
| `GSE121212` | 147 | RNA-seq comparator source view spanning atopic dermatitis, psoriasis, and healthy control skin |
| `GSE13355` | 180 | classic skin source view separating involved lesional skin, uninvolved nonlesional skin, and normal control skin |
| `GSE14905` | 82 | type-I-interferon lesional skin source view with dendritic-cell and T-cell infiltration signatures |
| `GSE30999` | 170 | moderate-to-severe plaque psoriasis trial biopsy source view with matched lesional and nonlesional skin |
| `GSE34248` | 28 | lesional and nonlesional skin discovery source view |
| `GSE41662` | 48 | lesional and nonlesional skin replication source view |
| `GSE53552` | 99 | brodalumab treatment source view with lesional, nonlesional, dose, and time labels |
| `GSE54456` | 174 | lesional psoriasis and normal skin RNA-seq source view with microarray overlap sidecar |
| `GSE66511` | 36 | RNA-seq lesional, nonlesional, and healthy-control skin source view with IL36 axis support |
| `GSE67785` | 28 | RNA-seq proteogenomic lesion and uninvolved skin source view |
| `GSE78097` | 33 | mild versus severe psoriasis vulgaris source view with IL-17 pathway activation labels |
| `GSE85034` | 179 | adalimumab and methotrexate response-prediction source view across baseline and early treatment timepoints |

## Release Blockers

- matrix materialization remains disabled by the sample adapter gate
- executor release and compute ledger are absent for scientific modules
- claims remain forbidden until result envelopes, nulls, falsifiers, and certificates are written
