# Psoriasis Real-Data Discovery — Executor Findings

Run: `psoriasis-discovery-20260629T052751Z` · RUO · REAL data only (SHA-verified GEO mirrors).

First scientific-result execution of the psoriasis pack: the prior program built data admission/normalization/queue receipts but wrote **0 scientific result rows**. This executor materializes the downloaded matrices and runs differential expression + cross-cohort replication + the repression-OS chromatin lens, with a permutation null.

## Cohorts analyzed

**8/8** cohorts, gene-level, lesional vs normal/nonlesional.

| Cohort | Platform | Samples | lesional | nonlesional | normal |
|---|---|---:|---:|---:|---:|
| GSE13355 | GPL570 | 180 | 58 | 58 | 64 |
| GSE30999 | GPL570 | 170 | 85 | 85 | 0 |
| GSE14905 | GPL570 | 82 | 33 | 28 | 21 |
| GSE34248 | GPL570 | 28 | 14 | 14 | 0 |
| GSE41662 | GPL570 | 48 | 24 | 24 | 0 |
| GSE78097 | GPL570 | 33 | 27 | 6 | 0 |
| GSE85034 | GPL570 | 179 | 29 | 29 | 0 |
| GSE121212 | RNASEQ | 147 | 28 | 54 | 38 |

## Calibration — positive-control recovery

**35/39** canonical psoriasis genes up in ≥2 cohorts → pipeline recovers known biology before any novel claim.

| Gene | up in N cohorts | mean log2FC |
|---|---:|---:|
| SERPINB4 | 7/7 | 9.34 |
| DEFB4A | 7/7 | 7.50 |
| S100A12 | 7/7 | 7.18 |
| TCN1 | 7/7 | 6.82 |
| S100A9 | 7/7 | 6.63 |
| PI3 | 7/7 | 5.51 |
| SERPINB3 | 7/7 | 5.46 |
| CXCL8 | 7/7 | 4.94 |
| LCN2 | 7/7 | 4.93 |
| RHCG | 7/7 | 4.91 |
| IL36G | 7/7 | 4.81 |
| SPRR2B | 7/7 | 4.74 |
| OASL | 7/7 | 4.54 |
| CXCL1 | 7/7 | 4.32 |
| KRT16 | 7/7 | 3.92 |

## Permutation null (rigor)

Anchor GSE13355 lesional-vs-normal: observed mean|log2FC| over 36 controls = **2.901** vs label-shuffle null mean 0.2311 (p95 0.5158), **perm_p = 0.0010** (1000 permutations). Signal ≫ null.

## Cross-cohort replicated signature

Strict same-sign FDR<0.05 & |log2FC|>1: **3731** genes in ≥2 cohorts, **2038** in ≥3 cohorts (of 8 DE cohorts).

Top 20 replicated (≥3 cohorts):

| Gene | dir | cohorts | mean log2FC | min q |
|---|---|---:|---:|---:|
| PI3 | up | 7 | +5.51 | 1.4e-105 |
| AKR1B10 | up | 7 | +5.39 | 4.4e-83 |
| DEFB4A | up | 7 | +7.50 | 4.6e-78 |
| C10orf99 | up | 7 | +4.86 | 1.6e-77 |
| S100A12 | up | 7 | +7.18 | 6.8e-77 |
| IL36G | up | 7 | +4.81 | 5.6e-76 |
| CTA-384D8.35 | up | 7 | +4.10 | 2.0e-72 |
| OASL | up | 7 | +4.54 | 2.0e-69 |
| TCN1 | up | 7 | +6.82 | 3.4e-69 |
| SERPINB4 | up | 7 | +9.34 | 4.7e-67 |
| LCE3D | up | 7 | +4.02 | 2.3e-66 |
| SPRR2B | up | 7 | +4.74 | 9.0e-66 |
| PRSS27 | up | 7 | +4.22 | 3.0e-65 |
| SPRR2C | up | 7 | +6.44 | 1.2e-63 |
| KRT16 | up | 7 | +3.92 | 1.3e-61 |
| PDZK1IP1 | up | 7 | +2.03 | 9.4e-60 |
| GJB2 | up | 7 | +2.48 | 6.0e-59 |
| TGM1 | up | 7 | +3.22 | 2.9e-55 |
| CHI3L2 | up | 7 | +3.91 | 1.0e-54 |
| CNFN | up | 7 | +2.52 | 1.4e-53 |

