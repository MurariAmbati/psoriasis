# Real-Data Psoriasis Target Feature-Universe Binding Receipt

Feature-universe binding for psoriasis ChEMBL target components. This proves feature presence in real matrices only; it does not execute biology or promote target claims.

- Target-component bindings: 7
- Unique target symbols: 6
- Component feature hits: 28
- Unique-symbol feature hits: 18
- Feature universes with target hits: 3
- Accessions with target hits: 3
- Direct symbol hits: 28
- Direct Ensembl hits: 0
- Biological discovery claims promoted: 0
- Binding digest: `683acbe88aabb158bb1e4c28dbe7b8b1f1eb0e29ec5b905d8e1712ca17c892b8`

## Discoveries So Far

- All six psoriasis drug-target component gene symbols from the ChEMBL/Open Targets bridge are present in real processed psoriasis matrix feature universes.
- The current executable feature binding is symbol-level: the real feature universes contain TNF, IL12B, IL12A, IL23A, IL17A, and IL17RA as feature IDs, but not their Ensembl gene IDs.
- Three processed psoriasis matrix assets currently provide direct target-gene feature coverage for IL-12, IL-23, IL-17, and TNF axes before any scientific executor is released.
- Protein-complex targets remain component-level bindings, so IL-12 and IL-23 do not collapse into a single target feature.

## Component Bindings

| Target | Symbol | Ensembl IDs | Hits | Universes | Axes | Status |
| --- | --- | --- | ---: | ---: | --- | --- |
| `CHEMBL1825` | `TNF` | `ENSG00000232810` | 10 | 3 | `tnf_axis` | `component_symbol_bound_to_real_feature_universes` |
| `CHEMBL2364153` | `IL12B` | `ENSG00000113302` | 3 | 3 | `il12_axis` | `component_symbol_bound_to_real_feature_universes` |
| `CHEMBL2364153` | `IL12A` | `ENSG00000168811` | 3 | 3 | `il12_axis` | `component_symbol_bound_to_real_feature_universes` |
| `CHEMBL2364154` | `IL12B` | `ENSG00000113302` | 3 | 3 | `il23_axis` | `component_symbol_bound_to_real_feature_universes` |
| `CHEMBL2364154` | `IL23A` | `ENSG00000110944` | 3 | 3 | `il23_axis` | `component_symbol_bound_to_real_feature_universes` |
| `CHEMBL3390822` | `IL17A` | `ENSG00000112115` | 3 | 3 | `il17_axis` | `component_symbol_bound_to_real_feature_universes` |
| `CHEMBL3580485` | `IL17RA` | `ENSG00000177663` | 3 | 3 | `il17_axis` | `component_symbol_bound_to_real_feature_universes` |

## Unique Symbol Coverage

| Symbol | Targets | Hits | Accessions | Universes |
| --- | --- | ---: | ---: | ---: |
| `IL12A` | `CHEMBL2364153` | 3 | 3 | 3 |
| `IL12B` | `CHEMBL2364153, CHEMBL2364154` | 3 | 3 | 3 |
| `IL17A` | `CHEMBL3390822` | 3 | 3 | 3 |
| `IL17RA` | `CHEMBL3580485` | 3 | 3 | 3 |
| `IL23A` | `CHEMBL2364154` | 3 | 3 | 3 |
| `TNF` | `CHEMBL1825` | 3 | 3 | 3 |

## Hit Matrices

| Symbol | Accession | Matrix | Namespace | Feature index |
| --- | --- | --- | --- | ---: |
| `IL12A` | `GSE121212` | `GSE121212_readcount.txt.gz` | `gene_symbol_or_processed_feature` | 11317 |
| `IL12A` | `GSE54456` | `GSE54456_RPKM_samples.txt.gz` | `gene_symbol_or_processed_feature` | 8482 |
| `IL12A` | `GSE66511` | `GSE66511_Psoriasis_counts.txt.gz` | `gene_symbol` | 9427 |
| `IL12B` | `GSE121212` | `GSE121212_readcount.txt.gz` | `gene_symbol_or_processed_feature` | 11319 |
| `IL12B` | `GSE54456` | `GSE54456_RPKM_samples.txt.gz` | `gene_symbol_or_processed_feature` | 8483 |
| `IL12B` | `GSE66511` | `GSE66511_Psoriasis_counts.txt.gz` | `gene_symbol` | 9428 |
| `IL17A` | `GSE121212` | `GSE121212_readcount.txt.gz` | `gene_symbol_or_processed_feature` | 11328 |
| `IL17A` | `GSE54456` | `GSE54456_RPKM_samples.txt.gz` | `gene_symbol_or_processed_feature` | 8492 |
| `IL17A` | `GSE66511` | `GSE66511_Psoriasis_counts.txt.gz` | `gene_symbol` | 9437 |
| `IL17RA` | `GSE121212` | `GSE121212_readcount.txt.gz` | `gene_symbol_or_processed_feature` | 11333 |
| `IL17RA` | `GSE54456` | `GSE54456_RPKM_samples.txt.gz` | `gene_symbol_or_processed_feature` | 8497 |
| `IL17RA` | `GSE66511` | `GSE66511_Psoriasis_counts.txt.gz` | `gene_symbol` | 9442 |
| `IL23A` | `GSE121212` | `GSE121212_readcount.txt.gz` | `gene_symbol_or_processed_feature` | 11363 |
| `IL23A` | `GSE54456` | `GSE54456_RPKM_samples.txt.gz` | `gene_symbol_or_processed_feature` | 8516 |
| `IL23A` | `GSE66511` | `GSE66511_Psoriasis_counts.txt.gz` | `gene_symbol` | 9478 |
| `TNF` | `GSE121212` | `GSE121212_readcount.txt.gz` | `gene_symbol_or_processed_feature` | 28460 |
| `TNF` | `GSE54456` | `GSE54456_RPKM_samples.txt.gz` | `gene_symbol_or_processed_feature` | 19349 |
| `TNF` | `GSE66511` | `GSE66511_Psoriasis_counts.txt.gz` | `gene_symbol` | 21954 |

## Not Yet Discovered

- No target feature has been tested for differential expression, causality, repression, response, or therapeutic validity.
- No Affymetrix/GEO probe feature has been remapped to these target genes in this receipt.
- No proteomics abundance file has been joined to these target components.
- No module has consumed these feature bindings in a released scientific execution.

## Release Boundary

- add probe-to-gene annotation receipts for GEO ID_REF feature universes
- bind target-feature hits into module input contracts as priors only
- require normalization, missingness, falsifier, and claim-certificate receipts before target-feature results can be promoted
- join admitted proteomics abundance features to target components after proteomics derived-file admission
