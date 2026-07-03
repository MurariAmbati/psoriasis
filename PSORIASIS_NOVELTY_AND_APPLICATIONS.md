# What Can We Use These Discoveries For? — Translational Applications

**Psoriasis deep-dive (repression-os-v2) · applications synthesis**

This document answers, concretely and per-discovery: *what is each finding for, how ready is it, and what is the next experiment.* Every application carries a readiness level and an honest bound.

---

## Use-class 1 — DIAGNOSTIC / STRATIFICATION

### 1a. 6-gene lesional-classifier panel
**What it's for:** A compact transcriptomic panel — **ADAMDEC1, AKR1B10, BTC, PI3, S100A12, TCN1** — that distinguishes lesional from normal/non-lesional skin from a biopsy or (future) tape-strip sample.
**Evidence:** Held-out AUROC **0.806** (lesional vs normal, independent cohort GSE14905) and **0.987** (lesional vs non-lesional, GSE30999); permutation p=0.0005. Trained on GSE13355, tested on cohorts never seen in training.
**Readiness:** Analytical proof-of-concept. **Bound:** train resubstitution 1.00 → overfitting gap is real; needs prospective validation on a fresh cohort and a platform-independent assay (qPCR/NanoString) before any clinical claim.
**Next experiment:** Lock the 6 genes, run a qPCR panel on a prospective biopsy set with treatment-response follow-up to test whether baseline panel score predicts responder status.

### 1b. Differentiation-silencing score as a relapse/severity axis
**What it's for:** A second, orthogonal readout — the degree of differentiation-TF silencing (GATA3/FOXC1/GATA6/IRX1/TBX-family) — as a candidate **relapse-risk** marker distinct from inflammatory load.
**Evidence:** The silenced program is 71% PSO-enriched vs atopic dermatitis (more disease-specific than the shared inflammatory axis); reproducible across 5 cohorts.
**Readiness:** Hypothesis. **Bound:** the relapse link is mechanistic, not yet tested against longitudinal relapse data.
**Next experiment:** Score the silencing axis in pre/post-phototherapy paired biopsies and correlate residual silencing with time-to-relapse.

---

## Use-class 2 — THERAPEUTIC

### 2a. TEAD4 small-molecule inhibition (palmitate pocket) — TOPICAL
**What it's for:** A skin-directed small-molecule targeting the TEAD4 lipid pocket, to dial down the Hippo/YAP transcriptional output that tracks with keratinocyte hyperproliferation.
**Evidence:** 388-design de novo series docked into the validated 8CAA pocket (redock RMSD 1.0 Å); best −7.75 kcal/mol, 46 beat the parent lead; **9/10 top leads are topical-favorable** (MW<500, logP 1–3.5) — well-suited to a topical formulation, the preferred route for localized plaques.
**Readiness:** Computational lead series. **Bound:** docking-ranked starting points only; all weaker than the crystal ligand (−9.18); no synthesis, no MD/FEP, no cellular assay. TEAD4's *causal* role in psoriasis did not replicate cross-cohort — target validation is incomplete.
**Next experiment:** Synthesize the top 3 topical-favorable 7-deazapurine leads; test TEAD-reporter (8×GTIIC luciferase) inhibition in keratinocytes; measure effect on differentiation markers (KRT10, FLG).

### 2b. Rational de-repression (epigenetic) — reactivate the differentiation program
**What it's for:** Repurpose approved epigenetic drugs (**azacitidine/decitabine** DNMT inhibitors; EZH2/HDAC inhibitors) to *reverse* the methylation-silencing of differentiation enhancers — treating the "scar," not the inflammation.
**Evidence:** The scar is 77% persistent hyper-methylation at developmental-TF enhancers (repo data, CpG-island enrichment p=1.9e-13); the drugs are phase-4 approved with known mechanism.
**Readiness:** Mechanistic proposal. **Bound:** no reactivation assay performed; systemic hypomethylating agents carry toxicity and the nucleosides are **not skin-penetrant** (logP −2 to −3) — would need a delivery vehicle or a skin-permeable analog.
**Next experiment:** Treat patient-derived keratinocytes / 3D skin equivalents with low-dose decitabine; assay demethylation + re-expression of GATA3/FOXC1 and restoration of differentiation.

### 2c. YAP-TEAD interface disruptor (biologic modality)
**What it's for:** A stapled peptide / biologic blocking the YAP-TEAD protein-protein interface (distinct from 2a's pocket), for a more selective anti-Hippo mechanism.
**Evidence:** 21 interface hotspots mapped on TEAD4 (PDB 6SEN); 8 core residues (SER418, ASP272, TYR429, LYS297...); stapled-peptide TEAD inhibitors exist in the literature.
**Readiness:** Interface characterization. **Bound:** no binder designed (GPU design unavailable); biologic delivery to epidermis is itself unsolved.

---

## Use-class 3 — MECHANISTIC HYPOTHESIS (testable science)

### 3. The differentiation "scar" as a relapse substrate
**What it's for:** A falsifiable model: psoriasis plaques clear inflammation under therapy but retain a keratinocyte-intrinsic epigenetic memory (silenced differentiation enhancers) that primes the same site to relapse.
**Testable predictions:** (1) resolved lesional skin retains differentiation-TF silencing vs never-lesional skin; (2) residual silencing magnitude predicts relapse location; (3) de-repression (2b) reduces relapse rate in a model.
**Bound:** the dominant relapse model is tissue-resident memory T cells; the keratinocyte-scar view is a minority, complementary hypothesis, and our TEAD4 causal claim did not replicate.

---

## Use-class 4 — CROSS-DISEASE PLATFORM (the reusable engine)

### 4. Pan-epithelial mechanism map
**What it's for:** A reusable engine (this batch) that tests whether any psoriasis-derived mechanism recurs across 29 diseases — directly serving the "apply to every disease later" goal.
**Key finding:** The Hippo/differentiation-silencing axis is a **carcinoma pathway** (breast/digestive/prostate/colorectal association ~1.0; psoriasis ~0.25, near-bottom). 
**What this is FOR, honestly:** (1) it tells us the psoriasis novelty is *repositioning a cancer pathway to inflammatory skin*, not a new mechanism; (2) it flags that TEAD4 tool compounds developed in oncology could be repurposed to psoriasis; (3) the engine itself generalizes — point it at any pack's signature to rank mechanism-sharing across the disease atlas.
**Next use:** Run the engine on the next high-priority pack (e.g. AML modules) to find *its* under-explored-but-established axis.

---

## Bottom line

| Discovery | Best use | Readiness | Hard bound |
|---|---|---|---|
| 6-gene panel | Diagnostic classifier | PoC (needs prospective) | overfit gap; platform transfer |
| Differentiation-silencing score | Relapse-risk marker | Hypothesis | no longitudinal test |
| TEAD4 SM series (topical) | Therapeutic lead | Computational | starting points; causal role unproven |
| De-repression (aza/deci) | Scar-reversal therapy | Mechanistic | no assay; not skin-penetrant |
| YAP-TEAD interface | Biologic disruptor | Interface map | no binder designed |
| Cross-disease engine | Repositioning platform | **Operational** | descriptive (association-based) |

The two most *actionable* items are the **topical TEAD4 lead series** (synthesize + reporter assay) and the **cross-disease engine** (already operational, reusable across all 29 packs). The two most *honest-negative* framings — that TEAD4 is a known carcinoma pathway and that its psoriasis causal role didn't replicate — are what make the remaining claims trustworthy.
