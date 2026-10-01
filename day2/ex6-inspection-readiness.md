# Exercise 6: Inspection Readiness Plan

**Status:** Draft, awaiting team review
**Format:** One page: control points, estimated readiness level, 3 priority actions
**Last verified:** 2026-10-01

> **Important:** the brief gives no data on PortNormand's real security posture. The readiness levels below are **estimates drawn only from the brief** (OIV since 2015, 40-person IT department, 8-person security cell "recently created", nobody knows whom to contact at ANSSI). They must be validated with PortNormand.

## 1. Control points and estimated readiness

| # | Control point (what ANSSI would check) | Readiness | Basis for the estimate |
|---|---|---|---|
| 1 | **List of vital systems (SIIV)** declared and up to date | Medium | OIV since 2015, so a list likely exists. The recent acquisition may have changed the perimeter |
| 2 | **Representative and 24/7 contact point** designated to ANSSI | Low | The brief says nobody knows whom to contact |
| 3 | **Incident declaration procedure** to CERT-FR, tested | Low | No procedure is mentioned. Ex.4 shows many parallel duties |
| 4 | **Sectoral security rules** (Transports order) applied to the SIIV | Low to medium | Security cell is new. Rules not yet mapped to PortNormand's systems |
| 5 | **Qualified detection** (PDIS provider, qualified probes) running on the SIIV | Unknown | No information in the brief |
| 6 | **Audit reports and homologation decisions**, available for ANSSI | Unknown | No information in the brief |
| 7 | **Third parties** (SCADA vendors, integrators, maintenance) bound by contract to the security rules | Low | Not mentioned. The acquisition adds new third parties |
| 8 | **Cooperation with the inspection**: documentation, system access, named contacts | Low to medium | New security cell, no inspection experience mentioned |
| 9 | **NIS2 readiness**: gap analysis and entity registration | Low | Support letter just received, no analysis done |

**Overall estimate: low to medium.** The regime is known to the institution (OIV since 2015) but the organisation has not yet turned it into clear roles, procedures and evidence.

## 2. Three priority actions

1. **Name an ANSSI representative and a 24/7 incident contact, then write and test the declaration procedure** (use the Ex.4 timeline). Why first: failing to declare an incident is the only LPM breach that can be sanctioned **without a prior formal notice**.
2. **Build the compliance evidence file.** Confirm the SIIV list after the acquisition, map the Transports sectoral rules to each SIIV, and gather proof (homologation decisions, audit reports, detection contract and probe status). Then run a **mock control** with a qualified PASSI provider to find gaps before ANSSI does.
3. **Secure the third parties.** Add contractual security clauses for SCADA vendors, integrators and maintenance providers, and for interconnections with the acquired company. The Ex.4 scenario entered through a remote-access account, which is exactly this weakness.

---

## Supporting notes (outside the one-page plan)

### How an LPM control unfolds

1. **Who:** ANSSI, another State service, or a PASSI LPM provider qualified by ANSSI.
2. **Agreement:** a control agreement is signed between PortNormand and the controller, with a copy to ANSSI.
3. **Access:** PortNormand provides the information needed (technical documentation, even source code if required) and access to the systems.
4. **Report:** the controller writes a report, which may include recommendations.
5. **Right of reply:** PortNormand can submit observations **before** the report goes to ANSSI. ANSSI may then hear the parties within two months.

### What is at stake

| Regime | Breach | Maximum penalty |
|---|---|---|
| **LPM** (Defence Code art. L1332-7) | Not meeting the obligations of art. L1332-6-1 to L1332-6-4 | **EUR 150,000** (individuals), up to **EUR 750,000** (legal entities). A formal notice comes first, **except** for failing to declare incidents (art. L1332-6-2) |
| **NIS2** (future, directive art. 34) | Breach of risk-management or reporting duties | Up to **EUR 10 million or 2% of worldwide turnover**, whichever is higher. For PortNormand, 2% of EUR 340 million is EUR 6.8 million, so the EUR 10 million ceiling is the higher one |

### Uncertainties

1. **Readiness levels are estimates** from the brief only. No real audit data.
2. **The Transports sectoral order was not read.** Control points are drawn from the general LPM texts. The exact rules and their wording come from that order.
3. **Penalty amounts.** The ANSSI FAQ and Légifrance agree on EUR 150,000 and EUR 750,000. One commercial source gave different figures (EUR 75,000 and EUR 45,000); we ignored it.
4. **NIS2 penalties and control powers** depend on the final French law. The directive sets the minimum ceilings only.
5. **No notice period** for an inspection was found in public sources, and we do not know who would control PortNormand (ANSSI directly or a PASSI LPM provider).
6. **Representative clearance.** A 2015 law-firm summary says the representative to ANSSI must hold a defence clearance (art. R2311-7). Not re-verified.

### Sources

- ANSSI, *FAQ Systèmes d'information d'importance vitale*: [cyber.gouv.fr](https://cyber.gouv.fr/reglementation/cybersecurite-systemes-dinformation/directives-nis-nis2-et-dispositif-saiv/dispositif-saiv/faq-systemes-dinformation-dimportance-vitale/)
- Code de la défense, art. L1332-7: [Légifrance](https://www.legifrance.gouv.fr/codes/article_lc/LEGIARTI000028345141/2020-11-23)
- Squire Patton Boggs, *Opérateurs d'importance vitale : publication du décret d'application*: [larevue.squirepattonboggs.com](https://larevue.squirepattonboggs.com/operateurs-d-importance-vitale-publication-du-decret-d-application_a2596.html)
- ANSSI, *Le dispositif SAIV*: [cyber.gouv.fr](https://cyber.gouv.fr/reglementation/cybersecurite-systemes-dinformation/directives-nis-nis2-et-dispositif-saiv/dispositif-saiv/)
- Directive (EU) 2022/2555, art. 34: [EUR-Lex](https://eur-lex.europa.eu)
