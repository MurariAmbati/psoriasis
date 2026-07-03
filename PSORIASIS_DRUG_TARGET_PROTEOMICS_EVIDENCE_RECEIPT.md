# Psoriasis GEO Field-Mapping Receipt

Accession-specific mapping of admitted psoriasis GEO sample metadata into reviewable disease, skin-region, severity, treatment, timepoint, response, and subject fields. This receipt advances field mapping but still blocks matrix materialization and scientific result execution.

- Sample units: 1528
- Field-mapped samples: 1407
- Review-gated samples: 121
- Contrast rows: 91
- Contrast-ready rows: 25
- Contrast abstentions: 66
- Field mapping digest: `b91c4c3c4d7516740e7189bc2bcd4a271e4d79a5612f182424dac39b84a4458f`

## Class Counts

| Class | Counts |
| --- | --- |
| Disease | `atopic_dermatitis_comparator`=54, `healthy_or_normal_control`=223, `psoriasis`=1072, `unmapped`=179 |
| Skin region | `lesional`=746, `nonlesional`=420, `normal_or_healthy_skin`=205, `skin_unspecified`=157 |
| Severity | `mild_explicit`=14, `pasi_numeric_available`=307, `severe_explicit`=183, `unmapped`=1024 |
| Treatment | `adalimumab`=89, `brodalumab`=40, `etanercept`=131, `methotrexate`=90, `placebo`=10, `pre_treatment_or_baseline`=82, `unmapped`=893, `ustekinumab`=193 |
| Timepoint | `baseline_or_predose`=249, `day_15`=25, `day_43`=20, `day_8`=5, `unmapped`=953, `week_1`=187, `week_16`=29, `week_2`=30, `week_4`=30 |
| Response | `pasi75_nonresponder`=93, `pasi75_responder`=231, `unmapped`=1204 |

## Accession Mapping Status

| Accession | Status counts |
| --- | --- |
| `GSE117239` | `field_mapped_paired_psoriasis`=324 |
| `GSE121212` | `field_mapped_source_view`=147 |
| `GSE13355` | `field_mapped_paired_psoriasis`=116, `field_mapped_source_view`=64 |
| `GSE14905` | `field_mapped_source_view`=82 |
| `GSE30999` | `field_mapped_paired_psoriasis`=170 |
| `GSE34248` | `field_mapped_source_view`=28 |
| `GSE41662` | `field_mapped_source_view`=48 |
| `GSE53552` | `field_mapped_paired_psoriasis`=99 |
| `GSE54456` | `field_mapped_source_view`=174 |
| `GSE66511` | `field_mapped_source_view`=36 |
| `GSE67785` | `field_mapped_paired_psoriasis`=28 |
| `GSE78097` | `field_mapped_paired_psoriasis`=27, `field_mapped_source_view`=6 |
| `GSE85034` | `field_mapped_source_view`=58, `review_gated`=121 |

## Ready Contrasts

| Accession | Contrast | Left | Right | Paired possible |
| --- | --- | ---: | ---: | --- |
| `GSE117239` | `lesional_vs_nonlesional` | 240 | 84 | true |
| `GSE117239` | `pasi75_responder_vs_nonresponder` | 231 | 93 | false |
| `GSE121212` | `lesional_vs_nonlesional` | 55 | 54 | true |
| `GSE121212` | `lesional_vs_normal` | 55 | 38 | false |
| `GSE121212` | `psoriasis_vs_atopic_dermatitis` | 55 | 54 | false |
| `GSE121212` | `psoriasis_vs_healthy_or_normal` | 55 | 38 | false |
| `GSE13355` | `lesional_vs_nonlesional` | 58 | 58 | true |
| `GSE13355` | `lesional_vs_normal` | 58 | 64 | false |
| `GSE13355` | `psoriasis_vs_healthy_or_normal` | 116 | 64 | false |
| `GSE14905` | `lesional_vs_nonlesional` | 33 | 28 | true |
| `GSE14905` | `lesional_vs_normal` | 33 | 21 | false |
| `GSE14905` | `psoriasis_vs_healthy_or_normal` | 61 | 21 | false |
| `GSE30999` | `lesional_vs_nonlesional` | 85 | 85 | true |
| `GSE34248` | `lesional_vs_nonlesional` | 14 | 14 | true |
| `GSE41662` | `lesional_vs_nonlesional` | 24 | 24 | true |
| `GSE53552` | `lesional_vs_nonlesional` | 75 | 24 | true |
| `GSE53552` | `baseline_or_predose_treatment_axis` | 49 | 50 | false |
| `GSE54456` | `lesional_vs_normal` | 92 | 82 | false |
| `GSE54456` | `psoriasis_vs_healthy_or_normal` | 92 | 82 | false |
| `GSE66511` | `psoriasis_vs_healthy_or_normal` | 24 | 12 | false |
| `GSE67785` | `lesional_vs_nonlesional` | 14 | 14 | true |
| `GSE78097` | `lesional_vs_nonlesional` | 27 | 6 | true |
| `GSE78097` | `psoriasis_vs_healthy_or_normal` | 27 | 6 | false |
| `GSE78097` | `mild_vs_severe_source_axis` | 14 | 13 | false |
| `GSE85034` | `lesional_vs_nonlesional` | 29 | 29 | true |

## Release Boundary

- bind expression matrix rows/columns to mapped sample ids
- write per-contrast matrix availability receipts
- run differential/statistical modules into result envelopes
- attach null/falsifier certificates before any promoted claim
