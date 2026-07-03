# Psoriasis Sentinel Watchdog

Disease-pack Sentinel run over psoriasis real-data receipts. It audits claim/firewall status, review gates, abstentions, and overclaim hazards before any executor release.

- Watchdog status: `completed_psoriasis_receipt_watchdog`
- Source artifacts: 11
- Sentinel checks: 7
- Clean checks: 2
- Watchlist checks: 5
- Genuine overclaims: 0
- Report digest: `ea7c49304f0d6299a2c588f5cad4cba8d5a433833d03223941d470d1b829a583`

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

## Checks

| Check | Status | Observed | Finding |
| --- | --- | ---: | --- |
| `scientific_claim_firewall` | `clean` | 0 | No scientific result rows have been written for psoriasis. |
| `matrix_materialization_firewall` | `clean` | False | Normalization targets remain materialization-blocked. |
| `missingness_outlier_review_gate` | `watchlist` | 8 | Review-gated outlier or method profiles must be adjudicated before normalized matrices are released. |
| `module_abstention_bulk` | `watchlist` | 21025 | Module abstentions remain explicit and must not be counted as executed discoveries. |
| `contrast_matrix_unavailable_abstention` | `watchlist` | 267 | One field-ready contrast lacks a selected matrix asset and is propagated as abstention rows. |
| `lesion_severity_overclaim_guard` | `watchlist` | 307 | Lesion/nonlesion and mild/severe source axes are discovery inputs, not severity claims. |
| `treatment_response_overclaim_guard` | `watchlist` | 231 | Responder labels are field-mapped inputs only; no treatment-response claim is promoted. |

## Watchlist Focus

| Check | Observed | Finding |
| --- | ---: | --- |
| `missingness_outlier_review_gate` | 8 | Review-gated outlier or method profiles must be adjudicated before normalized matrices are released. |
| `module_abstention_bulk` | 21025 | Module abstentions remain explicit and must not be counted as executed discoveries. |
| `contrast_matrix_unavailable_abstention` | 267 | One field-ready contrast lacks a selected matrix asset and is propagated as abstention rows. |
| `lesion_severity_overclaim_guard` | 307 | Lesion/nonlesion and mild/severe source axes are discovery inputs, not severity claims. |
| `treatment_response_overclaim_guard` | 231 | Responder labels are field-mapped inputs only; no treatment-response claim is promoted. |

## Release Boundary

- adjudicate review-gated matrix profiles
- write batch/platform guards
- write downstream envelope binding receipts
- rerun sentinel after any executor release
