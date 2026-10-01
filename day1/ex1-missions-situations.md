# Exercise 1: ANSSI Missions / Situations Table

**Status:** Done
**Format:** Three-column table (situation, ANSSI mission, other possible actor), one row per situation
**Last verified:** 2026-10-01 (ANSSI missions checked on [cyber.gouv.fr/missions](https://cyber.gouv.fr/nous-connaitre/lagence/missions/))

## ANSSI's five missions (official wording)

| Mission | In short |
|---|---|
| **Défendre** (Defend) | Protect critical information systems (detection capabilities, trusted security products) and structure national assistance to victims of cyberattacks |
| **Connaître** (Know) | Maintain knowledge of the state of the art, of threats and risks, and of cybersecurity trends |
| **Partager** (Share) | Provide recommendations, methods and tools; share threat knowledge with national, European and international partners |
| **Accompagner** (Support) | Support public policy, regulated organisations (protection measures and incident response), training, and a trusted provider ecosystem |
| **Réguler** (Regulate) | Qualification and certification of products and services, design of regulatory frameworks, and control of their application |

## Missions / situations table

| Situation (PortNormand) | ANSSI mission | Other possible actor |
|---|---|---|
| Suspicious activity is detected on the SCADA supervision network of an oil terminal | **Défendre** (detection and assistance to victims, via CERT-FR) | PDIS-qualified detection provider; internal security cell |
| Ransomware encrypts the Port Community System and PortNormand needs technical help to respond | **Défendre** (assistance to victims) | PRIS-qualified incident response provider; police or gendarmerie (criminal complaint) |
| The same incident exposes personal data of employees and shipping customers | **Défendre** (technical side of the incident only) | **CNIL** (personal data breach notification) |
| The team wants to understand who is behind the attack and which techniques are used | **Connaître** and **Partager** (threat knowledge, CERT-FR publications) | Law-enforcement and intelligence services (attribution); sector information-sharing communities |
| The IT team needs practical guidance to secure its industrial control systems | **Partager** (recommendations, methods and guides) | Equipment vendors; integrators |
| PortNormand must choose an auditor for the security audit of its information systems | **Réguler** (qualification of audit providers, PASSI) | The PASSI-qualified provider itself (selected from the ANSSI directory) |
| PortNormand wants to host Port Community System data with a cloud provider | **Réguler** (SecNumCloud qualification) | The cloud provider; PortNormand's legal and procurement teams |
| The terminal network needs a security product (firewall, encryption) with proven assurance | **Réguler** (product certification and qualification) | CESTI evaluation labs; the product vendor |
| PortNormand wants to know which regulation applies to it (LPM as OIV, NIS2 as a new framework) | **Accompagner** (regulated organisations) and **Réguler** (regulatory frameworks) | SGDSN; Ministry in charge of Transports (sector coordination) |
| ANSSI wants to verify that PortNormand actually applies the required security measures | **Réguler** (control of application) | Qualified auditors acting under ANSSI's control; sector ministry (to confirm in Ex.6) |
| The 8-person security cell needs training | **Accompagner** (skills development, training) | Training providers and schools; Campus Cyber ecosystem |
| A subsidiary of the acquired logistics company in another EU member state suffers an incident | **Partager** (cooperation with European partners) | National authority or CSIRT of that member state; EU CSIRTs network; ENISA (support role) |
| A cyber crisis threatens the continuity of port operations at national level | **Défendre** (coordination of the response) | SGDSN; Ministry in charge of Transports; local prefecture |
| Management asks to "hack back" the attackers | **None.** Outside ANSSI's mandate: the French model separates defensive and offensive missions | Ministry of the Armed Forces (cyber command). A private company must not retaliate on its own |

## Notes and uncertainties

1. **Mission classification is a judgement call.** Several situations touch two missions (rows 4 and 9). We kept the most direct one first.
2. **The "other actor" column is indicative.** Exact roles (SGDSN, sector ministry, CERT-FR contact points for an OIV) are detailed in Ex.3.
3. **Control of OIV obligations (row 10)** may involve ANSSI directly or auditors it designates. This is verified in Ex.6.
4. **NIS2 designation of ANSSI as competent authority** and its entry into force in French law are checked in Ex.2. We make no claim on them here.
5. ANSSI is a service of the Prime Minister placed under the SGDSN, created by decree no. 2009-834 of 7 July 2009 ([source](https://cyber.gouv.fr/nous-connaitre/lagence/histoire-et-modele/)).

## Source

- ANSSI, *Missions*, cyber.gouv.fr (content under Etalab 2.0 licence, paraphrased here).