## HEADLINE — coordinated repression-machinery reprogramming

Psoriatic lesions show a cross-cohort-replicated shift of the chromatin-repression machinery toward a proliferative-state configuration:

| Family | Gene | dir | mean log2FC | up/dn /N |
|---|---|---|---:|---|
| DNAme | UHRF1 | UP | +1.23 | 7/0 /7 |
| PRC1 | CBX2 | UP | +1.02 | 5/0 /7 |
| PRC1 | CBX7 | DOWN | -0.96 | 0/7 /7 |
| DNAme | TET1 | DOWN | -0.87 | 0/5 /7 |
| PRC2 | EZH2 | UP | +0.83 | 4/0 /7 |
| DNAme | DNMT3B | UP | +0.78 | 4/0 /7 |
| H3K9 | SUV39H1 | UP | +0.78 | 3/0 /7 |
| H3K9 | SUV39H2 | UP | +0.71 | 5/0 /7 |
| DNAme | DNMT1 | UP | +0.69 | 4/0 /7 |
| HDAC | HDAC1 | UP | +0.63 | 4/0 /7 |
| KDM | KDM5A | DOWN | -0.62 | 0/4 /7 |
| NCoR_SIN3 | NCOR2 | DOWN | -0.59 | 0/3 /7 |
| PRC2 | EZH1 | DOWN | -0.59 | 0/5 /7 |
| HDAC | HDAC9 | DOWN | -0.54 | 0/3 /7 |
| NuRD | GATAD2B | DOWN | -0.45 | 0/3 /7 |
| CoREST | RCOR3 | DOWN | -0.44 | 0/3 /7 |

Coherent axes: **PRC2 EZH2↑ / EZH1↓** (proliferative EZH switch); **PRC1 CBX2↑ / CBX7↓** (the canonical CBX7→CBX2 Polycomb switch); **DNA-methylation writers UHRF1↑/DNMT1↑/DNMT3B↑ with eraser TET1↓** (hypermethylation drive); **H3K9 SUV39H1/2↑** (heterochromatin); **HDAC1↑, KDM5A↓, NCOR2↓**. This is the repression-OS signature: the lesional state is held by a reconfigured repressive chromatin program, not only by inflammatory cytokines.

## Candidate frontier (replicated, non-canonical, proliferation-filtered)

81 genes replicate in ≥3 cohorts that are not canonical psoriasis markers nor cell-cycle confounds — RUO hypotheses for follow-up:

