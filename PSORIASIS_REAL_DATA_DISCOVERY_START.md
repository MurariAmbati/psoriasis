# Real-Data Psoriasis Proteomics Feature-Universe Receipt

Parsed feature-universe receipt for admitted small PRIDE proteomics files. This records real protein feature coverage and schema boundaries only; no scientific execution or biological claim is released.

- Parsed files: 12
- Abundance feature files: 5
- Human protein-group matrices: 4
- Human protein-group feature rows: 21179
- Human sample/run columns: 96
- Human nonempty abundance cells: 321399
- Mouse workbook protein rows: 7747
- Direct IL/TNF target-symbol hits in admitted proteomics: 0
- Biological discovery claims promoted: 0
- Receipt digest: `5e3e482899b7b23f39cb43b93e5cb1b9091235e856ec044bf8bbe0528ee8a674`

## Discoveries So Far

- PXD063539 now contributes four real human psoriasis spatial-layer DIA-NN protein-group abundance matrices covering outer epidermis, inner epidermis, dermis, and subcutis.
- Those four human matrices provide 21,179 layer-specific protein-group feature rows and 96 sample/run columns across lesional, nonlesional, and healthy skin-layer contexts.
- PXD077433 now contributes a parsed mouse psoriasis-like intervention workbook with 7,747 protein rows and three abundance-ratio columns.
- Current admitted proteomics feature universes have no direct IL/TNF target-symbol hits for TNF, IL12B, IL12A, IL23A, IL17A, or IL17RA, so target-feature bridging remains transcriptomics-only until larger/raw proteomics admission or identifier expansion is added.

## Parsed Files

| File | Role | Species | Features/Rows | Samples | Target hits |
| --- | --- | --- | ---: | ---: | ---: |
| `Metadata_PsoLayers_Moeller_et_al.csv` | `proteomics_layer_metadata` | `Homo sapiens` | 15 | 0 | 0 |
| `OuterEpidermis_DIANN181_MBR.stats_deidentified.tsv` | `diann_run_quality_statistics` | `Homo sapiens` | 24 | 0 | 0 |
| `Dermis_DIANN181_MBR.stats_deidentified.tsv` | `diann_run_quality_statistics` | `Homo sapiens` | 24 | 0 | 0 |
| `InnerEpidermis_DIANN181_MBR.stats_deidentified.tsv` | `diann_run_quality_statistics` | `Homo sapiens` | 24 | 0 | 0 |
| `Subcutis_DIANN181_MBR.stats_deidentified.tsv` | `diann_run_quality_statistics` | `Homo sapiens` | 24 | 0 | 0 |
| `OuterEpidermis_DIANN181_MBR.pg_matrix_deidentified.tsv` | `protein_group_abundance_matrix` | `Homo sapiens` | 4749 | 24 | 0 |
| `Subcutis_DIANN181_MBR.pg_matrix_deidentified.tsv` | `protein_group_abundance_matrix` | `Homo sapiens` | 4803 | 24 | 0 |
| `Dermis_DIANN181_MBR.pg_matrix_deidentified.tsv` | `protein_group_abundance_matrix` | `Homo sapiens` | 5247 | 24 | 0 |
| `InnerEpidermis_DIANN181_MBR.pg_matrix_deidentified.tsv` | `protein_group_abundance_matrix` | `Homo sapiens` | 6380 | 24 | 0 |
| `checksum.txt` | `checksum_manifest` | `mixed_or_project_manifest` | 17 | 0 | 0 |
| `checksum.txt` | `checksum_manifest` | `mixed_or_project_manifest` | 17 | 0 | 0 |
| `psoriasis_proteomics.xlsx` | `protein_workbook_abundance_ratio_table` | `Mus musculus` | 7747 | 0 | 0 |

## Human Protein Matrices

| Layer | Features | Samples | Nonempty cells | Missing cells | Conditions |
| --- | ---: | ---: | ---: | ---: | --- |
| `outer_epidermis` | 4749 | 24 | 59090 | 54886 | `{'healthy': 8, 'lesional': 8, 'nonlesional': 8}` |
| `subcutis` | 4803 | 24 | 66914 | 48358 | `{'healthy': 8, 'lesional': 8, 'nonlesional': 8}` |
| `dermis` | 5247 | 24 | 80632 | 45296 | `{'healthy': 8, 'lesional': 8, 'nonlesional': 8}` |
| `inner_epidermis` | 6380 | 24 | 114763 | 38357 | `{'healthy': 8, 'lesional': 8, 'nonlesional': 8}` |

## Not Yet Discovered

- No protein abundance matrix has been normalized, contrasted, or released for scientific execution.
- No protein feature has been joined to ChEMBL/Open Targets target components.
- No raw mass-spectrometry file or large derived search library has been admitted by this receipt.
- No proteomic marker, pathway, drug response, or repression claim has been promoted.

## Release Boundary

- add protein identifier crosswalk receipts for UniProt, Ensembl, and gene symbols
- write proteomics normalization and missingness receipts for abundance matrices
- define layer/condition contrasts and falsifier gates before module execution
