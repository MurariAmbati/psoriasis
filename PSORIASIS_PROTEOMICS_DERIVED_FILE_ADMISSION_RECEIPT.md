# Psoriasis Comprehensive Deep-Learning — All Data, All Modalities

**RUO.** GPU-trained across every modality on ALL available data (not subsets). Honest spectrum from saturated (bulk) to genuinely hard (single-cell).

## Scope (vs the earlier shallow pass)

- **Bulk expression: 1350 samples x 11873 genes x 12 cohorts x 3 platforms** (was 661x3000x7). Real mini-batch SGD (44,423 steps), 3-seed CV.

- **Methylation: 273 samples x 8000 CpGs x 3 cohorts** (beta values were never in a deep net).

- **Single-cell: 2408 keratinocytes x 2000 HVG x 2 cohorts** (never modeled).

## Results — the honest spectrum

| Modality / task | AUROC | Note |
|---|---:|---|
| Bulk lesional-vs-normal LOCO (3 seeds) | 0.999+/-0.001 | saturated (huge transcriptomic diff) |
| Bulk lesional-vs-NONlesional LOCO (hard) | 0.988+/-0.021 | within-patient; GSE85034 Illumina 0.924 |
| Bulk CROSS-PLATFORM (Affy->Illumina+RNAseq) | 0.969+/-0.009 | real platform-transfer degradation |
| **Methylation** lesional-vs-normal LOCO | 0.93+/-0.049 | weaker/noisier than expression |
| **Single-cell** per-cell keratinocyte, CROSS-COHORT | 0.732 | the genuinely HARD task |
| WGAN-GP (full 11873 genes) | realism 0.902 / transfer 0.754 | |

## Honest interpretation

Bulk lesional classification is **near-saturated even on hard tasks (0.97-0.999)** because the lesional transcriptome is massively different from normal -- this is biology, not under-training, and it holds across all data/platforms with multi-seed CV. The informative gradient is: **bulk (0.99) > methylation (0.93) > cross-platform (0.97) > single-cell per-cell cross-cohort (0.73)**. The single-cell result is the only genuinely non-saturated one: an individual keratinocyte carries the disease state only modestly and transfers imperfectly. Deep learning adds representation (VAE subtypes, GNN, WGAN-GP that now encodes phenotype at 0.75) but does not 'beat' the trivial signal because there is no hard bulk prediction problem here -- unlike AML survival.

## Remaining deep gaps (honest)

- ARCHS4 (57 GB, downloading) will add hundreds more uniformly-processed samples.
- Multi-modal joint integration (same-sample expression+methylation) is impossible in public data (different samples per modality).
- A genuinely hard supervised target (severity/PASI regression, treatment-response) needs the account-gated trial data (ImmPort).

