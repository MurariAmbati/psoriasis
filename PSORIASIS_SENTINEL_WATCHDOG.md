# Psoriasis Result-Envelope Targets

Planned result-envelope targets for every matrix-backed psoriasis module input. These targets bind real-data matrix availability, field mapping, null/falsifier requirements, certificate requirements, and a closed claim firewall without running scientific executors.

- Result-envelope targets: 6408
- Matrix-bound input rows: 6408
- Inherited module abstentions: 21025
- Inherited contrast-unavailable abstentions: 267
- Certificates per target: 11
- Null models per target: 6
- Falsifiers per target: 8
- Target digest: `7d48f976210424a8893eea7ec3d162b35fe8c32ca788684c208ff6373cc6cfce`

## Family Targets

| Source queue | Units | Contrasts | Targets | Direct GSM | Processed bridge |
| --- | ---: | ---: | ---: | ---: | ---: |
| `anduril_rm` | 198 | 24 | 4752 | 3366 | 1386 |
| `artmethods_method` | 22 | 24 | 528 | 374 | 154 |
| `program_engine` | 10 | 24 | 240 | 170 | 70 |
| `rband_module` | 37 | 24 | 888 | 629 | 259 |

## Certificate Requirements

| Requirement | Status |
| --- | --- |
| `input_receipt_sha256` | `required_not_present` |
| `matrix_asset_sha256` | `required_not_present` |
| `field_mapping_sha256` | `required_not_present` |
| `processed_bridge_sha256_when_needed` | `required_not_present` |
| `matrix_normalization_receipt` | `required_not_present` |
| `sample_membership_receipt` | `required_not_present` |
| `null_model_receipt` | `required_not_present` |
| `falsifier_receipt` | `required_not_present` |
| `multiplicity_receipt` | `required_not_present` |
| `support_domain_receipt` | `required_not_present` |
| `claim_firewall_receipt` | `required_not_present` |

## Release Boundary

- materialize matrix-normalization receipts for each envelope target
- execute module-specific null model targets
- execute module-specific falsifier targets
- write certificate vectors for every completed target
- keep abstention inheritance attached to non-executed module and contrast rows
