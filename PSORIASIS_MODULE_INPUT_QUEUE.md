# Psoriasis KnownMethods Discovery Plan

KnownMethods planning report for psoriasis. It records the local literature-method harvest state and maps the current psoriasis data modalities to the planner without making scientific claims.

- Seed queries available: 600
- Methods corpus present: false
- Method records: 0
- Experiments file present: false
- Experiment records: 0
- Report digest: `958df0507da7c73713f352a81ca05e7b5b3efde67ed3735aea9f326ae2475f7c`

## Seed Wave

| Axis | Count or cap |
| --- | ---: |
| Family terms in seeds.yaml | 105 |
| Modality terms in seeds.yaml | 9 |
| Intent terms in seeds.yaml | 10 |
| Families per wave cap | 40 |
| Modalities per wave cap | 9 |
| Intents per wave cap | 6 |
| Query cap | 600 |
| Planned seed queries | 600 |

## Current Matrix Chain Plan

- Modalities: `clinical`, `expr`, `expression`, `geo`
- Status: `corpus_absent_or_not_enumerated`

## Declared Disease-Pack Plan

- Modalities: `clinical`, `expr`, `expression`, `geo`, `pathway`, `single_cell`, `target_evidence`
- Status: `corpus_absent_or_not_enumerated`

## Next Required

- run knownmethods harvest wave with open-source literature endpoints if method corpus is desired
- enumerate harvested methods into experiments.jsonl
- filter experiments against current psoriasis matrix modalities and disease-pack declared modalities
- emit method abstention rows for missing modality requirements
