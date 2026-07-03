# Real-Data Psoriasis Proteomics Missingness Filter Receipt

Missingness filter candidate receipt for real grouped PXD063539 proteomics contrast targets. This does not materialize filtered matrices, normalize values, execute modules, or promote biological claims.

- Missingness filter receipts: 12
- Thresholds tested: 5
- Primary min observed per group: 4
- Primary candidate feature rows: 34819
- Biological discovery claims promoted: 0
- Receipt digest: `aeae6e8c24f4644db47462f3120b1a949d3b9dad05f04218837f10cf314982f5`

## Threshold Totals

| Min observed per group | Passing both groups | Passing either group |
| ---: | ---: | ---: |
| 1 | 54143 | 62387 |
| 2 | 45453 | 58713 |
| 4 | 34819 | 50075 |
| 6 | 26265 | 40279 |
| 8 | 16399 | 27475 |

## Discoveries So Far

- A primary grouped proteomics missingness candidate gate requiring at least four observed samples in each compared group retains 34,819 contrast feature rows across the 12 layer contrasts.
- A strict complete-case gate requiring all eight samples in each compared group retains 16,399 contrast feature rows, showing that complete-case execution would discard substantial real proteomics coverage.
- A permissive one-sample-per-group gate matches the contrast-readiness detected-both count of 54,143 feature rows.
- Missingness filtering can now be audited per layer and per grouped condition contrast before normalization is attempted.

## Contrast Filters

| Contrast | Features | Min1 | Min2 | Min4 | Min6 | Min8 |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| `dermis:lesional_vs_nonlesional` | 5247 | 4995 | 4476 | 3585 | 2747 | 1655 |
| `dermis:lesional_vs_healthy` | 5247 | 4279 | 3597 | 2730 | 2071 | 1186 |
| `dermis:nonlesional_vs_healthy` | 5247 | 4260 | 3551 | 2711 | 2061 | 1213 |
| `inner_epidermis:lesional_vs_nonlesional` | 6380 | 5987 | 5565 | 4906 | 4219 | 3280 |
| `inner_epidermis:lesional_vs_healthy` | 6380 | 5662 | 5102 | 4224 | 3517 | 2554 |
| `inner_epidermis:nonlesional_vs_healthy` | 6380 | 5597 | 5067 | 4237 | 3533 | 2571 |
| `outer_epidermis:lesional_vs_nonlesional` | 4749 | 4098 | 3542 | 2556 | 1616 | 448 |
| `outer_epidermis:lesional_vs_healthy` | 4749 | 3284 | 1797 | 1023 | 650 | 371 |
| `outer_epidermis:nonlesional_vs_healthy` | 4749 | 3161 | 1787 | 1022 | 655 | 342 |
| `subcutis:lesional_vs_nonlesional` | 4803 | 4453 | 3873 | 2852 | 1987 | 1055 |
| `subcutis:lesional_vs_healthy` | 4803 | 4186 | 3541 | 2464 | 1603 | 880 |
| `subcutis:nonlesional_vs_healthy` | 4803 | 4181 | 3555 | 2509 | 1606 | 844 |

## Not Yet Discovered

- No filtered proteomics matrix has been materialized.
- No normalization, imputation, statistical contrast, or module execution has been released.
- No paired design has been proven from deidentified sample names.
- No protein marker, target, pathway, drug-response, or repression claim has been promoted.

## Release Boundary

- write normalization method receipts for the selected missingness threshold
- materialize filtered matrices only after normalization and matrix-output gates pass
- prove or reject sample pairing before paired proteomics tests are allowed
- bind filtered proteomics contrast targets into module contracts only as executor-blocked inputs