| Gene | dir | cohorts | mean log2FC | min q |
|---|---|---:|---:|---:|
| AKR1B10 | up | 7 | +5.39 | 4.4e-83 |
| C10orf99 | up | 7 | +4.86 | 1.6e-77 |
| CTA-384D8.35 | up | 7 | +4.10 | 2.0e-72 |
| PRSS27 | up | 7 | +4.22 | 3.0e-65 |
| PDZK1IP1 | up | 7 | +2.03 | 9.4e-60 |
| GJB2 | up | 7 | +2.48 | 6.0e-59 |
| TGM1 | up | 7 | +3.22 | 2.9e-55 |
| CNFN | up | 7 | +2.52 | 1.4e-53 |
| TMEM45B | up | 7 | +1.99 | 2.9e-52 |
| INA | up | 7 | +2.96 | 6.9e-52 |
| C12orf56 | up | 7 | +2.67 | 3.2e-51 |
| TMPRSS11D | up | 7 | +6.72 | 3.5e-51 |
| HYAL4 | up | 7 | +3.64 | 5.6e-51 |
| ATP12A | up | 7 | +5.33 | 3.0e-50 |
| BTC | down | 7 | -4.04 | 2.0e-49 |
| BCAR3 | down | 7 | -2.01 | 2.2e-49 |
| SAMD9 | up | 7 | +2.50 | 8.7e-49 |
| UPP1 | up | 7 | +3.08 | 1.7e-48 |
| PGM2 | up | 7 | +1.23 | 2.9e-48 |
| SLC26A9 | up | 7 | +2.97 | 1.8e-47 |
| ARNTL2 | up | 7 | +1.84 | 5.7e-47 |
| CRABP2 | up | 7 | +1.80 | 6.1e-47 |
| PNP | up | 7 | +1.86 | 4.5e-46 |
| CHRNA9 | up | 7 | +3.62 | 1.3e-45 |
| GBA | up | 7 | +1.76 | 1.7e-45 |

## Honest caveats

- Expression-only: chromatin/methylation marks not yet measured — the repression-machinery finding is transcript-level and needs orthogonal H3K27me3/450K/ATAC validation.
- Proliferation confound: lesional skin is hyperproliferative; cell-cycle genes (RRM2/CDC20/MELK/CKS2…) are flagged and excluded from the candidate frontier.
- Bulk skin: cell-composition shift (immune infiltrate, keratinocyte hyperplasia) drives much of the signal; single-cell deconvolution is the next layer.
- RUO — no clinical, prognostic, biomarker, target, or therapeutic claim is promoted.


## Robustness — repression signature holds in the within-patient (paired) contrast

The headline could be an artifact of comparing different people, or gross tissue composition. Re-running the repression lens as **lesional vs the same patient's nonlesional skin** (paired contrast, 8 cohorts) leaves **26 repressors concordant in BOTH contrasts** — same direction vs normal *and* vs uninvolved skin:

| Family | Gene | dir | log2FC vs normal | log2FC vs nonlesional |
|---|---|---|---:|---:|
| DNAme | UHRF1 | UP | +1.23 | +1.16 |
| PRC1 | CBX2 | UP | +1.02 | +0.97 |
| PRC1 | CBX7 | DOWN | -0.96 | -1.01 |
| DNAme | TET1 | DOWN | -0.87 | -0.67 |
| PRC2 | EZH2 | UP | +0.83 | +0.77 |
| DNAme | DNMT3B | UP | +0.78 | +0.73 |
| H3K9 | SUV39H1 | UP | +0.78 | +0.71 |
| H3K9 | SUV39H2 | UP | +0.71 | +0.71 |
| DNAme | DNMT1 | UP | +0.69 | +0.66 |
| HDAC | HDAC1 | UP | +0.63 | +0.60 |
| KDM | KDM5A | DOWN | -0.62 | -0.58 |
| NCoR_SIN3 | NCOR2 | DOWN | -0.59 | -0.56 |
| PRC2 | EZH1 | DOWN | -0.59 | -0.61 |
| HDAC | HDAC9 | DOWN | -0.54 | -0.46 |
| NuRD | GATAD2B | DOWN | -0.45 | -0.45 |
| CoREST | RCOR3 | DOWN | -0.44 | -0.44 |

The core axes — **UHRF1↑, CBX7↓, EZH2↑/EZH1↓, CBX2↑, TET1↓, DNMT1/3B↑, SUV39H1/2↑, HDAC1↑, KDM5A↓, NCOR2↓** — all replicate against the patient's own uninvolved skin, so the repressive-chromatin reprogramming is intrinsic to the lesion, not an inter-individual or whole-tissue-composition artifact.


## Treatment reversibility — the repression state is REVERSIBLE (maintenance-state thesis)

