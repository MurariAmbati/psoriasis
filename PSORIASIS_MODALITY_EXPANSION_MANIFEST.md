# Psoriasis Program Reports

Aggregate disease-pack run for the psoriasis Repression, Sentinel, and Vindicate lanes.

- Samples: 1528
- Matrix-backed contrasts: 24
- Result-envelope targets: 6408
- Scientific result rows written: 0
- Aggregate digest: `fb0705a07b6f09ff50ed22f105ba94b706cb50dd01366a83c255825c53dd6a3f`

## Program Reports

| Program | Status | Digest |
| --- | --- | --- |
| `repression` | `repression_inputs_bound_executor_blocked` | `dffc045926550605e5ba45fba9d71c02d9a9e1e8ecc00279ce5c08a2639395b7` |
| `sentinel` | `completed_psoriasis_receipt_watchdog` | `ea7c49304f0d6299a2c588f5cad4cba8d5a433833d03223941d470d1b829a583` |
| `vindicate` | `vindicate_interception_inputs_bound_executor_blocked` | `a7818a8d04bcbc23a2dd46163f5d0dd44fd9476bc03928fa833312eb7f240ba7` |

## Real Data Scope

| Scope | Count |
| --- | ---: |
| `sample_unit_count` | 1528 |
| `field_mapped_sample_count` | 1407 |
| `field_ready_contrast_count` | 25 |
| `matrix_backed_contrast_count` | 24 |
| `matrix_asset_count` | 17 |
| `feature_universe_parsed_feature_id_count` | 540973 |
| `matrix_scale_audit_value_cell_count` | 63607757 |
| `missingness_outlier_profiled_value_cell_count` | 63607757 |
| `contrast_normalization_target_count` | 24 |
| `module_input_row_count` | 27700 |
| `matrix_bound_module_input_rows` | 6408 |
| `result_envelope_target_count` | 6408 |
| `scientific_result_rows_written` | 0 |

## Source Artifacts

| Artifact | Path | Digest |
| --- | --- | --- |
| `field_mapping` | `diseases/MONDO_0005083_psoriasis/results/psoriasis_geo_field_mapping_receipt_latest.json` | `e4c7c70a8dc585d5d6af653a3e1d46cca162e090eb8d2011bc583584c9125536` |
| `matrix_availability` | `diseases/MONDO_0005083_psoriasis/results/psoriasis_matrix_availability_receipt_latest.json` | `00a58db1087c6fd54f5981577292b213fceb9441ffa7ba4db450dc109dbb7c92` |
| `contrast_sample_membership` | `diseases/MONDO_0005083_psoriasis/results/psoriasis_contrast_sample_membership_receipts_latest.json` | `d74ccb998cbfee391114b49fd47c13428b38278d1515df9d12928d218bc70615` |
| `feature_universe` | `diseases/MONDO_0005083_psoriasis/results/psoriasis_feature_universe_receipts_latest.json` | `acff26172635e4d661506e4cc8e5e39858346789add159d9382877af2cd37cbf` |
| `matrix_scale_audit` | `diseases/MONDO_0005083_psoriasis/results/psoriasis_matrix_scale_audit_receipts_latest.json` | `a8fb066d75f469f968aafffbf2602af1b4a315cef0b26571d3951ceed05658dd` |
| `normalization_method` | `diseases/MONDO_0005083_psoriasis/results/psoriasis_normalization_method_receipts_latest.json` | `2a607f55fbb8e68f94b315e1ec9240e3b55128a36ce6dec72b60c1c565e3d25f` |
| `missingness_outlier` | `diseases/MONDO_0005083_psoriasis/results/psoriasis_missingness_outlier_receipts_latest.json` | `1f0e0bebfde3c8b8c6611036119a7470f5e560e64e830b6b13ffcb21452b46f8` |
| `contrast_normalization_targets` | `diseases/MONDO_0005083_psoriasis/results/psoriasis_contrast_normalization_targets_latest.json` | `70be591c5d1072d936b3c1d6146187ca9df0e6c4b2bc37bb356c44c67c272dff` |
| `module_input_queue` | `diseases/MONDO_0005083_psoriasis/results/psoriasis_module_input_queue_latest.json` | `708499f14ecb89080449c32781463dd39bb367c31795c07630408263a2ba4593` |
| `result_envelope_targets` | `diseases/MONDO_0005083_psoriasis/results/psoriasis_result_envelope_targets_latest.json` | `57ce45ddb454e61e771bea0df014ae4ae16749fd48ee9936a8140e1d4ebe3fb4` |
| `discovery_dossier` | `diseases/MONDO_0005083_psoriasis/results/psoriasis_real_data_discovery_start_latest.json` | `3fbf1cdc99694dec061702925596b0f92404a5e85a67e7f235af63abd3b80e00` |

## Release Boundary

- batch_or_platform_guard_receipts
- downstream_envelope_binding_receipts
- executor release ledger
- null/falsifier/certificate execution
