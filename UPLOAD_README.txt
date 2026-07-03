PSORIASIS SECTION — repression-os-v2
====================================
This is the psoriasis section of the repression-os-v2 repository, cloned verbatim
(diseases/MONDO_0005083_psoriasis), plus a pinned Python environment spec.

To upload to GitHub manually:
  1. Create/choose a repo (or the diseases/ path inside repression-os-v2).
  2. Copy the psoriasis/ folder in at diseases/MONDO_0005083_psoriasis/
     (or wherever you want it), commit, and push.

CONTENTS (psoriasis/)
  manuscript/              earlier manuscript drafts
  nature_manuscript/       Nature-depth expansion + clinical_epigenetics_submission/
                           (the current Springer Nature template manuscript, figures,
                            supplementary information, additional files, cover letter)
  novel_discoveries/       tables + figures from the discovery batches
  novelty_and_applications/ project-level novelty & applications narratives
  repression/              repression-analysis outputs
  results/                 full result envelopes (JSON) from every analysis stage
  batch2_constructions/    generative-chemistry + construction outputs
  reports/                 summary reports
  sentinel/, vindicate/    QC / verification artefacts
  *.lock.json, manifest.json  data + experiment provenance locks

ENVIRONMENT
  environment.yml / requirements.txt  pinned package versions (Python 3.13; scanpy
    1.12.2; numpy 2.4.6; scipy 1.18.0; pandas 2.3.3; scikit-learn 1.9.0; rdkit
    2026.03.1; statsmodels 0.14.6; leidenalg 0.12.0; umap-learn 0.5.12; matplotlib
    3.10.9; networkx 3.6.1; biopython; reportlab)
  EXTERNAL_TOOLS.txt  AutoDock Vina (build f458505) — install separately.

All results were computed from public GEO data; the chemistry is docking-ranked and
hypothesis-generating (no compound synthesized/assayed).