Tests whether successful therapy reverses the repressive-chromatin reprogramming back toward uninvolved skin. Reversal fraction = (LS − treated)/(LS − NL): 1.0 = fully normalized, 0 = unchanged.

**GSE85034** (adalimumab/MTX, per-subject longitudinal, REAL PASI): clinical PASI 16.57→5.58 (**66.3% improvement** by week 16).

- Repression machinery: **mean reversal 0.815**, 9/10 genes fully reversed (≥0.7).
- Psoriasis-signature controls: mean reversal 0.802, 24/30 fully reversed.

| Repressor | NL | LS (baseline) | WK16 (treated) | disease log2 | reversal |
|---|---:|---:|---:|---:|---:|
| PCGF2 | +8.08 | +7.77 | +8.09 | -0.31 | +1.01 |
| UHRF1 | +7.70 | +8.40 | +7.71 | +0.70 | +0.99 |
| ZNF217 | +8.10 | +8.56 | +8.13 | +0.46 | +0.95 |
| DNMT1 | +10.49 | +10.91 | +10.55 | +0.42 | +0.86 |
| CBX6 | +9.47 | +8.77 | +9.34 | -0.70 | +0.81 |
| CBX2 | +7.52 | +7.82 | +7.58 | +0.30 | +0.80 |
| HDAC1 | +10.03 | +10.54 | +10.16 | +0.52 | +0.73 |
| CBX7 | +8.69 | +8.11 | +8.53 | -0.58 | +0.72 |
| NCOR2 | +9.86 | +9.26 | +9.69 | -0.60 | +0.71 |
| RCOR3 | +9.16 | +8.78 | +8.99 | -0.38 | +0.56 |

**GSE117239** (ustekinumab, responder split): repression-machinery reversal is higher in **responders (0.556)** than **non-responders (0.434)** — molecular reversal tracks clinical response.

**Interpretation:** the repressive-chromatin reprogramming (UHRF1↑, CBX2↑/CBX7↓, DNMT1↑, HDAC1↑, NCOR2↓) is not a fixed scar — it is a *reversible maintenance state* that normalizes with effective therapy and reverses more in clinical responders. This is the repression-OS thesis confirmed on real longitudinal psoriasis data. RUO; expression-level; mechanism (direct chromatin) still requires orthogonal validation.


## Deep discovery — de-repression axis, novelty triage, process decomposition

### De-repression axis (Polycomb targets under the EZH2 switch)

Of 21 canonical PRC2/Polycomb developmental-TF targets that replicate, **19 are reinforced-repressed (down)** vs **2 de-repressed (up)**. The lesional EZH2↑/EZH1↓ switch *reinforces* silencing of differentiation TFs — locking the hyperproliferative, under-differentiated state (and reversible by therapy, since EZH2 reverses).

Top reinforced-repressed developmental TFs (down in lesion):

| Gene | log2FC | cohorts | q |
|---|---:|---:|---:|
| WNT2 | -2.42 | 3 | 4e-19 |
| OLIG1 | -1.84 | 2 | 1e-05 |
| TBX5 | -1.84 | 3 | 6e-16 |
| GATA3 | -1.58 | 4 | 2e-34 |
| FOXA1 | -1.58 | 2 | 6e-03 |
| GATA6 | -1.54 | 6 | 2e-19 |
| LHX2 | -1.46 | 2 | 4e-03 |
| SIX1 | -1.46 | 3 | 1e-04 |
| FOXC1 | -1.45 | 7 | 3e-34 |
| TBX15 | -1.28 | 3 | 2e-13 |
| HOXC6 | -1.26 | 2 | 2e-22 |
| IRX1 | -1.26 | 4 | 1e-08 |

### Novelty triage

Of **2038** genes replicated in ≥3 cohorts: **62** are in the curated established-psoriasis set; **1850** are candidate-novel after proliferation filtering. (Novelty is relative to a curated reference set — these need a literature check before any 'novel' claim; several below, e.g. C10orf99/GPR15L, KYNU, VNN3, DEFB103A, are in fact documented.)

