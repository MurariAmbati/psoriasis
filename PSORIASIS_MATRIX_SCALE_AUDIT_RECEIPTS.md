# Real-Data Psoriasis Proteomics Contrast Readiness Receipt

Grouped contrast-readiness receipt for admitted human PXD063539 proteomics layer matrices. This records real sample groups and missingness only; no normalization, statistical testing, executor release, or claim promotion is allowed.

- Matrix readiness receipts: 4
- Contrast readiness targets: 12
- Condition groups: 12
- Total feature rows across matrices: 21179
- Total contrast feature rows: 63537
- Features detected in both compared groups: 54143
- Features complete in both compared groups: 16399
- Paired design allowed: false
- Biological discovery claims promoted: 0
- Receipt digest: `f491220cb21e46d6b788e929b6c04d01a6d45866e682c7fa7977119d893f25fe`

## Discoveries So Far

- PXD063539 provides four human spatial-layer proteomics abundance matrices with balanced grouped condition coverage: 8 lesional, 8 nonlesional, and 8 healthy sample/run columns per layer.
- Twelve grouped proteomics contrast targets are now auditable across lesional-vs-nonlesional, lesional-vs-healthy, and nonlesional-vs-healthy comparisons for each layer.
- Across all proteomics contrast targets, 54,143 feature rows have at least one observed abundance value in both compared groups before any normalization or differential testing.
- Only 16,399 contrast feature rows are complete across all compared samples, so missingness-aware normalization and filtering are mandatory before execution.
- No admitted proteomics matrix contains direct IL/TNF target-symbol hits, so target-linked proteomics claims remain blocked.

## Matrix Readiness

| Layer | Features | Samples | Lesional | Nonlesional | Healthy | Target hits |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| `dermis` | 5247 | 24 | 8 | 8 | 8 | 0 |
| `inner_epidermis` | 6380 | 24 | 8 | 8 | 8 | 0 |
| `outer_epidermis` | 4749 | 24 | 8 | 8 | 8 | 0 |
| `subcutis` | 4803 | 24 | 8 | 8 | 8 | 0 |

## Contrast Targets

| Contrast | Features | Detected both | Complete both | Left only | Right only |
| --- | ---: | ---: | ---: | ---: | ---: |
| `dermis:lesional_vs_nonlesional` | 5247 | 4995 | 1655 | 183 | 54 |
| `dermis:lesional_vs_healthy` | 5247 | 4279 | 1186 | 899 | 42 |
| `dermis:nonlesional_vs_healthy` | 5247 | 4260 | 1213 | 789 | 61 |
| `inner_epidermis:lesional_vs_nonlesional` | 6380 | 5987 | 3280 | 324 | 52 |
| `inner_epidermis:lesional_vs_healthy` | 6380 | 5662 | 2554 | 649 | 50 |
| `inner_epidermis:nonlesional_vs_healthy` | 6380 | 5597 | 2571 | 442 | 115 |
| `outer_epidermis:lesional_vs_nonlesional` | 4749 | 4098 | 448 | 622 | 20 |
| `outer_epidermis:lesional_vs_healthy` | 4749 | 3284 | 371 | 1436 | 19 |
| `outer_epidermis:nonlesional_vs_healthy` | 4749 | 3161 | 342 | 957 | 142 |
| `subcutis:lesional_vs_nonlesional` | 4803 | 4453 | 1055 | 154 | 142 |
| `subcutis:lesional_vs_healthy` | 4803 | 4186 | 880 | 421 | 126 |
| `subcutis:nonlesional_vs_healthy` | 4803 | 4181 | 844 | 414 | 131 |

## Not Yet Discovered

- No paired sample design has been proven from the deidentified matrix column names.
- No proteomics matrix has been normalized, filtered, contrasted, or tested.
- No proteomics contrast has been released to Anduril, ArtMethods, R-band, or KnownMethods executors.
- No protein marker, pathway, target, drug-response, or repression claim has been promoted.

## Release Boundary

- write proteomics missingness filter receipts for each layer and contrast
- write normalization method receipts for DIA-NN protein-group abundance values
- prove or reject sample pairing before paired tests are allowed
- bind accepted proteomics contrast targets into module input contracts after normalization gates pass
