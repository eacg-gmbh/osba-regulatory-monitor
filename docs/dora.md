---
tags:
   - cybersecurity
   - financial services
   - insurance
---

# Digital Operational Resilience Act (DORA)

Das Gesetz über die digitale operative Widerstandsfähigkeit (Digital Operational Resilience Act, DORA) ist ein umfassender Rechtsrahmen, der von der Europäischen Union (EU) eingeführt wurde, um die operative Widerstandsfähigkeit von Finanzinstituten und kritischen Drittanbietern zu verbessern. DORA soll sicherstellen, dass Finanzinstitute und ihre Dienstleister allen Arten von Störungen und Bedrohungen im Zusammenhang mit der Informations- und Kommunikationstechnologie (IKT) standhalten, darauf reagieren und sich davon erholen können.

## Überblick

* **Segment**: IT Sicherheit / Financial Services

* **Verabschiedet / Veröffentlicht**: 

* **Gültig ab**:
  * 17.01.2025
  
* **Gültig für**:
  
  DORA gilt für eine Vielzahl von Finanzunternehmen (20 Ttypen), darunter Banken, Wertpapierfirmen, Versicherungsgesellschaften und wichtige Drittanbieter, die Finanzdienstleistungen unterstützen. Es umfasst IKT-bezogene Vorfälle, die die Finanzstabilität und die Kontinuität der Dienstleistungen beeinträchtigen könnten.
  
* **Nicht gültig für**:
  * Nicht-Finanzunternehmen, es sei denn, sie erbringen Dienste für diese.
  
* **Grauzone**:
  * k.A.
  
* **Ziel**:
  Die Verordnung betont die Bedeutung der operativen Widerstandsfähigkeit und verpflichtet Finanzinstitute zur Einführung robuster Rahmenwerke für das IKT-Risikomanagement. Dazu gehören die Identifizierung, Bewertung und Minderung von IKT-Risiken, um die Kontinuität kritischer Betriebsabläufe sicherzustellen.



## Zentrale Forderungen

Finanzinstitute müssen umfassende Rahmenwerke für das IKT-Risikomanagement einrichten, die Richtlinien, Verfahren und Kontrollen zur Bewältigung von IKT-Risiken umfassen. Dazu gehören regelmäßige Risikobewertungen, die Planung von Maßnahmen zur Reaktion auf Vorfälle und das Business Continuity Management.

* **Risikomanagement bei Dritten**:

  DORA legt großen Wert auf das Management von Risiken, die mit Drittanbietern verbunden sind. Finanzinstitute müssen Due-Diligence-Prüfungen bei Drittanbietern durchführen, deren Leistung überwachen und sicherstellen, dass sie die selben Resilienzstandards einhalten.

* **Meldung von Vorfällen**:

  Die Verordnung schreibt die Meldung schwerwiegender IKT-Vorfälle an die zuständigen Behörden vor. Finanzinstitute müssen über Mechanismen zur Erkennung, Meldung und Bewältigung von IKT-Vorfällen verfügen, um Transparenz und Rechenschaftspflicht zu gewährleisten.

* **Tests der digitalen Betriebsresilienz**:

  DORA verpflichtet Finanzinstitute, ihre IKT-Systeme und -Prozesse regelmäßig zu testen, um sicherzustellen, dass sie Störungen standhalten und sich davon erholen können. Dazu gehören Penetrationstests, Schwachstellenanalysen und Resilienztests.

* **Governance und Rechenschaftspflicht**:

  Die Verordnung betont die Bedeutung von Governance und Rechenschaftspflicht beim Management von IKT-Risiken. Finanzunternehmen müssen klare Rollen und Verantwortlichkeiten für das IKT-Risikomanagement festlegen, wobei die Geschäftsleitung und der Verwaltungsrat eine wichtige Rolle bei der Überwachung der Resilienzmaßnahmen spielen.

* **Aufsicht und Durchsetzung**:

  Die DORA führt Aufsichts- und Durchsetzungsmechanismen ein, um die Einhaltung der Verordnung sicherzustellen. Die Aufsichtsbehörden sind befugt, Inspektionen durchzuführen, Sanktionen zu verhängen und Durchsetzungsmaßnahmen gegen nicht konforme Unternehmen zu ergreifen.



## Lösungsansätze & Hilfestellungen

* EBA, ESMA und EIOPA haben gemeinsame Regulatory Technical Standards (RTS) zu DORA veröffentlicht, die konkrete technische Anforderungen spezifizieren: [ESAs DORA RTS](https://www.eba.europa.eu/regulation-and-policy/digital-operational-resilience-act-dora)
* ENISA bietet Orientierungshilfen für ICT-Risikomanagement im Finanzsektor

### Tools & Werkzeuge

#### ICT-Risikomanagement & GRC

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [Eramba](https://www.eramba.org/) | Open Source (AGPL, Community Edition) | GRC-Plattform: Risikoregister, Controls, Policy-Management, Audit-Trails | DORA Art. 5–14: ICT-Risikomanagement-Rahmenwerk |
| [OpenRMF](https://github.com/Cingulara/openrmf-oss) | Open Source (GPL-3.0) | RMF-Dokumentation, STIG-Checklisten, Control-Tracking | ICT-Risikodokumentation |

#### Drittparteien-ICT-Risiko & Vendor Management

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [simple-tprm](https://github.com/ossf/wg-best-practices-os-developers) | Open Source | Fragebögen und Templates für Third-Party Risk Assessments nach OpenSSF Best Practices | DORA Art. 28–44: Due-Diligence bei ICT-Drittanbietern |

#### Incident Management & Reporting

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [TheHive](https://thehive-project.org/) | Open Source (AGPL) | Security Incident Response; strukturiertes Case Management und Dokumentation | DORA Art. 17–23: ICT-Incident Management und Meldepflichten |
| [Deming](https://github.com/dbarzin/deming) | Open Source (GPL) | Web-basiertes IT-Sicherheits-Audit-Management nach ISO 27001; Maßnahmen-Tracking und Audit-Dokumentation | DORA Art. 17–19: Nachweisführung zu ICT-Incident-Management-Prozessen |

#### Resilience Testing

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [Chaos Monkey / Chaos Engineering Tools](https://netflix.github.io/chaosmonkey/) | Open Source (Apache-2.0) | Resilience Testing durch gezieltes Einbringen von Fehlern in Produktivsysteme | DORA Art. 24–27: Testen der digitalen Betriebsresilienz |
