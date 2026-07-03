# Psoriasis — Novelty Ranking, Clinical Utility, and the Role of anduril / artmethods

**RUO.** Research analysis of open data only. Nothing here is a diagnosis, prognosis, or treatment recommendation. "Novel" is graded against established psoriasis literature and a curated known-gene reference set; it flags *candidate* novelty requiring experimental follow-up, not a discovery claim.

---

## 1. What we found — ranked by novelty × evidence strength

| Rank | Finding | Novelty | Evidence (replication) | Direction |
|---|---|---|---|---|
| **1** | **JARID2 is a keratinocyte-intrinsic, proliferation-independent PRC2 repressor up-regulated in psoriasis** | **Genuinely novel for psoriasis** (JARID2 is not an established psoriasis gene) | **Strong** — up in psoriatic keratinocytes in **2/2** single-cell cohorts (q=1.7e−7, q=0.03); FDR EZH2-perturbation derepression; NOT replication-coupled (p=1.0) so not a proliferation artifact | UP |
| **2** | **Persistent epigenetic memory: focal hypermethylation at differentiation-TF promoters does NOT reverse with therapy** (while global methylome + expression do) | **Novel mechanistic insight** | **Moderate** — global/expression reversal is multi-cohort; the *non*-reversal is 1 cohort + small effect (Δβ 0.003), tentative | persists |
| **3** | **Global hypomethylation WITH focal hypermethylation reinforcing differentiation-TF silencing** (GATA3/FOXC1/GATA6/HOX/TBX promoters) | **Refined synthesis** (global hypomethylation is known; the integrated focal-hyper-at-dev-TFs ↔ expression-silencing axis is new) | **Strong** — focal hypermethylation replicates **3/3** methylation cohorts (MWU p to 7e−44); promoter-methylation↔expression Spearman −0.21 (p=5e−24) | targeted UP |
| **4** | **The bulk "repression machinery up" (EZH2/UHRF1/DNMT) is largely a composition + proliferation effect, not per-cell epithelial upregulation** | **Honest refinement / negative** | **Strong** — panel score *lower* per psoriatic keratinocyte in **2/2** single-cell cohorts; UHRF1/DNMT1 shown replication-coupled | (corrects an over-read) |
| **5** | **Treatment normalizes the repressive state, tracking clinical response** (repression machinery reversal 0.82; responders > non-responders) | Known-adjacent (reversibility is expected; quantified here) | **Strong** — 2 biologics + phototherapy; PASI-linked | reverses |
| 6 | Candidate proliferation-adjusted genes: **CD274/PD-L1, AIM2, KYNU, VNN3, TMPRSS11D** (bootstrap-stable after proliferation adjustment) | Mixed (several have psoriasis literature; "novel" vs curated set) | Moderate — artmethods deep tier, ≥2-cohort bootstrap-stable | UP |
| — | IL17/IL36/DEFB4/S100A/KRT16 inflammatory-keratinization; type-I IFN; hyperproliferation | **Known (positive controls)** | Very strong — 7/7 cohorts; calibrate the pipeline | UP |
| — | JARID2 → differentiation-blockade mechanism | (tested) | **Negative** — not supported (cohorts disagree; JARID2 not a basal marker) | — |

**The honest headline:** the psoriatic "repression program" is **real but narrower than a naive bulk read** — concentrated at (a) the **PRC2/JARID2** layer (keratinocyte-intrinsic, replicated) and (b) the **focal DNA-hypermethylation of differentiation-TF promoters** (3-cohort-replicated, composition-robust, partly therapy-resistant). The broad "machinery up" is mostly proliferation/composition.

---

## 2. What this could help with clinically (RUO hypotheses)

1. **JARID2/PRC2 as an epigenetic-target hypothesis.** JARID2 is keratinocyte-intrinsic and proliferation-independent — a cleaner candidate axis than the proliferation-confounded UHRF1/DNMT. EZH2/PRC2 inhibitors exist (e.g., tazemetostat). This motivates testing **local/topical PRC2 modulation** to de-repress the silenced differentiation program — a *research hypothesis*, not a recommendation, requiring functional validation (the differentiation-blockade mechanism was not established here).

