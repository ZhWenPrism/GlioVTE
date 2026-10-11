<div align="center">

# GlioVTE

**Postoperative venous thromboembolism prediction for patients with glioma**

[![Status](https://img.shields.io/badge/Status-research_in_development-D97706?style=flat-square)](#project-status)
[![Collaboration](https://img.shields.io/badge/Collaboration-Beijing_Tiantan_Hospital-2563EB?style=flat-square)](#collaboration)
[![Scope](https://img.shields.io/badge/Scope-postoperative_VTE_prediction-7C3AED?style=flat-square)](#research-scope)

<sub>clinical risk modeling · perioperative data · interpretable prediction · collaborative research</sub>

</div>

GlioVTE is a collaborative research project with **Beijing Tiantan Hospital** focused on developing a postoperative venous thromboembolism prediction model for patients undergoing surgery for glioma.

The project is intended to organize perioperative clinical information into a reproducible prediction workflow, investigate patient-level VTE risk after glioma surgery, and support future research on interpretable clinical risk stratification. The repository currently provides the collaboration structure and research scaffold; it does not yet publish patient data, trained models, clinical performance claims, or deployment-ready code.

## Research scope

The planned research workflow covers four connected components:

1. **Cohort definition** — establish explicit inclusion, exclusion, index-surgery, follow-up, and postoperative VTE outcome rules.
2. **Perioperative representation** — organize demographics, tumor-related variables, comorbidities, laboratory measurements, operative information, medications, mobility, and other prediction-time-available factors.
3. **Risk modeling** — compare transparent clinical baselines with machine-learning models under patient-level, leakage-controlled evaluation.
4. **Clinical interpretation** — examine calibration, discrimination, subgroup behavior, decision thresholds, and patient-level explanations without treating model attribution as causal evidence.

The final prediction time, observation window, outcome horizon, feature set, and validation protocol will be frozen before confirmatory evaluation. Until those definitions and source artifacts are approved, this repository should be read as a project framework rather than a completed prediction system.

## Planned workflow

```text
Clinical source data
        │
        ▼
Cohort and outcome specification
        │
        ▼
Prediction-time feature construction
        │
        ▼
Patient-level development and validation splits
        │
        ├── Clinical baseline models
        ├── Machine-learning models
        └── Calibration and uncertainty analysis
        │
        ▼
Discrimination · calibration · subgroup analysis
        │
        ▼
Research-only risk report and interpretation
```

## Repository layout

```text
GlioVTE/
├── assets/                         # public-safe figures and diagrams
├── configs/                        # cohort, feature, model, and experiment settings
├── data/
│   └── README.md                   # data-access boundary; no patient data
├── docs/
│   ├── RESEARCH_SCOPE.md           # intended study and open questions
│   └── DATA_GOVERNANCE.md          # privacy and release requirements
├── models/                         # future model definitions
├── scripts/                        # future training and evaluation entry points
├── src/
│   └── gliovte/                    # future reusable package
├── tests/                          # future unit and integration tests
├── .github/
│   ├── ISSUE_TEMPLATE/             # structured research and engineering requests
│   ├── CODEOWNERS                  # review routing
│   └── pull_request_template.md    # collaborative review checklist
├── CONTRIBUTING.md                 # branch, commit, review, and privacy rules
└── README.md
```


## Project status

GlioVTE is currently under active research development. Public materials are limited to the project scope, governance rules, collaboration workflow, and empty implementation scaffold. Model performance will be added only after the cohort, outcome, prediction time, evaluation protocol, and result provenance have been formally verified.

