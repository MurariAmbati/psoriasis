# Real-Data Psoriasis Module Evidence Prior Bridge Receipt

Module-facing bridge from psoriasis drug, target, and proteomics metadata priors into Anduril, ArtMethods, R-band, and KnownMethods planning surfaces. This does not execute modules or promote claims.

- Module families bridged: 3
- Module units covered: 1092
- Input rows covered: 27300
- Units requiring prior modalities: 468
- Units missing prior modalities: 357
- Units routable to prior evidence: 547
- Matrix-bound executor-blocked rows: 6168
- ChEMBL indication rows: 260
- Open Targets direct associated targets: 6963
- PRIDE files: 148
- ChEMBL mechanism targets bridged: 5
- Target components bridged: 7
- Matched target Ensembl IDs: 6
- Target-component feature hits: 28
- Target hit feature universes: 3
- Mirrored small proteomics files: 12
- Mirrored small proteomics bytes: 6433305
- Parsed proteomics feature files: 12
- Human proteomics feature rows: 21179
- Direct proteomics target-symbol hits: 0
- Proteomics contrast-readiness targets: 12
- Proteomics detected-both contrast feature rows: 54143
- Proteomics primary missingness-filter feature rows: 34819
- Open-source PRIDE search candidates: 31
- Open-source GEO broad psoriasis records: 621
- Open-source GEO indexed download candidates: 32
- Open-source ChEMBL unique molecules: 216
- Biological discovery claims promoted: 0
- Bridge digest: `038eebec1777791d04e8efcdb24ce695004d8e29ba931bcde86564d9c6ebc4c5`

## Module Connection Discoveries

- Drug-response priors now have explicit module-family gap counts for Anduril, ArtMethods, and R-band planning.
- Proteomics priors now have explicit module-family gap counts and PRIDE raw/derived admission boundaries.
- Target-evidence priors now have Open Targets association counts and cross-source axis routing for modules that require target evidence.
- ChEMBL mechanism targets now have component-level identifier bridges to Open Targets Ensembl rows before module consumption.
- Target identifier priors now have target-feature universe bindings for TNF, IL12B, IL12A, IL23A, IL17A, and IL17RA in three real processed psoriasis matrices.
- Proteomics priors now include 12 mirrored small derived PRIDE files with local digests while raw mass-spectrometry files remain blocked.
- Proteomics feature priors now include parsed human protein-group matrices and a mouse protein workbook, with no direct IL/TNF target-symbol overlap in admitted proteomics features.
- Proteomics contrast priors now include 12 grouped layer/condition contrast-readiness targets while paired design, normalization, and execution remain blocked.
- Proteomics missingness priors now include thresholded filter candidates, retaining 34,819 feature rows at the primary four-observed-samples-per-group gate.
- Open-source discovery priors now include live PRIDE/GEO/ChEMBL/Open Targets metadata-search evidence for additional psoriasis proteomics, drug-response, single-cell, spatial, drug, and target-evidence admission queues.
- KnownMethods remains a seed-plan surface with no harvested method corpus; it can consume priors only after literature-method enumeration.

## Prior Modalities

| Modality | Evidence units | Required units | Missing rows | Status |
| --- | ---: | ---: | ---: | --- |
| `drug_response` | 260 | 269 | 6725 | `prior_available_not_executor_released` |
| `proteomics` | 148 | 113 | 2825 | `prior_available_not_executor_released` |
| `target_evidence` | 6963 | 234 | 0 | `prior_available_not_executor_released` |

## Family Bridges

| Family | Units | Requiring priors | Missing priors | Routable | Missing rows |
| --- | ---: | ---: | ---: | ---: | --- |
| `anduril_rm` | 650 | 180 | 134 | 259 | `{'drug_response': 2875, 'proteomics': 475, 'target_evidence': 0}` |
| `artmethods_method` | 202 | 82 | 55 | 82 | `{'drug_response': 1050, 'proteomics': 375, 'target_evidence': 0}` |
| `rband_module` | 240 | 206 | 168 | 206 | `{'drug_response': 2800, 'proteomics': 1975, 'target_evidence': 0}` |

## Prior Axes