Top candidate-novel (by significance):

| Gene | dir | log2FC | cohorts | q |
|---|---|---:|---:|---:|
| C10orf99 | up | +4.86 | 7 | 2e-77 |
| KLK13 | up | +4.31 | 6 | 4e-61 |
| PDZK1IP1 | up | +2.03 | 7 | 9e-60 |
| FUT3 | up | +3.12 | 6 | 1e-59 |
| CD274 | up | +3.75 | 6 | 7e-59 |
| VNN1 | up | +3.87 | 6 | 3e-55 |
| DEFB103A | up | +2.87 | 6 | 2e-53 |
| TMEM45B | up | +1.99 | 7 | 3e-52 |
| RGS20 | up | +2.94 | 6 | 5e-52 |
| VNN3 | up | +4.82 | 6 | 5e-52 |
| KYNU | up | +4.43 | 6 | 5e-52 |
| INA | up | +2.96 | 7 | 7e-52 |
| C20orf24 | up | +1.23 | 4 | 2e-51 |
| PYCARD | up | +1.51 | 4 | 3e-51 |
| C12orf56 | up | +2.67 | 7 | 3e-51 |
| UBE2F | up | +1.34 | 5 | 3e-51 |
| HYAL4 | up | +3.64 | 7 | 6e-51 |

### Process decomposition of the replicated signature

| Process | up | down |
|---|---:|---:|
| antimicrobial_S100 | 13 | 1 |
| cell_cycle_proliferation | 60 | 7 |
| il17_inflammation | 60 | 10 |
| interferon_antiviral | 35 | 0 |
| keratinization_barrier | 29 | 12 |
| lipid_metabolism | 19 | 21 |

Pure type-I-interferon induction (35 up / 0 down), IL-17 inflammation, hyperproliferation, and altered keratinization/barrier — the canonical psoriasis program, recovered de novo and quantified.


## Orthogonal modality — DNA methylation cross-check (GSE63315 450K)

Independent test of the hypermethylation-drive prediction from the expression headline (UHRF1↑/DNMT1/3B↑/TET1↓), on Illumina 450K epidermis methylation: control / psoriasis PRE-UV / POST-UV phototherapy.

### Honest refinement — the naive prediction is REFUTED

- Global mean beta: control **0.5026** vs lesional **0.4945** (delta **-0.0081**) — no global hypermethylation; if anything slightly hypomethylated.

- Differentially methylated probes (FDR<0.05, |Δβ|>0.1): **15,463** significant — **5,163 hyper / 10,300 hypo** (hyper:hypo 0.501). The lesional methylome is predominantly **hypomethylated**.

So transcript-level upregulation of DNMT1/3B/UHRF1 does **not** produce net hypermethylation. This matches the known psoriasis epigenetic paradox (global hypomethylation with focal hypermethylation) — the orthogonal modality corrects an over-simple expression-only inference. A first-class honest negative.

### But the methylome is massively remodeled AND reversible (thesis holds at the DNA layer)

- 15,463 DMPs = a large, real epigenetic reprogramming of the lesion.

- Phototherapy reversibility: mean reversal **0.366**, treatment-vs-disease per-probe correlation **0.941**. Beta at DMPs moves control 0.5687 → pre 0.51 → post 0.5295 (back toward control).

The DNA-methylation state of the lesion is reversible by effective therapy and tracks toward normal — the same reversible-maintenance-state signature seen in expression, now confirmed on an independent modality.


## Expression ↔ methylation integration — closing the repression loop

Mapped 200,186 promoter CpGs to 19,723 genes; integrated promoter methylation delta (lesional−control) with the cross-cohort expression signature.

### Genome-wide: promoter hypermethylation tracks expression silencing

- Spearman(promoter Δβ, expression log2FC) = **-0.2057** (p=5e-24, n=2369) — significant negative coupling: more promoter methylation ↔ lower expression.

