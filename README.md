# PortNormand: ANSSI Compliance Case Study

> A two-day compliance exercise: helping a (fictional) French port operator understand the role of **ANSSI**, qualify its regulatory status under **LPM** and **NIS2**, notify a cyber incident, choose qualified providers, and prepare for a compliance inspection.

![Status](https://img.shields.io/badge/status-in%20progress-yellow)
![Domain](https://img.shields.io/badge/domain-cybersecurity%20compliance-0A66FF)
![Framework](https://img.shields.io/badge/framework-NIS2%20%7C%20LPM-blue)
![License](https://img.shields.io/badge/license-MIT-green)

## Table of contents

- [Context](#context)
- [Deliverables and progress](#deliverables-and-progress)
- [Repository structure](#repository-structure)
- [Methodology](#methodology)
- [Key references](#key-references)
- [Team](#team)
- [Disclaimer](#disclaimer)
- [License](#license)

## Context

**PortNormand** is a fictional port operator (container freight, oil terminals, maritime traffic management). It has been an **Operator of Vital Importance (OIV, "Transports" sector)** since 2015, and has recently acquired a European multimodal logistics company. After receiving a letter from ANSSI announcing a compliance support phase linked to the transposition of the **NIS2 Directive**, nobody in the organisation knows whom to contact or which obligations already apply under the **LPM** (Military Programming Law).

Our team acts as PortNormand's **compliance cell** and must:

1. Clarify ANSSI's role and its counterparts
2. Determine the organisation's precise regulatory status
3. Prepare the organisation to notify an incident correctly
4. Identify the providers and qualification schemes to use
5. Anticipate an ANSSI compliance inspection

## Deliverables and progress

| # | Deliverable | Day | File | Status |
|---|---|---|---|---|
| 1 | Missions / situations table | 1 | [`day1/ex1-missions-situations.md`](day1/ex1-missions-situations.md) | Draft |
| 2 | Regulatory status note (1 page) | 1 | [`day1/ex2-regulatory-status.md`](day1/ex2-regulatory-status.md) | Draft |
| 3 | Actors table and information-flow diagram | 1 | [`day1/ex3-actors-map.md`](day1/ex3-actors-map.md) | Todo |
| 4 | Notification timeline and draft message | 2 | [`day2/ex4-incident-notification.md`](day2/ex4-incident-notification.md) | Todo |
| 5 | Qualification table (PASSI / PDIS / PRIS / SecNumCloud) | 2 | [`day2/ex5-qualifications.md`](day2/ex5-qualifications.md) | Todo |
| 6 | Inspection readiness action plan (1 page) | 2 | [`day2/ex6-inspection-readiness.md`](day2/ex6-inspection-readiness.md) | Todo |

Supporting material: [`docs/glossary.md`](docs/glossary.md) and [`docs/qcm-study-notes.md`](docs/qcm-study-notes.md).

## Repository structure

```text
.
├── README.md
├── LICENSE
├── CONTRIBUTING.md
├── .gitignore
├── day1/                       # Understand ANSSI and qualify PortNormand
│   ├── ex1-missions-situations.md
│   ├── ex2-regulatory-status.md
│   └── ex3-actors-map.md
├── day2/                       # React to an incident and prepare for an inspection
│   ├── ex4-incident-notification.md
│   ├── ex5-qualifications.md
│   └── ex6-inspection-readiness.md
└── docs/
    ├── assets/                 # Diagrams (PNG/SVG)
    ├── glossary.md
    └── qcm-study-notes.md
```

## Methodology

- **Primary sources first.** Legal claims are checked against official texts (Légifrance, EUR-Lex) and ANSSI publications on cyber.gouv.fr.
- **Uncertainty is explicit.** Open questions and assumptions are listed in each deliverable, never hidden.
- **One exercise, one file.** Each deliverable follows the format required by the brief (table, one-page note, timeline, etc.).
- **Dated legal status.** Each regulatory statement mentions the date it was last verified.

## Key references

- [cyber.gouv.fr](https://cyber.gouv.fr): ANSSI institutional website (missions, frameworks, qualified provider directory)
- [Article 22, Law No. 2013-1168 (LPM)](https://www.legifrance.gouv.fr): Légifrance
- [Directive (EU) 2022/2555 (NIS2)](https://eur-lex.europa.eu): EUR-Lex
- [ENISA](https://www.enisa.europa.eu): EU cybersecurity agency, NIS2 resources

## Team

| Name | GitHub |
|---|---|
| [Member 1] | [@mugire-can](https://github.com/mugire-can) |


## Disclaimer

This is an **educational case study** completed as part of a training programme at La Plateforme. PortNormand is fictional. Nothing here is legal advice. The original course brief is not redistributed in this repository.

## License

Released under the [MIT License](LICENSE).
