# Real-Data Psoriasis Target Identifier Bridge Receipt

Identifier bridge from ChEMBL named-drug mechanism targets to ChEMBL target components, HGNC symbols, UniProt accessions, and Open Targets Ensembl rows. This does not execute modules or promote target claims.

- Mechanism rows: 6
- Unique ChEMBL targets: 5
- Target component rows: 7
- Unique component gene symbols: 6
- Component rows matched to Open Targets: 7
- Unique matched Ensembl IDs: 6
- Axes with ChEMBL targets: il12_axis, il17_axis, il23_axis, tnf_axis
- Biological discovery claims promoted: 0
- Bridge digest: `0140dcf2133ca3468b9c075ebdee63fca459036bd802987edd5dbd673d484707`

## Identifier Bridge Discoveries

- ChEMBL mechanism target IDs for psoriasis named drugs now resolve to real ChEMBL target records.
- IL-12 and IL-23 are represented as protein complexes and are bridged to component-level gene symbols rather than flattened to a single target.
- ChEMBL component gene symbols bridge to Open Targets Ensembl rows for IL12B, IL12A, IL23A, IL17RA, IL17A, and TNF.

## ChEMBL Targets

| ChEMBL target | Name | Type | Components | Ensembl IDs |
| --- | --- | --- | --- | --- |
| `CHEMBL1825` | Tumor necrosis factor | `SINGLE PROTEIN` | TNF | ENSG00000232810 |
| `CHEMBL2364153` | Interleukin-12 | `PROTEIN COMPLEX` | IL12B, IL12A | ENSG00000113302, ENSG00000168811 |
| `CHEMBL2364154` | Interleukin-23 | `PROTEIN COMPLEX` | IL12B, IL23A | ENSG00000110944, ENSG00000113302 |
| `CHEMBL3390822` | Interleukin-17A | `SINGLE PROTEIN` | IL17A | ENSG00000112115 |
| `CHEMBL3580485` | Interleukin-17 receptor A | `SINGLE PROTEIN` | IL17RA | ENSG00000177663 |

## Mechanism Bridges

| Drug query | Mechanism | ChEMBL target | Components | Ensembl IDs |
| --- | --- | --- | --- | --- |
| `ustekinumab` | Interleukin-12 inhibitor | `CHEMBL2364153` | IL12B, IL12A | ENSG00000113302, ENSG00000168811 |
| `ustekinumab` | Interleukin-23 inhibitor | `CHEMBL2364154` | IL12B, IL23A | ENSG00000110944, ENSG00000113302 |
| `brodalumab` | Interleukin-17 receptor A antagonist | `CHEMBL3580485` | IL17RA | ENSG00000177663 |
| `secukinumab` | Interleukin 17A inhibitor | `CHEMBL3390822` | IL17A | ENSG00000112115 |
| `risankizumab` | Interleukin-23 inhibitor | `CHEMBL2364154` | IL12B, IL23A | ENSG00000110944, ENSG00000113302 |
| `adalimumab` | TNF-alpha inhibitor | `CHEMBL1825` | TNF | ENSG00000232810 |

## Component Bridges

| Gene | UniProt | ChEMBL target | Open Targets matches | Ensembl IDs |
| --- | --- | --- | ---: | --- |
| `TNF` | `P01375` | `CHEMBL1825` | 2 | ENSG00000232810 |
| `IL12B` | `P29460` | `CHEMBL2364153` | 2 | ENSG00000113302 |
| `IL12A` | `P29459` | `CHEMBL2364153` | 2 | ENSG00000168811 |
| `IL12B` | `P29460` | `CHEMBL2364154` | 2 | ENSG00000113302 |
| `IL23A` | `Q9NPF7` | `CHEMBL2364154` | 2 | ENSG00000110944 |
| `IL17A` | `Q16552` | `CHEMBL3390822` | 2 | ENSG00000112115 |
| `IL17RA` | `Q96F46` | `CHEMBL3580485` | 2 | ENSG00000177663 |

## Not Yet Discovered

- No target has been validated as causal, therapeutic, diagnostic, or repressive.
- No module has consumed these identifier bridges in scientific execution.
- No feature matrix has been materialized from these target identifiers.