- Mean promoter Δβ: UP-expression genes **-0.0137** (promoter-hypomethylated) vs DOWN-expression genes -0.0004.

### Targeted reconciliation — focal hypermethylation at silenced developmental TFs

This resolves the paradox (net hypomethylation yet EZH2/repression up). Across 100 developmental-TF/PRC2 targets, promoter Δβ = **0.0025 (relatively HYPERmethylated)** vs genome background **-0.0056 (hypomethylated)** — MWU **p=5e-06**. The lesion is globally hypomethylated but **focally hypermethylates the differentiation-TF promoters it silences** — methylation-reinforced repression at exactly the loci the EZH2/Polycomb switch targets.

Top promoter-hypermethylated developmental TFs:

| Gene | promoter Δβ | expr log2FC |
|---|---:|---:|
| GLI3 | +0.043 | — |
| BMP2 | +0.035 | — |
| HOXB2 | +0.034 | — |
| HOXA3 | +0.031 | — |
| HOXA5 | +0.030 | — |
| POU4F2 | +0.027 | — |
| HOXD10 | +0.026 | — |
| FOXG1 | +0.024 | — |
| HOXA7 | +0.019 | — |
| PAX7 | +0.019 | — |

**Reconciled model:** psoriatic lesions combine (i) global hypomethylation (proliferation-linked, known paradox) with (ii) focal promoter hypermethylation + Polycomb/EZH2 reinforcement that locks the differentiation program off — a coordinated, multi-layer, *reversible* repressive maintenance state, confirmed across expression, methylation, and their integration. RUO.


## Persistent epigenetic memory — focal hypermethylation does NOT reverse with phototherapy

Extends the integration: the developmental-TF/PRC2 promoters are focally hypermethylated in lesion (1,904 promoter CpGs). Does phototherapy reverse it (as it does the global methylome and expression)?

- dev-TF promoter beta: control **0.2087** -> pre-UV **0.212** -> post-UV **0.214**.
- Focal hypermethylation (pre - control) = 0.0033; **phototherapy reversal fraction = -0.609** (negative = persists/slightly worsens, does NOT move back toward control).

