# Psoriasis Module Input Queue

Matrix-backed input queue connecting psoriasis real-data contrasts to Anduril, ArtMethods, R-band, and program-engine jobs. This is an input-binding and abstention ledger only; matrix materialization and scientific execution remain blocked.

- Module jobs: 1108
- Ready module jobs: 267
- Field-ready contrasts: 25
- Matrix-backed contrasts: 24
- Input rows: 27700
- Matrix-bound executor-blocked rows: 6408
- Module abstention rows: 21025
- Contrast-unavailable abstention rows: 267
- Queue digest: `e507f8367f7d43d87a10038a76749b52497f4457fe3c850f5b57d444aba638f4`

## Row States

| State | Rows |
| --- | ---: |
| `contrast_matrix_unavailable_abstention` | 267 |
| `matrix_bound_executor_blocked` | 6408 |
| `module_abstention_record` | 21025 |

## Family Summaries

| Source queue | Units | Input rows | Matrix-bound | Abstentions |
| --- | ---: | ---: | ---: | ---: |
| `anduril_rm` | 650 | 16250 | 4752 | 11498 |
| `artmethods_method` | 202 | 5050 | 528 | 4522 |
| `program_engine` | 16 | 400 | 240 | 160 |
| `rband_module` | 240 | 6000 | 888 | 5112 |

## Contrast Matrix Status

| Status | Contrasts |
| --- | ---: |
| `contrast_matrix_ready_direct_gsm` | 17 |
| `contrast_matrix_ready_processed_bridge` | 7 |
| `contrast_matrix_unavailable` | 1 |

## Release Boundary

- materialize matrix-normalization ledgers for each matrix-backed contrast
- attach per-module output envelope targets and cost gates
- emit null and falsifier certificates for every executed input row
- keep module abstentions and unavailable-contrast abstentions in the claim firewall
