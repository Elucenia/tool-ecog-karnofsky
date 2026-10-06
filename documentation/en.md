<!-- ELUCENIA technical documentation · ecog-karnofsky · en · no clinical/professional/rights approval -->

# ECOG and Karnofsky

[conditions, sources and permissions](https://elucenia.org/en/tools/ecog-karnofsky)

## How to use

Use the tool in the portal or open index.html through a local HTTP server. Select the language, complete the fields and calculate.

## Inputs and units

### Karnofsky Performance Status

`kps`

- `0` — 0% · Dead
- `10` — 10% · Moribund
- `20` — 20% · Very ill; active supportive care required
- `30` — 30% · Severely disabled; hospitalization indicated
- `40` — 40% · Disabled; needs special care
- `50` — 50% · Requires considerable assistance and frequent medical care
- `60` — 60% · Requires occasional assistance
- `70` — 70% · Cares for self but unable to work
- `80` — 80% · Normal activity with effort
- `90` — 90% · Normal activity; minimal signs or symptoms
- `100` — 100% · Normal; no complaints or evidence of disease

## Method edition

ECOG 0–5/Oken 1982; ECOG-ACRIN KPS correspondence 90–100/70–80/50–60/30–40/10–20/0

## Documented formula

ECOG-ACRIN mapping: Karnofsky 100–90% = ECOG 0; 80–70% = ECOG 1; 60–50% = ECOG 2; 40–30% = ECOG 3; 20–10% = ECOG 4; 0% = ECOG 5 (death).

The scales are not identical: ECOG-ACRIN itself presents this table as “one way” of mapping one to the other.

## Limits and population

The ECOG-ACRIN table presents a commonly used correspondence between ECOG and Karnofsky, among several possible ways to map the scales. They describe functional capacity and help define trial populations; conversion alone does not establish eligibility for a treatment. Functional assessment and clinical protocol criteria must be preserved.

## References

- [Oken MM et al. Toxicity and response criteria of the Eastern Cooperative Oncology Group. Am J Clin Oncol, 1982.](https://doi.org/10.1097/00000421-198212000-00014)

- [ECOG-ACRIN Cancer Research Group. ECOG Performance Status Scale (comparação com a escala de Karnofsky).](https://ecog-acrin.org/resources/ecog-performance-status/)

## Reproduce the technical tests

Run node test.cjs in the root directory of this repository to repeat the recorded synthetic cases. Original inputs, expectations and tolerances are preserved. Technical tests do not constitute clinical validation.

```sh
node test.cjs
```

tool.json contains sources, edition and review scope. examples.json retains synthetic inputs and expectations; results.json records the obtained results.

[Record and references](../tool.json) · [JavaScript code](../calculator.js) · [Reference cases](../examples.json) · [results.json](../results.json)

## Review and conditions of use

Independent clinical review has not been performed.

This interface is an authorial translation, not an official or certified edition. Independent clinical review, professional language review and instrument rights clearance have not been performed.

Formula or classification result. Interpretation, care and applicability depend on professional assessment and the selected source.

## License and attribution

Apache-2.0 applies only to ELUCENIA code. Rights to instruments, publications, translations and data remain with their respective holders. Preserve LICENSE and NOTICE.

ELUCENIA · Felipe Guedes · Copyright © 2026

## Documented results

The information below preserves the method outputs for synthetic examples. It does not constitute independent clinical validation.

### 1

Fully active, no restriction compared with pre-disease status

| Result details | |
| --- | --- |
| Karnofsky 90% | Able to carry on normal activity; minimal signs or symptoms of disease |
| Karnofsky range for this ECOG | 100–90% |


### 2

Restricted in strenuous physical activity, but ambulatory and able to do light or sedentary work

| Result details | |
| --- | --- |
| Karnofsky 70% | Cares for self, but is unable to carry on normal activity or to do active work |
| Karnofsky range for this ECOG | 80–70% |


### 3

Ambulatory and able to care for self, but unable to work; up and about more than 50% of waking hours

| Result details | |
| --- | --- |
| Karnofsky 50% | Needs considerable assistance and frequent medical care |
| Karnofsky range for this ECOG | 60–50% |

ECOG ≥ 2: most cytotoxic chemotherapy trials included only ECOG 0 to 1 (or 2); weigh benefit and toxicity.


### 4

Limited self-care; in bed or chair more than 50% of waking hours

| Result details | |
| --- | --- |
| Karnofsky 30% | Severely disabled; hospital admission indicated, though death not imminent |
| Karnofsky range for this ECOG | 40–30% |

ECOG ≥ 2: most cytotoxic chemotherapy trials included only ECOG 0 to 1 (or 2); weigh benefit and toxicity.

