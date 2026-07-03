# Real-Data Psoriasis Open-Source Discovery Receipt

Live metadata search/download receipt for psoriasis open-source modalities. Raw payloads, scientific execution, matrix materialization, and result claims remain blocked.

- Run id: `rdq-20260627-psoriasis-open-source-discovery`
- Metadata records: 49
- Metadata payload bytes: 1178755
- PRIDE unique project candidates: 31
- PRIDE new candidates beyond current manifest: 25
- GEO broad psoriasis reported records: 621
- GEO treatment/drug/therapy reported records: 436
- GEO single-cell reported records: 99
- GEO spatial/transcriptomics reported records: 94
- GEO indexed accessions: 10
- GEO indexed download candidates: 32
- ChEMBL indication row instances: 520
- ChEMBL unique molecules: 216
- Open Targets direct associated targets: 6963
- Open Targets indirect-enabled associated targets: 7146
- Biological result claims promoted: 0
- Receipt digest: `b86afecdc9ce2a7f8b3451b42c72dc4b6591cd262a73210c0582fe1ba424888b`

## Discoveries So Far

- PRIDE keyword searches discovered 31 unique psoriasis/psoriatic proteomics project candidates; 25 are not yet represented in the current modality candidate manifest.
- GEO E-utilities reported 621 psoriasis GSE records, including 436 treatment/drug/therapy records, 99 single-cell records, and 94 spatial/transcriptomics records.
- The receipt indexed exact FTP directories for 10 top GEO candidates and found 32 small/metadata download candidates while keeping 9 raw or bulk payloads blocked.
- ChEMBL psoriasis indication slices downloaded 520 row instances across mesh/EFO terms, covering 216 unique molecule IDs for drug-prior routing.
- Open Targets metadata returned 6963 direct and 7146 indirect-enabled psoriasis associated-target counts.
- These are source and admission discoveries only; they are not validated disease mechanisms, drug-response findings, biomarkers, repressors, targets, or treatment claims.

## PRIDE Search

| Keyword | Returned projects |
| --- | ---: |
| `psoriasis` | 26 |
| `psoriatic` | 14 |
| `psoriasis vulgaris` | 2 |

## New PRIDE Candidates

| Accession | Keywords | Organisms | Title |
| --- | --- | --- | --- |
| `PAD000024` | psoriasis | Homo sapiens (human) | Major depressive disorder shares systemic immune signatures and potential therapeutic targets with inflammatory skin diseases |
| `PXD000707` | psoriatic | Homo sapiens (human) | Discovery and Confirmation of a Protein Biomarker Panel with Potential to Predict Response to Biologic Therapy in Psoriatic Arthritis |
| `PXD010852` | psoriatic | Homo sapiens (human) | Connective tissue regeneration dynamics persistently alter epithelial dynein DNAH10 expression - DNAH10 overexpression in psoriatic lesional epidermis |
| `PXD011872` | psoriatic | Homo sapiens (human) | Human Arthritic Synovial Fluid LC-MS/MS |
| `PXD022442` | psoriatic | Homo sapiens (human) | Proteinases in psoriatic arthritis |
| `PXD023779` | psoriasis | Mus musculus (mouse) | CCDC88B affinity proteomic analysis |
| `PXD027364` | psoriasis | Homo sapiens (human) | Thrombospondin-4 is a soluble dermal signal that selectively promotes fibroblast migration and keratinocyte proliferation for skin regeneration and wound healing |
| `PXD029030` | psoriasis, psoriatic | Homo sapiens (human) | Hsa-miR-31-5p controls a metabolic switch in psoriatic keratinocytes that identifies therapeutic intervention |
| `PXD029881` | psoriasis | Homo sapiens (human) | Olfactomedin-4 improves cutaneous wound healing by promoting skin cell proliferation and migration |
| `PXD031064` | psoriasis | Homo sapiens (human) | Human LC-MS/MS for MBTPS1/S1P protein |
| `PXD033009` | psoriasis | Homo sapiens (human) | The CARD14E138A phosphoproteome |
| `PXD033039` | psoriasis | Homo sapiens (human) | The CARD14WT/E138A interactome. |
| `PXD036366` | psoriasis, psoriatic | Mus musculus (mouse) | CMTM4 is a subunit of the IL-17 receptor and mediates autoimmune pathology |
| `PXD037093` | psoriasis | Deinagkistrodon acutus | Isolation and Characterization of ZK002, A Novel Dual Function Snake Venom Peptide from Deinagkistrodon acutus with Anti-angiogenic and Anti-inflammatory Properties |
| `PXD037593` | psoriatic | Homo sapiens (human) | Proliferation, migration and inflammation-related signaling pathways activated in THBS4-stimulated keratinocytes characterize both wound healing and atopic dermatitis |

## GEO Search

| Query | Reported records | Returned summaries |
| --- | ---: | ---: |
| `broad` | 621 | 25 |
| `treatment_drug_therapy` | 436 | 25 |
| `single_cell` | 99 | 25 |
| `spatial_transcriptomics` | 94 | 25 |
| `proteomics` | 4 | 4 |

## New GEO Candidates

