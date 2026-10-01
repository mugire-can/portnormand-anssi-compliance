# Exercise 5: Qualification Frameworks

**Status:** Done
**Format:** Table of need / required qualification / justification, one need per row
**Last verified:** 2026-10-01 (framework versions read on the ANSSI qualification page)

## 1. Qualification, certification, label: the difference

| Term | Applies to | Issued by | Example |
|---|---|---|---|
| **Qualification** | Services and products, with a high level of trust (Decree no. 2015-350) | ANSSI | PASSI, PDIS, PRIS, PACS, SecNumCloud |
| **Certification** | Products evaluated against a standard | ANSSI, via licensed evaluation labs (CESTI) | CSPN, Common Criteria |
| **Label** | Training programmes or similar | ANSSI | SecNumedu |

Frameworks and versions currently published by ANSSI: **PASSI v2.2, PRIS v3.2, PDIS v2.0, PACS v2.0, SecNumCloud v3.2**.

## 2. Needs / qualification table

| Need (PortNormand) | Qualification required | Justification |
|---|---|---|
| **Security audits of the vital systems (SIIV)**: homologation audit, and audits ordered by ANSSI on the SCADA supervision and PCS | **PASSI**. **Required** (LPM) for controls ordered by ANSSI: the **PASSI LPM** (high level) variant. ANSSI's FAQ lets an OIV perform its own homologation audit with an internal team or a PASSI | LPM controls are run by ANSSI, another State service or a PASSI LPM provider. PASSI covers five scopes: architecture, configuration, source code, intrusion tests, organisational and physical |
| **Continuous detection of incidents on the SIIV** (SCADA, PCS) | **PDIS** provider operating **qualified detection probes**. **Required** (LPM detection rule), unless ANSSI or another State service does it | The LPM detection rule requires qualified probes run by a qualified provider. An OIV may qualify itself as a PDIS provider, which is heavy for a 40-person IT department |
| **Incident response** (ransomware, SCADA intrusion as in Ex.4) | **PRIS**. **Recommended**, no LPM obligation found | The Ex.4 scenario needs forensics, containment and recovery within hours. A PRIS provider on a retainer avoids searching for one during the crisis |
| **Governance, risk analysis, crisis preparation, NIS2 gap analysis** | **PACS** (v2.0, two levels: substantial and high). **Recommended** | PortNormand's 8-person security cell is new. PACS covers architecture advice, security policy and cyber-crisis preparation. The level is the beneficiary's choice unless a text imposes one |
| **Hosting PCS data or backups in the cloud** | **SecNumCloud** (v3.2). **Recommended**, mandatory only in certain public-sector cases (see Uncertainty 1) | Qualified offers resist non-EU laws and meet ANSSI's cloud requirements. Backups kept offline or in a qualified cloud help against ransomware |
| **Remote maintenance of SCADA by vendors and integrators** | **PAMS** (secure administration and maintenance), if the framework is available. **Recommended** | In Ex.4 the suspected entry point is a remote-access account. Third-party maintenance is a typical weak point, so contracts should require qualified providers |
| **Security products on the OT network** (firewalls, data diodes, encryption) | **Certified or qualified products** (CSPN, Common Criteria, ANSSI product qualification). **Recommended**; required where a sectoral text says so | The ANSSI catalogue lists certified and qualified products. Choosing from it gives proven assurance for the terminals |

## 3. How to use qualified providers

1. Pick providers **only from ANSSI's official lists** (cyber.gouv.fr and MesServicesCyber). Only providers that agreed to be public appear, for PDIS.
2. **Check the scope, the level and the validity dates** of each qualification, not just the name.
3. **Match the need to the framework**: one provider can hold several qualifications (for example PASSI and PRIS), but each service is qualified separately.
4. **Put the requirement in the contract**: qualification maintained for the whole duration of the service.

## 4. Uncertainties

1. **SecNumCloud status is disputed.** Several commercial sources say it is mandatory for OIV. We found no single text requiring it for an OIV or a NIS2 entity. One 2026 source reports an order of 12 August 2026 making v3.2 binding for the hosting of sensitive State data. We did not verify it. **If PortNormand is a public body or a State operator, the answer may change.**
2. **PASSI wording.** ANSSI's FAQ (older) allows an internal team for homologation audits, while some commercial sites say an external PASSI is always required. We followed ANSSI. The **Transports sectoral order** must be read to confirm.
3. **"High level" and "PASSI LPM"** appear to describe the same requirement for OIV audits. We treat them as equivalent, to be confirmed.
4. **PRIS and PACS are not mandatory under the LPM** as far as we found. We call them recommended.
5. **PAMS** appears in ANSSI's list of qualifications in progress. We could not confirm the final framework.
6. **The PDIS rule applies to SIIV only.** Which PortNormand systems are SIIV is unknown (see Ex.2).
7. **NIS2** adds no qualification obligation that we know of. The final French text may change this.
8. **We name no provider.** Lists change monthly, and counts differed between sources.

## Sources

- ANSSI, *Référentiels d'exigences pour la qualification*: [cyber.gouv.fr](https://cyber.gouv.fr/offre-de-service/solutions-certifiees-et-qualifiees/comprendre-levaluation-de-securite/qualification-de-produit-et-services/referentiels-qualification/)
- ANSSI, *FAQ Systèmes d'information d'importance vitale*: [cyber.gouv.fr](https://cyber.gouv.fr/faq-systemes-dinformation-dimportance-vitale)
- ANSSI, *Le dispositif SAIV*: [cyber.gouv.fr](https://cyber.gouv.fr/reglementation/cybersecurite-systemes-dinformation/directives-nis-nis2-et-dispositif-saiv/dispositif-saiv/)
- ANSSI, *Solutions en cours de qualification*: [cyber.gouv.fr](https://cyber.gouv.fr/decouvrir-des-solutions-en-cours-de-qualification)
- ANSSI catalogue of certified and qualified products and services: [messervices.cyber.gouv.fr](https://messervices.cyber.gouv.fr/visas/catalogue-produits-services-profils-de-protection-sites-certifies-qualifies-agrees-anssi.pdf)
- SecNumCloud overview: [donneespersonnelles.fr](https://www.donneespersonnelles.fr/secnumcloud-certification)
- PASSI v2.2 levels: [Fidens](https://www.fidens.fr/referentiels-anssi/)