| Axis | ChEMBL hits | Open Targets hits | Status |
| --- | ---: | ---: | --- |
| `il12_axis` | 1 | 4 | `shared_prior_axis` |
| `il17_axis` | 2 | 6 | `shared_prior_axis` |
| `il23_axis` | 2 | 2 | `shared_prior_axis` |
| `il36_axis` | 0 | 1 | `single_source_prior_axis` |
| `tnf_axis` | 1 | 2 | `shared_prior_axis` |
| `tyk2_axis` | 0 | 2 | `single_source_prior_axis` |

## Top Prior Gap Units


### anduril_rm

| Unit | Missing rows | Modalities | Title |
| --- | ---: | --- | --- |
| `RM0008` | 25 | `{'proteomics': 25}` | Plain-baseline dominance test (DeLong + reclassification) as an earned-complexity gate |
| `RM0025` | 25 | `{'drug_response': 25}` | Positivity/overlap diagnostics with principled abstain |
| `RM0026` | 25 | `{'drug_response': 25}` | Double-negative-control (proximal g-computation) treatment effects |
| `RM0030` | 25 | `{'drug_response': 25}` | Double machine learning with cross-fitting for nuisance orthogonalization |
| `RM0031` | 25 | `{'drug_response': 25}` | Targeted minimum-loss estimation (TMLE) wrapper for any plug-in feature |
| `RM0040` | 25 | `{'drug_response': 25}` | Immortal-time-bias guard for treatment/exposure cohorts |
| `RM0089` | 25 | `{'drug_response': 25}` | Endotype treatment interaction scan |
| `RM0104` | 25 | `{'drug_response': 25}` | Truncal-versus-branch lesion classifier and therapeutic-anchor selector |

### artmethods_method

| Unit | Missing rows | Modalities | Title |
| --- | ---: | --- | --- |
| `D7.1` | 50 | `{'drug_response': 25, 'proteomics': 25}` | RNA-protein discordance (CCLE) |
| `D7.7` | 50 | `{'drug_response': 25, 'proteomics': 25}` | Protein/RNA ratio stability biomarker |
| `D1.10` | 25 | `{'drug_response': 25}` | Blast%/age/WBC continuous prognosis |
| `D1.4` | 25 | `{'drug_response': 25}` | Tertile/quartile dose-response prognosis |
| `D1.8` | 25 | `{'drug_response': 25}` | Mutation univariate prognosis (BeatAML) |
| `D1.9` | 25 | `{'proteomics': 25}` | Protein univariate prognosis |
| `D10.1` | 25 | `{'drug_response': 25}` | Label-permutation FDR calibration |
| `D10.3` | 25 | `{'drug_response': 25}` | Negative-control drug set |

### rband_module

| Unit | Missing rows | Modalities | Title |
| --- | ---: | --- | --- |
| `CF05` | 50 | `{'drug_response': 25, 'proteomics': 25}` | Structure/affinity consensus |
| `CI03` | 50 | `{'drug_response': 25, 'proteomics': 25}` | Dynamic signaling state-space |
| `CI07` | 50 | `{'drug_response': 25, 'proteomics': 25}` | Rescue and compensation predictor |
| `DG00` | 50 | `{'drug_response': 25, 'proteomics': 25}` | Inhibition-versus-degradation triage |
| `DG01` | 50 | `{'drug_response': 25, 'proteomics': 25}` | E3 ligase context atlas |
| `DG02` | 50 | `{'drug_response': 25, 'proteomics': 25}` | Warheadligaselinker object compiler |
| `DG03` | 50 | `{'drug_response': 25, 'proteomics': 25}` | Linker generation and conformer enumeration |
| `DG04` | 50 | `{'drug_response': 25, 'proteomics': 25}` | Ternary-complex structure generation |

## KnownMethods

- Seed queries: 600
- Method records: 0
- Status: `seed_plan_only_no_harvested_method_corpus`

## Not Yet Discovered

- No module has consumed these priors in a scientific execution.
- No prior has been promoted to a validated discovery, therapeutic claim, or biomarker.
- No proteomics raw file, drug-response assay matrix, or target-evidence transform has been released as an execution input.
- No target identifier bridge has been consumed by a released scientific executor.

## Release Boundary

- per-module feature-use contracts that consume target-feature binding rows without promoting claims
- proteomics normalization method receipts for missingness-filter candidate feature sets
- drug-response assay matrix admission before treatment-response modules execute
- per-family null/falsifier/certificate bindings for any prior-consuming module run