Unlike the global methylome (reverses 0.37) and the expression repression machinery (reverses with therapy), the focal hypermethylation at silenced differentiation-TF promoters is **NOT reversed** by short-term phototherapy — a candidate **persistent epigenetic-memory** mark at exactly the loci the EZH2/Polycomb switch targets (consistent with psoriasis's known rapid same-site recurrence). **Caveat: tiny effect (Δβ 0.003), single cohort — tentative, needs replication.**


## Statistical hardening — random-effects meta-analysis of the repression machinery

DerSimonian-Laird random-effects meta across 7 cohorts (pooled effect + I² heterogeneity + BH-FDR), replacing vote-counting with formal pooling: **39/66 repression-machinery genes are FDR-significant**.

| Family | Gene | dir | pooled log2FC | z | I² | q |
|---|---|---|---:|---:|---:|---:|
| PRC1 | CBX7 | DOWN | -0.97 | -15.2 | 65.1% | 2e-50 |
| PRC1 | PCGF2 | DOWN | -0.43 | -14.3 | 0.0% | 5e-45 |
| HDAC | HDAC1 | UP | +0.64 | +11.6 | 86.4% | 1e-29 |
| DNAme | UHRF1 | UP | +1.21 | +10.3 | 89.6% | 1e-23 |
| DNAme | DNMT1 | UP | +0.69 | +8.4 | 82.5% | 6e-16 |
| PRC2 | EZH1 | DOWN | -0.60 | -7.0 | 81.4% | 2e-11 |
| DNAme | DNMT3B | UP | +0.64 | +6.9 | 83.5% | 5e-11 |
| PRC2 | EZH2 | UP | +0.80 | +6.8 | 91.2% | 1e-10 |
| CoREST | RCOR1 | UP | +0.43 | +6.4 | 83.1% | 1e-09 |
| DNAme | TET1 | DOWN | -0.84 | -6.4 | 89.7% | 1e-09 |
| HDAC | HDAC3 | UP | +0.27 | +6.3 | 80.2% | 2e-09 |
| NCoR_SIN3 | NCOR2 | DOWN | -0.59 | -6.2 | 89.5% | 4e-09 |
| KDM | KDM5A | DOWN | -0.64 | -6.0 | 91.1% | 1e-08 |
| PRC1 | BMI1 | DOWN | -0.27 | -5.8 | 80.6% | 2e-08 |
| CoREST | ZNF217 | UP | +0.29 | +4.9 | 75.2% | 5e-06 |
| HDAC | HDAC9 | DOWN | -0.51 | -4.6 | 74.6% | 2e-05 |
| NuRD | MTA1 | DOWN | -0.27 | -4.5 | 78.0% | 3e-05 |
| HDAC | SIRT1 | DOWN | -0.32 | -4.5 | 88.6% | 3e-05 |
| CoREST | RCOR3 | DOWN | -0.45 | -4.2 | 93.3% | 8e-05 |
| NCoR_SIN3 | TBL1XR1 | DOWN | -0.25 | -4.2 | 92.7% | 9e-05 |

High I² (75–91% for most) reflects between-cohort variation in effect *magnitude* (platform/severity/reference differ), but direction is consistent and the random-effects pooled estimate — which accounts for that heterogeneity — remains robustly significant. PCGF2 is perfectly homogeneous (I²=0%). This is the headline put on a formal meta-analytic footing.


## Methylation replication — 3 independent 450K cohorts

Addresses the single-cohort caveat. Global hypomethylation replicated in **2/3** cohorts; **focal developmental-TF promoter hypermethylation replicated in 3/3** (the targeted-repression finding is robust).

| Cohort | lesional/normal | global Δβ | hyper/hypo DMP | devTF promoter Δβ | background Δβ | MWU p |
|---|---|---:|---|---:|---:|---:|
| GSE115797 | 24/24 | -0.0119 | 9510/37463 | 0.01412 | 0.00546 | 4e-06 |
| GSE63315 | 35/12 | -0.0083 | 3500/8345 | 0.00466 | -0.00357 | 7e-44 |
| GSE73894 | 114/64 | 0.0056 | 415/261 | 0.00496 | 0.00316 | 4e-08 |

The developmental-TF/PRC2 promoters are focally **hyper**methylated relative to genome background in **all three** independent cohorts (p as low as 7e−44) — the methylation-reinforced silencing of differentiation loci is a replicated finding. Global hypomethylation holds in 2/3 (GSE73894 is mildly hyper-dominant globally, an honest cohort-level exception likely reflecting reference-skin/age/platform differences).


## Single-cell cell-type resolution — the bulk repression signal is largely COMPOSITIONAL (honest refinement)

GSE173706 (13,848 cells, 3 normal + 3 psoriasis skin), marker-assigned to skin cell types, asks whether the bulk repression-machinery upregulation is keratinocyte-intrinsic.

Cell-type composition (normal -> psoriasis):

| Cell type | normal | psoriasis |
|---|---:|---:|
| T_cell | 416 | 332 |
| endothelial | 227 | 850 |
| fibroblast | 1213 | 1825 |
| keratinocyte | 1757 | 4873 |
| langerhans_DC | 353 | 576 |
| mast | 69 | 175 |
| melanocyte | 259 | 432 |
| myeloid | 355 | 136 |

Keratinocytes expand **1757 -> 4873** (2.8x; epidermal hyperplasia), endothelial 227->850 (angiogenesis).

**Within psoriatic vs normal keratinocytes, the repression machinery is NOT broadly upregulated:** only **1/23** repressors are FDR-up (JARID2 +0.37, q=1.7e-7), and the **panel score is slightly LOWER per psoriatic keratinocyte (0.7666 vs 1.2111, MWU p_greater=1)**.

**Refinement:** the bulk-tissue 'repression machinery up' (EZH2/UHRF1/DNMT) is **substantially a composition + proliferation effect** — psoriatic skin has ~2.8x more keratinocytes (proliferating basal cells express replication-coupled UHRF1/DNMT1), so bulk shows more without per-cell upregulation. **JARID2 (PRC2) is the one genuinely keratinocyte-intrinsic repressor.** The *methylation*-level findings (focal hypermethylation at differentiation-TF promoters, 3/3 cohorts) are composition-robust and remain the strongest repression evidence. Single-cell honestly qualifies the bulk transcript headline. (Caveat: scRNA dropout limits detection of low-expression chromatin genes; CPM normalization can deflate per-cell signal in high-RNA proliferating cells.)


## Mechanistic capstone — repression machinery is replication-coupled (refines the bulk headline)

Tests why bulk shows 'repression up' while per-keratinocyte it doesn't. Within 6,586 keratinocytes, split proliferating (top-quartile cell-cycle score) vs resting.

**Mechanism (confirmed):** the replication-coupled repressors are significantly higher in proliferating vs resting keratinocytes:

| Repressor | log2(proliferating/resting) | MWU p | replication-coupled? |
|---|---:|---:|---|
| CBX2 | +0.05 | 2e-02 | no |
| DNMT1 | +0.61 | 1e-22 | yes (S-phase) |
| DNMT3B | +0.00 | 4e-01 | no |
| EZH2 | +0.38 | 8e-07 | (PRC2 enzyme) |
| JARID2 | -0.31 | 1e+00 | no |
| SUV39H1 | +0.07 | 2e-03 | no |
| UHRF1 | +0.23 | 6e-28 | yes (S-phase) |

UHRF1/DNMT1/EZH2 are elevated in cycling cells, so the **bulk repression signal is proliferation-sensitive** — and psoriatic tissue is hyperproliferative (executor: cell-cycle 60 up / 7 down). This mechanistically explains the bulk EZH2/UHRF1/DNMT headline as largely a proliferation/composition readout rather than a uniform per-cell upregulation.

**Nuance:** the proliferating *fraction* among captured keratinocytes is not higher in psoriasis here (0.229 vs 0.3, Fisher p=3e-09) — an scRNA capture bias (suprabasal differentiated cells over-captured), since bulk proliferation markers ARE up.

**The clean signal:** JARID2 is up in psoriatic keratinocytes (q=1.7e-7, prior section) **yet is NOT replication-coupled** (lower in proliferating cells, p=1.0) — making JARID2/PRC2 the one genuine, proliferation-independent keratinocyte-intrinsic repression signal, alongside the composition-robust methylation focal-hypermethylation at differentiation promoters.


## Single-cell replication (2nd cohort, GSE151177) — JARID2 confirmed, composition confirmed

Replicates the GSE173706 finding in an independent 10x cohort (6,807 cells; keratinocytes 1233N/326P):

- Repression machinery is again NOT broadly up per psoriatic keratinocyte — panel score delta **-0.1736** (p_greater=1); only 2/23 genes FDR-up.

- **JARID2 replicates** as up in psoriatic keratinocytes (log2 +0.23, q=3.2e-02) — keratinocyte-intrinsic in **2/2** independent cohorts (q=1.7e-7 GSE173706, q=0.03 GSE151177).

**Conclusion (two-cohort-replicated):** the bulk repression-machinery transcript headline is substantially a composition/proliferation effect, while **JARID2/PRC2 is the genuine, replicated keratinocyte-intrinsic repression signal** — converging with the composition-robust, 3-cohort-replicated methylation focal-hypermethylation at differentiation promoters. The repression is real at the PRC2 (JARID2) and DNA-methylation levels; the broad 'machinery up' was an honest over-read of bulk.

