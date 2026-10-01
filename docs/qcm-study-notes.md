# QCM Study Notes

Preparation for the individual 15-question quiz at the end of Day 2. Everything here comes from facts verified in Ex.1 to Ex.6 (dated 2026-10-01).

## 1. Traps to remember

- **Three different 72-hour clocks:** CNIL (GDPR), criminal complaint (insurance), NIS2 incident notification. Different recipients, different purposes.
- **LPM applies now, NIS2 does not yet** (in France, as of 2026-10-01). PortNormand will end up under both.
- **CERT-FR is the OIV's entry point**, not Cybermalveillance.gouv.fr and not a regional CSIRT.
- **"Without delay" is not "24 hours".** 24 hours is the future NIS2 early warning.
- **Qualification, certification, label are different things** (services and products / evaluated products / training).
- **Failing to declare an incident is the exception to the formal-notice rule** (art. L1332-7): other breaches of art. L1332-6-1 to L1332-6-4 get a formal notice first.
- **ANSSI does not run offensive operations.** A company must not hack back.
- **Qualified detection (PDIS + probes) applies to the SIIV**, not necessarily to the whole information system.
- **ANSSI vs CNIL:** an incident with personal data triggers both, each for its own reason.

## 2. Practice questions

**1. Which of these is NOT one of ANSSI's five missions?**

- A. Attaquer (offensive operations)
- B. Défendre
- C. Partager
- D. Accompagner

**2. Where does an OIV declare an incident affecting a vital information system (SIIV)?**

- A. The local prefecture
- B. CERT-FR (ANSSI)
- C. CNIL
- D. Cybermalveillance.gouv.fr

**3. What is the LPM deadline to declare an incident to CERT-FR?**

- A. 72 hours
- B. One month
- C. Without delay (no fixed number of hours)
- D. 24 hours

**4. Within what time must a personal data breach be notified to the CNIL (GDPR art. 33)?**

- A. 24 hours
- B. 7 days
- C. One month
- D. 72 hours from awareness

**5. Which rule conditions cyber insurance compensation (Insurance Code art. L12-10-1)?**

- A. A criminal complaint within 72 hours of awareness
- B. A CNIL notification within 24 hours
- C. A CERT-FR declaration within one week
- D. No condition exists

**6. What is the NIS2 article 23 reporting sequence?**

- A. Early warning 48 h, notification one week
- B. Early warning 24 h, notification 72 h, final report one month after the notification
- C. Notification 72 h, report 7 days, final report 3 months
- D. Early warning 1 h, notification 24 h, report 72 h

**7. What was the status of NIS2 in France on 1 October 2026?**

- A. Repealed and replaced by the LPM
- B. Applicable to OIV only
- C. Transposition bill not yet promulgated; the Commission referred France to the CJEU in July 2026
- D. Fully applicable since 2024

**8. What NIS2 category is PortNormand expected to fall into?**

- A. Important entity
- B. Out of scope
- C. Digital infrastructure provider
- D. Essential entity

**9. Which qualified provider type operates detection on a SIIV with qualified probes?**

- A. PDIS
- B. PASSI
- C. PRIS
- D. PACS

**10. What does a PRIS provider do?**

- A. Cloud hosting
- B. Incident response (forensics, containment, recovery)
- C. Security audits
- D. Continuous detection

**11. What is a PASSI LPM provider qualified to do?**

- A. Host data in the cloud
- B. Label training programmes
- C. Audit and control the vital systems of OIV
- D. Certify products

**12. Which LPM breach can be sanctioned WITHOUT a prior formal notice?**

- A. Not maintaining protection measures
- B. Late audit
- C. Missing documentation
- D. Failing to declare an incident (art. L1332-6-2)

**13. What is the maximum fine for a legal entity under Defence Code art. L1332-7?**

- A. EUR 750,000
- B. EUR 45,000
- C. EUR 75,000
- D. EUR 150,000

**14. Who is Cybermalveillance.gouv.fr designed for?**

- A. Foreign CSIRTs
- B. Individuals, small organisations and local authorities
- C. Operators of vital importance only
- D. State ministries only

**15. What is SecNumCloud?**

- A. A training label
- B. An audit qualification
- C. An ANSSI qualification for cloud service providers (framework v3.2)
- D. A product certification for firewalls

<details>
<summary>Answer key (try the questions first)</summary>

1. **A**. The five missions are Défendre, Connaître, Partager, Accompagner and Réguler. The French model separates defence from offence, so offensive operations are outside ANSSI's mandate.
2. **B**. Defence Code art. L1332-6-2: the OIV notifies CERT-FR through the ANSSI form.
3. **C**. The law says 'sans délai'. The 1-hour target in Ex.4 is our own internal assumption.
4. **D**. 72 hours, and the notification can be completed later if information is missing.
5. **A**. The complaint must be a full complaint; a pre-complaint is not enough. This 72 h clock is separate from the CNIL one.
6. **B**. 24 hours, 72 hours, then one month after the incident notification.
7. **C**. As verified in Ex.2. Re-check before relying on it, the situation can change.
8. **D**. Port managing bodies are in Annex I (water transport), 1,200 staff exceeds the large-entity ceiling, and OIV are treated as essential.
9. **A**. The LPM detection rule requires qualified probes run by a qualified PDIS provider (unless ANSSI or the State does it).
10. **B**. PRIS = Prestataire de réponse aux incidents de sécurité. Recommended, but we found no LPM obligation.
11. **C**. ANSSI's SAIV page says controls are run by ANSSI, another State service, or a PASSI LPM provider.
12. **D**. Art. L1332-7: the penalty for breaching L1332-6-1 to L1332-6-4 is preceded by a formal notice, except for the incident declaration duty.
13. **A**. EUR 150,000 for individuals, up to EUR 750,000 for legal entities (ANSSI FAQ and Légifrance agree).
14. **B**. It is not the entry point for an OIV like PortNormand: that is CERT-FR.
15. **C**. Recommended for sensitive hosting. Whether it is mandatory for PortNormand depends on its legal status (see Ex.5 uncertainties).

</details>

## 3. Review checklist

- [ ] ANSSI's five missions and what each covers (Ex.1)
- [ ] OIV status today vs NIS2 essential entity tomorrow (Ex.2)
- [ ] Who does what: ANSSI, CERT-FR, SGDSN, CNIL, police, CSIRTs (Ex.3)
- [ ] Notification deadlines and recipients, and the 12-step timeline (Ex.4)
- [ ] PASSI, PDIS, PRIS, PACS, SecNumCloud: purpose of each and which are mandatory (Ex.5)
- [ ] How an LPM control unfolds and the penalties (Ex.6)
