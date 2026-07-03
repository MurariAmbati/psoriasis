# Psoriasis Vindicate Interception

Disease-pack Vindicate run for psoriasis interception and treatment-response discovery inputs. The report binds source axes and handoff requirements while blocking treatment, candidate-tool, and response claims.

- Program status: `vindicate_interception_inputs_bound_executor_blocked`
- Samples: 1528
- Treatment/exposure samples: 635
- Pasi75 responders: 231
- Pasi75 nonresponders: 93
- Result-envelope handoffs: 6408
- Report digest: `a7818a8d04bcbc23a2dd46163f5d0dd44fd9476bc03928fa833312eb7f240ba7`

## Interception Lanes

| Lane | Status | Contrasts | Role |
| --- | --- | ---: | --- |
| `skin_lesion_state_interception` | `inputs_bound_executor_blocked` | 11 | lesional versus nonlesional discovery axis for reversible inflammatory skin state hypotheses |
| `psoriasis_control_divergence` | `inputs_bound_executor_blocked` | 10 | psoriasis versus healthy or normal skin divergence axis |
| `treatment_response_interception` | `inputs_bound_executor_blocked` | 2 | PASI75 responder/nonresponder and treatment-time source axes without response claims |
| `severity_source_axis` | `source_axis_only_overclaim_blocked` | 1 | mild/severe source contrast and PASI availability require endpoint certificates before severity claims |
| `target_and_tool_handoff` | `result_envelope_targets_planned_executor_blocked` | 24 | candidate target/tool hypotheses remain in result-envelope targets until nulls, falsifiers, and certificates exist |

## Response Source Evidence

| Accession | Contrast | Left | Right |
| --- | --- | ---: | ---: |
| `GSE117239` | `pasi75_responder_vs_nonresponder` | 231 | 93 |
| `GSE53552` | `baseline_or_predose_treatment_axis` | 49 | 50 |

## Handoff Requirements

- `result_envelope_target_count`: 6408
- `required_certificate_count_per_target`: 11
- `null_model_target_count_per_target`: 6
- `falsifier_target_count_per_target`: 8
- `executor_release_present`: False
- `intervention_claim_allowed`: False

## Next Required Receipts

- batch_or_platform_guard_receipts
- downstream_envelope_binding_receipts
- null_model_execution_receipts
- falsifier_execution_receipts
- claim_certificate_vectors
