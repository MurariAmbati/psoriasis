# Real-Data Psoriasis Drug, Target, And Proteomics Evidence Receipt

Evidence-prior receipt over downloaded psoriasis ChEMBL, Open Targets, and PRIDE metadata. This does not execute modules or promote biological claims.

- ChEMBL indication rows: 260
- ChEMBL unique molecules: 216
- ChEMBL clinical-trial NCT references: 1054
- Named drug mechanisms: 6
- Open Targets direct associated targets: 6963
- Open Targets indirect-enabled associated targets: 7146
- PRIDE projects: 6
- PRIDE listed files: 148
- PRIDE listed bytes: 882490484774
- Biological discovery claims promoted: 0
- Receipt digest: `a0c6d85ca70135e84c956889c22795022433ac7f4e2f87d27021ed8902adfc21`

## Discoveries So Far

- ChEMBL metadata exposes 260 psoriasis indication rows, 216 unique molecules, phase distribution, and clinical-reference structure.
- Named ChEMBL mechanism lookups expose IL-12, IL-23, IL-17, and TNF drug-axis priors for the queried psoriasis drugs.
- Open Targets metadata exposes 6963 direct and 7146 indirect-enabled psoriasis associated-target counts, with top downloaded rows for target-prior triage.
- PRIDE metadata exposes six psoriasis-relevant proteomics projects, 148 listed files, and explicit raw-versus-derived admission classes.
- Cross-source prior axes can now be tracked before execution, including IL-12, IL-23, IL-17, and TNF overlap between ChEMBL mechanisms and Open Targets top rows.

## ChEMBL

| Field | Count |
| --- | ---: |
| phase `0.5` | 2 |
| phase `1.0` | 54 |
| phase `2.0` | 105 |
| phase `3.0` | 26 |
| phase `4.0` | 73 |
| reference `ATC` | 17 |
| reference `ClinicalTrials` | 239 |
| reference `DailyMed` | 153 |
| reference `EMA` | 21 |
| reference `FDA` | 8 |
| reference `USAN` | 9 |

## Named Drug Mechanisms

| Query | ChEMBL | Mechanisms | Axes |
| --- | --- | ---: | --- |
| `ustekinumab` | `CHEMBL1201835` | 2 | il12_axis, il23_axis |
| `brodalumab` | `CHEMBL1742996` | 1 | il17_axis |
| `secukinumab` | `CHEMBL1743068` | 1 | il17_axis |
| `risankizumab` | `CHEMBL3990029` | 1 | il23_axis |
| `adalimumab` | `CHEMBL1201580` | 1 | tnf_axis |
| `methotrexate` | `CHEMBL2074969` | 0 | none |

## Open Targets Top Rows

| Mode | Top targets |
| --- | --- |
| `direct` | IL12B, TYK2, IL23A, TRAF3IP2, IL17RA, PDE4A, TNF, IL17A, AHR, VDR |
| `indirect_enabled` | CARD14, IL36RN, IL12B, TYK2, IL17RA, IL23A, TRAF3IP2, AP1S3, PDE4A, AHR |

## Cross-Source Prior Axes

| Axis | ChEMBL mechanism hits | Open Targets top hits | Status |
| --- | ---: | ---: | --- |
| `il12_axis` | 1 | 4 | `shared_prior_axis` |
| `il17_axis` | 2 | 6 | `shared_prior_axis` |
| `il23_axis` | 2 | 2 | `shared_prior_axis` |
| `il36_axis` | 0 | 1 | `single_source_prior_axis` |
| `tnf_axis` | 1 | 2 | `shared_prior_axis` |
| `tyk2_axis` | 0 | 2 | `single_source_prior_axis` |

## PRIDE Proteomics

| Project | Files | Raw files | Listed bytes | Next classes |
| --- | ---: | ---: | ---: | --- |
| `PXD021673` | 16 | 15 | 14300740896 | `{'proteomics_derived_file_next_candidate': 1, 'raw_ms_payload_blocked': 15}` |
| `PXD063539` | 15 | 5 | 785952364554 | `{'proteomics_derived_file_next_candidate': 10, 'raw_ms_payload_blocked': 5}` |
| `PXD035174` | 11 | 10 | 9963921987 | `{'proteomics_derived_file_next_candidate': 1, 'raw_ms_payload_blocked': 10}` |
| `PXD001387` | 72 | 48 | 38462722825 | `{'proteomics_derived_file_next_candidate': 24, 'raw_ms_payload_blocked': 48}` |
| `PXD077433` | 17 | 15 | 28045324274 | `{'proteomics_derived_file_next_candidate': 2, 'raw_ms_payload_blocked': 15}` |
| `PXD063928` | 17 | 15 | 5765410238 | `{'proteomics_derived_file_next_candidate': 2, 'raw_ms_payload_blocked': 15}` |

## Proteomics Admission Classes

| Class | Files | Bytes |
| --- | ---: | ---: |
| `proteomics_derived_file_next_candidate` | 40 | 12051036780 |
| `raw_ms_payload_blocked` | 108 | 870439447994 |

## Not Yet Discovered

- No target, drug, pathway, protein marker, responder, or repressor has been validated by module execution.
- No PRIDE raw mass-spectrometry file has been mirrored or quantified.
- No ChEMBL or Open Targets prior has been converted into a claim certificate.

## Next Required

- Admit proteomics derived result/search/peak files before raw mass-spectrometry mirroring.
- Map ChEMBL mechanism target identifiers to Ensembl/HGNC in a versioned bridge before target modules consume them.
- Join Open Targets target rows to R-band, Anduril, and ArtMethods module input queues as priors only.
- Require source-specific claim certificates before any drug, target, or protein is called a discovery.
