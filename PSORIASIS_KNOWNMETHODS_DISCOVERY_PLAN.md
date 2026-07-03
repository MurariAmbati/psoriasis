# Real-Data Psoriasis Modality GEO Adapter Receipt

Adapter-source receipt over the downloaded psoriasis modality GEO payloads. This discovers real sample, matrix, and next-file structure without executing modules or promoting biological claims.

- Downloaded payloads checked: 20
- Local payload SHA-256 matches: 20
- Parsed series matrices: 7
- Sample metadata units: 950
- Processed matrices probed: 2
- GEO filelists parsed: 5
- Biological discovery claims promoted: 0
- Receipt digest: `14ba1303ce2bc41d30edcb8be88a32ece5c3866adc1e35457bc6c0e6179b7fc2`

## Discoveries So Far

- The psoriasis modality chain has admitted 20 real GEO payloads from seven accessions and verified local SHA-256 custody for the downloaded files.
- Seven downloaded series matrices expose 950 real GEO sample metadata units with phenotype and tissue fields on every parsed unit.
- Two downloaded processed matrices are structurally readable and expose feature/sample dimensions for later matrix bridge work.
- Five downloaded GEO supplementary filelists expose the next candidate raw, processed, and single-cell component files to review under size/access gates.
- Proteomics, ChEMBL drug indications, Open Targets associations, CELLxGENE, and NYU spatial catalogue evidence are currently discovered as metadata/file-manifest opportunities, not executed biology.

## Not Yet Discovered

- No validated repressor, target, pathway, drug responder, proteomic marker, or biomarker has been promoted.
- No adapter has been released for scientific module execution from the new modality GEO payloads.
- No raw human single-cell, bulk RAW tar, or PRIDE proteomics raw file has been mirrored by this adapter receipt.

## Candidate Field Coverage

| Category | Samples |
| --- | ---: |
| `age` | 0 |
| `lesion_or_severity` | 192 |
| `phenotype_or_diagnosis` | 950 |
| `sex` | 0 |
| `subject_identity` | 463 |
| `technical_or_batch` | 271 |
| `tissue_or_region` | 950 |
| `treatment_or_exposure` | 215 |

## Accessions

| Accession | Modalities | Files | Samples | Processed matrices | Next file classes |
| --- | --- | ---: | ---: | ---: | --- |
| `GSE106992` | drug_response, expression, ustekinumab, etanercept | 3 | 192 | 0 | `{'archive_blocked': 1, 'microarray_raw_cel_next_candidate': 192}` |
| `GSE117468` | drug_response, expression, clinical_trial, brodalumab | 1 | 0 | 0 | `{'archive_blocked': 1, 'microarray_raw_cel_next_candidate': 565}` |
| `GSE150672` | single_cell, expression, inflammatory_skin_disease | 5 | 438 | 1 | `{'archive_blocked': 1, 'processed_matrix_next_candidate': 45}` |
| `GSE151177` | single_cell, expression, immune_cells, keratinocyte | 3 | 23 | 0 | `{'archive_blocked': 1, 'metadata_only_unclassified': 23, 'processed_matrix_next_candidate': 46}` |
| `GSE162183` | single_cell, expression, skin, healthy_control | 2 | 6 | 0 | `{}` |
| `GSE171012` | drug_response, expression, cell_subset, secukinumab | 3 | 271 | 1 | `{}` |
| `GSE228421` | single_cell, drug_response, risankizumab, longitudinal | 3 | 20 | 0 | `{'archive_blocked': 1, 'oversized_blocked': 19, 'single_cell_component_next_candidate': 41}` |

## Processed Matrix Probes

| Accession | Matrix | Features | Sample columns | SHA matched |
| --- | --- | ---: | ---: | --- |
| `GSE171012` | `GSE171012_CountData_SecukinumabPsoRnaSeq_20210324.tsv.gz` | 58037 | 271 | true |
| `GSE150672` | `GSE150672_rsem.genes.count.matrix.txt.gz` | 23686 | 384 | true |

## Filelist Next Admission Classes

| Class | Files | Bytes |
| --- | ---: | ---: |
| `archive_blocked` | 5 | 5271111680 |
| `metadata_only_unclassified` | 23 | 159877773 |
| `microarray_raw_cel_next_candidate` | 757 | 2380000161 |
| `oversized_blocked` | 19 | 2292170549 |
| `processed_matrix_next_candidate` | 91 | 79457266 |
| `single_cell_component_next_candidate` | 41 | 358855922 |

## Top Candidate Fields

| Category | Field | Sample coverage | Accessions |
| --- | --- | ---: | ---: |
| `tissue_or_region` | `tissue` | 512 | 5 |
| `subject_identity` | `subject id` | 463 | 2 |
| `phenotype_or_diagnosis` | `condition` | 438 | 1 |
| `phenotype_or_diagnosis` | `sample type` | 438 | 1 |
| `phenotype_or_diagnosis` | `clinical status` | 271 | 1 |
| `technical_or_batch` | `sequencing batch` | 271 | 1 |
| `technical_or_batch` | `sequencing lane` | 271 | 1 |
| `tissue_or_region` | `cell type` | 271 | 1 |
| `treatment_or_exposure` | `treatment` | 215 | 2 |
| `lesion_or_severity` | `pasi75resp` | 192 | 1 |
| `phenotype_or_diagnosis` | `patient diagnosis` | 192 | 1 |
| `subject_identity` | `patient diagnosis` | 192 | 1 |
| `tissue_or_region` | `skin type` | 192 | 1 |
| `treatment_or_exposure` | `time` | 192 | 1 |
| `phenotype_or_diagnosis` | `disease state` | 49 | 3 |

## Next Required

- Bind series-matrix candidate fields into explicit contrast definitions.
- Bridge processed matrix sample columns to parsed sample units and reject ambiguous columns.
- Admit specific filelist rows one batch at a time with checksum, size, privacy, and license gates.
- Build PRIDE proteomics raw-file admission tiers separately from metadata because the current file manifest is hundreds of gigabytes.
- Use ChEMBL and Open Targets slices as target/drug priors only after versioned evidence transforms and claim certificates exist.