| Accession | Labels | Samples | Taxon | Title |
| --- | --- | ---: | --- | --- |
| `GSE299050` | broad, single_cell, spatial_transcriptomics, treatment_drug_therapy | 5 | Homo sapiens | Immune Dynamics in Palmoplantar Pustulosis Unveiled by Single-Cell and High-Resolution Spatial Transcriptomics [scRNA-seq] |
| `GSE299051` | broad, single_cell, spatial_transcriptomics, treatment_drug_therapy | 2 | Homo sapiens | Immune Dynamics in Palmoplantar Pustulosis Unveiled by Single-Cell and High-Resolution Spatial Transcriptomics [Spatial Transcriptomics] |
| `GSE328285` | broad, single_cell, spatial_transcriptomics, treatment_drug_therapy | 10 | Homo sapiens | Inhibition of Salt-Inducible Kinases 2 and 3 reduces inflammatory signature in Psoriasis |
| `GSE331382` | broad, single_cell, spatial_transcriptomics, treatment_drug_therapy | 60 | Homo sapiens | Inhibition of Salt-Inducible Kinases 2 and 3 reduces inflammatory signature in Psoriasis |
| `GSE263148` | broad, spatial_transcriptomics, treatment_drug_therapy | 2 | Mus musculus | RNA-seq of ear skins from KAT8 cKO and WT mice in IMQ-induced psoriatic model |
| `GSE287897` | broad, single_cell, treatment_drug_therapy | 9 | Mus musculus | SPT6 maintains epidermal homeostasis by inhibiting an NF-kB- positive feedback loop to prevent excessive inflammation |
| `GSE294009` | single_cell, spatial_transcriptomics, treatment_drug_therapy | 204 | Homo sapiens | Spatial Transcriptomic Analysis of Early and Late Stages of Hidradenitis Suppurativa |
| `GSE294435` | broad, single_cell, treatment_drug_therapy | 2 | Mus musculus | Transcription Elongation Factor SPT6 Maintains Epidermal Homeostasis and Suppresses Skin Inflammation in Mice |
| `GSE301804` | broad, single_cell, spatial_transcriptomics | 19 | Homo sapiens | Rare ADAR1 loss-of-function variants alter RNA editing and drive interferon-dependent inflammation in psoriasis |
| `GSE310145` | broad, spatial_transcriptomics, treatment_drug_therapy | 103 | Homo sapiens | Spatial transcriptomic profiling reveals body site-specific inflammatory differences in psoriasis lesions |
| `GSE314158` | broad, single_cell, spatial_transcriptomics | 134 | Homo sapiens | 6K-plex RNA CosMx data fra human FFPE samples from patients with psoriasis. |
| `GSE318600` | broad, single_cell, treatment_drug_therapy | 4 | Mus musculus | Psoriasis-like disease prevents squamous skin tumor development by neutrophil-driven inflammation |
| `GSE324735` | broad, single_cell, treatment_drug_therapy | 6 | Mus musculus | PEPITEM regulates the synovial microenvironment during immune-mediated inflammatory arthritis to limit disease |
| `GSE279719` | broad, treatment_drug_therapy | 72 | Homo sapiens | Human CD14+ monocytes from early inflammatory arthritis patients before and after a 5day-and 30day-period of methotrexate treatment |
| `GSE295541` | broad, treatment_drug_therapy | 12 | Mus musculus | TCN2 promotes psoriatic skin inflammation and keratinocyte proliferation via the IL-1beta-STAT3 pathway |

## GEO File Index Gate

| Accession | Files | Download candidates | Bulk blocked | Candidate bytes | Blocked bytes |
| --- | ---: | ---: | ---: | ---: | ---: |
| `GSE299050` | 4 | 3 | 1 | 8126 | 71065600 |
| `GSE299051` | 5 | 3 | 2 | 7347 | 2146030571 |
| `GSE328285` | 4 | 4 | 0 | 1137787 | 0 |
| `GSE331382` | 4 | 4 | 0 | 19887986 | 0 |
| `GSE263148` | 3 | 3 | 0 | 176919 | 0 |
| `GSE287897` | 3 | 3 | 0 | 567917 | 0 |
| `GSE294009` | 5 | 3 | 2 | 43270 | 13535597 |
| `GSE294435` | 4 | 3 | 1 | 7248 | 210585600 |
| `GSE301804` | 4 | 3 | 1 | 11358 | 761395200 |
| `GSE310145` | 5 | 3 | 2 | 24140 | 8763948 |

## ChEMBL And Open Targets

| Source slice | Rows | Unique molecules |
| --- | ---: | ---: |
| `mesh_psoriasis` | 260 | 216 |
| `efo_psoriasis` | 200 | 200 |
| `efo_psoriasis_vulgaris` | 52 | 52 |
| `efo_pustulosis_palmaris_et_plantaris` | 8 | 8 |

| Open Targets mode | Associated target count | Top rows |
| --- | ---: | ---: |
| `direct` | 6963 | 50 |
| `indirect_enabled` | 7146 | 50 |

## Release Boundary

- promote selected new PRIDE projects into exact project/file admission receipts before downloading derived or raw payloads
- promote selected new GEO series into exact file manifests and small-file ledgers before matrix adapters consume them
- resolve ChEMBL molecules and Open Targets genes into versioned target/drug identifier bridges before module use
- only run Anduril, ArtMethods, R-band, or KnownMethods modules after source-specific matrices pass checksum, sample, missingness, normalization, and abstention gates

## Still Blocked

- raw mass spectrometry payload downloads
- GEO RAW archives and oversized matrices
- clinical, treatment, target, drug, biomarker, severity, responder, or cure claims
- scientific execution against newly discovered sources
