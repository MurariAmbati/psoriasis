# Psoriasis Deep Module Discovery Run

Aggregate report for psoriasis Anduril, ArtMethods, R-band, and KnownMethods discovery planning over the admitted real-data receipt chain.

- Source artifacts: 10
- Unit reports: 1092
- Matrix-bound rows across Anduril/ArtMethods/R-band: 6168
- KnownMethods seed queries: 600
- Aggregate digest: `ba61d394168fcac26d0716f736caa97a41b0ed5c759a2f73c8581d06a2472d3d`

## Family Reports

| Family | Units | Matrix-bound rows | Digest |
| --- | ---: | ---: | --- |
| `anduril_rm` | 650 | 4752 | `7c87bc7bac5c02583841c40a33602b8f83a81f8843caf60593eccb0b18d012ea` |
| `artmethods_method` | 202 | 528 | `5b7241be283d2e1bbbe34708769bea6cbdbd90bbd2e88eff6e1e1cef143f5866` |
| `rband_module` | 240 | 888 | `6e9396c847a7f1fc9e5f42d76391a9ba564d16d07a7595a1ce6f04353d1ac0bb` |
| `knownmethods` | 0 |  | `958df0507da7c73713f352a81ca05e7b5b3efde67ed3735aea9f326ae2475f7c` |

## Queue States

| Family | Input rows | Matrix-bound | Module abstentions | Contrast unavailable | Top missing modality |
| --- | ---: | ---: | ---: | ---: | --- |
| `anduril_rm` | 16250 | 4752 | 11300 | 198 | `mutation` |
| `artmethods_method` | 5050 | 528 | 4500 | 22 | `survival` |
| `rband_module` | 6000 | 888 | 5075 | 37 | `drug_response` |

## Source Artifacts

| Artifact | Path | Digest |
| --- | --- | --- |
| `module_input_queue` | `diseases/MONDO_0005083_psoriasis/results/psoriasis_module_input_queue_latest.json` | `708499f14ecb89080449c32781463dd39bb367c31795c07630408263a2ba4593` |
| `contrast_normalization_targets` | `diseases/MONDO_0005083_psoriasis/results/psoriasis_contrast_normalization_targets_latest.json` | `70be591c5d1072d936b3c1d6146187ca9df0e6c4b2bc37bb356c44c67c272dff` |
| `result_envelope_targets` | `diseases/MONDO_0005083_psoriasis/results/psoriasis_result_envelope_targets_latest.json` | `57ce45ddb454e61e771bea0df014ae4ae16749fd48ee9936a8140e1d4ebe3fb4` |
| `discovery_dossier` | `diseases/MONDO_0005083_psoriasis/results/psoriasis_real_data_discovery_start_latest.json` | `3fbf1cdc99694dec061702925596b0f92404a5e85a67e7f235af63abd3b80e00` |
| `field_mapping` | `diseases/MONDO_0005083_psoriasis/results/psoriasis_geo_field_mapping_receipt_latest.json` | `e4c7c70a8dc585d5d6af653a3e1d46cca162e090eb8d2011bc583584c9125536` |
| `missingness_outlier` | `diseases/MONDO_0005083_psoriasis/results/psoriasis_missingness_outlier_receipts_latest.json` | `1f0e0bebfde3c8b8c6611036119a7470f5e560e64e830b6b13ffcb21452b46f8` |
| `anduril_execution_plan` | `anduril/RM_EXECUTION_PLAN.json` | `367398403be01a40eb5d0b5715735153b4439caa70e8fe91a934368680a7c431` |
| `artmethods_execution_plan` | `artmethods/METHOD_EXECUTION_PLAN.json` | `1c0ad039b71d960ec04c590f8c4bc0ecd1e762dd43b16adc60f0078bd1bb52ca` |
| `rband_execution_plan` | `docs/programs/REPRESSOME_RBAND_MODULE_EXECUTION_PLAN.json` | `71adb60f1f785776f28e11d04650f5c51f475c21fa8fc5f6cbfc5058863fa6f1` |
| `knownmethods_seeds` | `knownmethods/seeds.yaml` | `740be8fb4eb3379ebc42140098e8a8a80049e769d806f5c6298b365b17f9711f` |

## KnownMethods State

- Seed queries: 600
- Methods corpus present: false
- Method records: 0
- Experiments file present: false
- Experiment records: 0

## Release Boundary

- batch_or_platform_guard_receipts
- downstream_envelope_binding_receipts
- scientific_executor_release_ledger
- per-unit null_falsifier_certificate_vectors
- knownmethods harvest/enumeration if literature-method expansion is requested
