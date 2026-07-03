# Real-Data Psoriasis Proteomics Derived-File Admission Receipt

Small derived PRIDE proteomics file admission for psoriasis. Files are mirrored and hashed, but no parser, quantification, module execution, or biological claim is released.

- Selected small derived files: 12
- Stored small derived files: 12
- Stored bytes: 6433305
- Blocked raw files: 108
- Blocked larger derived candidates: 28
- Projects represented: 3
- Biological discovery claims promoted: 0
- Admission digest: `ea4300ca13091f7b1d72fdaf63d0720a275ec02ec57c8d971e24431d4db79e45`

## Discoveries So Far

- Small derived PRIDE proteomics files can now be mirrored with source URLs, local SHA-256 digests, byte counts, and per-file execution gates.
- PXD063539 contributes deidentified psoriasis skin-layer metadata, DIA-NN statistics, and protein-group matrices for dermis, inner epidermis, outer epidermis, and subcutis.
- PXD077433 contributes a small psoriasis_proteomics.xlsx file for an IMQ/clove/eugenol psoriasis-like intervention model, plus a checksum file.
- PXD063928 contributes only a small checksum file at this gate; its proteomics payloads remain blocked until the large-derived/raw policy is expanded.
- Target feature coverage for TNF, IL12B, IL12A, IL23A, IL17A, and IL17RA is available for later protein/gene identifier joins, but no protein abundance has been mapped yet.

## Admitted Files

| Project | File | Category | Bytes | Text shape | SHA-256 |
| --- | --- | --- | ---: | --- | --- |
| `PXD063539` | `Metadata_PsoLayers_Moeller_et_al.csv` | `Other type file URI` | 2708 | yes | `7ac1c923fd4dac74061bb464960344d493acdcfe6c1d7cbb4806427776f61d41` |
| `PXD063539` | `OuterEpidermis_DIANN181_MBR.stats_deidentified.tsv` | `Search engine output file URI` | 6209 | yes | `aea648d7818a7a331ab1e49bc7614a329ef7ac87706b55cbde11a06c1dae44c0` |
| `PXD063539` | `Dermis_DIANN181_MBR.stats_deidentified.tsv` | `Search engine output file URI` | 6234 | yes | `d3c459a0f8f69557dba6de7cc857b2a2a4913b7fe85015547beccc00dc1ca740` |
| `PXD063539` | `InnerEpidermis_DIANN181_MBR.stats_deidentified.tsv` | `Search engine output file URI` | 6247 | yes | `8d34612912eff048582dc2eba964284970d0ff33e0ceba36a69f0d2d28b2901d` |
| `PXD063539` | `Subcutis_DIANN181_MBR.stats_deidentified.tsv` | `Search engine output file URI` | 6247 | yes | `610edf847f8c1e9e692b09c270e079107b04ae6811388a925517f250fc39f985` |
| `PXD063539` | `OuterEpidermis_DIANN181_MBR.pg_matrix_deidentified.tsv` | `Search engine output file URI` | 632762 | yes | `7951a3deae61adbf6c94eef8c05296f301f2f90fd590881c9bdecb7893a27e58` |
| `PXD063539` | `Subcutis_DIANN181_MBR.pg_matrix_deidentified.tsv` | `Search engine output file URI` | 688597 | yes | `2804e24bdbfef1a0dd0afb7d18d7f8676ae7389a06b9d7df2fda45bcd8b554eb` |
| `PXD063539` | `Dermis_DIANN181_MBR.pg_matrix_deidentified.tsv` | `Search engine output file URI` | 803553 | yes | `2877358e8cfa1136e4c7cde44d924be8b6b27606fb2883f917b88422fcd0c4d5` |
| `PXD063539` | `InnerEpidermis_DIANN181_MBR.pg_matrix_deidentified.tsv` | `Search engine output file URI` | 1090898 | yes | `357f03d7c06930c4052d7f2de3bce3c260f3d9f5015908312787546a9af80315` |
| `PXD063928` | `checksum.txt` | `Other type file URI` | 3113 | yes | `763c7c64cecda27c2ff97c4940ce3df6fdb591246f1d6997fa2e0fdc52836d65` |
| `PXD077433` | `checksum.txt` | `Other type file URI` | 2250 | yes | `6b9367164c6e3a1d2206121380c519d4f16d2b65355b1dadc16caf1e888765bf` |
| `PXD077433` | `psoriasis_proteomics.xlsx` | `Search engine output file URI` | 3184487 | no | `04e39305a8e66cb2bfac94049152f4e888df34ec4b0ae74fbbe06d3ab7c04b9d` |

## Blocked Larger Derived Candidates

| Project | Files | Bytes |
| --- | ---: | ---: |
| `PXD001387` | 24 | 6657460416 |
| `PXD021673` | 1 | 627905353 |
| `PXD035174` | 1 | 3644280832 |
| `PXD063539` | 1 | 855063012 |
| `PXD063928` | 1 | 259893862 |

## Not Yet Discovered

- No proteomics file has been parsed into a protein abundance feature universe.
- No UniProt, gene-symbol, or Ensembl mapping has been joined from these files to target components.
- No PRIDE raw mass-spectrometry payload has been mirrored, searched, quantified, or normalized.
- No protein marker, pathway, drug-response, or repression claim has been promoted.

## Release Boundary

- parse admitted TSV/CSV/XLSX schemas into protein-feature universe receipts
- separate checksum/metadata-only files from abundance matrices
- map UniProt and gene-symbol protein identifiers to target-feature binding symbols
- require proteomics normalization, missingness, batch, falsifier, and claim-certificate receipts before discoveries are promoted