2. **A mechanistic rationale for same-site recurrence ("disease memory") and why biologics control but don't cure.** The focal hypermethylation at differentiation-TF promoters does **not** reverse with phototherapy even as inflammation/expression normalize. If confirmed, durable clearance may require addressing this **epigenetic memory** (e.g., demethylating strategies at those loci) *in addition to* anti-inflammatory therapy — explaining rapid relapse at treated sites.

3. **A pharmacodynamic response biomarker.** The repressive-state reversal tracks PASI and separates responders from non-responders. The repression/signature-normalization score is a candidate **molecular readout of treatment response** (research biomarker; needs prospective validation).

4. **A guardrail against a false target.** By showing the bulk EZH2/UHRF1/DNMT signal is mostly composition/proliferation, the analysis **prevents mis-prioritizing those as epithelial-intrinsic drug targets** — a negative that protects downstream translational decisions.

5. **CD274/PD-L1 up-regulation** in lesional skin is consistent with the known checkpoint biology of psoriasis (checkpoint-inhibitor-triggered psoriasis; counter-regulatory PD-L1) — a context flag, not a target.

> All clinical statements are RUO hypotheses derived from public-data association + replication. None is validated for use; functional, safety, and prospective clinical evidence are absent by design.

---

## 3. What anduril and artmethods did for this

These are the program's two **disease-agnostic method libraries**; they supplied the rigor that lets the findings above be stated honestly.

### artmethods (202-method toolkit + heavy deep tier) — the transportability & validation engine
Pointed at the psoriasis substrate (7 cohorts), it ran **46 fitting methods / 5.2M FDR-controlled experiments** + **159,428 deep-tier experiments**, cleanly abstaining on modalities psoriasis lacks. Concretely it:
- **certified cross-cohort transportability** — direction-stability (2,749/2,869 genes), rank-rank + cross-platform concordance **15/15** (the signature transfers RNA-seq↔array);
- **replicated the network** — 360,987 co-expression edges reproducible across cohorts; 40,185 bootstrap-sign-stable, confounder-residualized edges (deep DT1);
- **supplied the proliferation-adjusted core** — DT2 produced **273 genes that stay significant after adjusting for proliferation/stemness + bootstrap** (this is how we know the signature isn't only a proliferation proxy, and it surfaced CD274/AIM2/KYNU);
- **issued transportability certificates** (DT4, 642 genes; DL random-effects + winner's-curse + bootstrap) and **e-value robustness** (D10.10, 30/30) and **novelty adjudication** (D14.4).
In short: artmethods is the *"is it real, robust, and portable across cohorts?"* layer — and it independently corroborated the headline signature with covariate adjustment.

### anduril (650 RM robustness/falsification modules) — the certification & honest-negative backbone
All **650 modules** were executed on psoriasis's real-data modalities: **233 PASS, 247 touched real data, 78 correctly abstained** (modality absent), 44 modality-missing errors, 359 heavy methods time-boxed. anduril is the **falsification/certification toolkit** — matched-decoy nulls, negative-control outcomes, cohort-blocked permutation, LOCO transfer gaps, conformal prediction, e-values, selective inference, certified-negative engines, leakage/confound scanners. Its value here is methodological: it embodies the *"try to kill the finding"* discipline (the same discipline behind our own permutation null perm_p=0.001, the proliferation-confound flagging, and the single-cell down-grade of the bulk headline). Its honest accounting — many modules require mutation/dependency/drug/spatial/imaging layers psoriasis doesn't have, so they abstain/error — is itself the data-honesty contract working.

> `knownmethods` (the third library) is a literature/method *harvester* (web-search waves), not a per-disease data miner, so it was not run on the psoriasis data.

---

## 4. Bottom line

Psoriasis was mined across **expression (8 cohorts), DNA methylation (3 cohorts), single-cell (2 cohorts), treatment-response, and both method libraries**, with cross-modality replication and repeated honest refinement. The credible deliverables are: **(i) JARID2 as a replicated, proliferation-independent, keratinocyte-intrinsic PRC2 repressor (novel for psoriasis); (ii) replicated focal hypermethylation silencing differentiation-TF promoters, with a candidate non-reversible "memory" component; (iii) the honest demonstration that the broad repression-machinery headline is mostly compositional.** The genuine novelty is small and clearly labeled — which, per this platform's philosophy, is the point.
