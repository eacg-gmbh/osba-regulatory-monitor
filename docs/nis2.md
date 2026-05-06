---
tags:
   - cybersecurity
   - saas
   - kritis
---

# EU Network & Infratsructure Directive v2 (NIS2)

Der EU NIS2 ist ein Meilenstein für die IT-Sicherheit in Europa. Die neue, zweite Richtlinie über Netz- und Informationssysteme (NIS2) ist ein umfassender Rechtsrahmen, der von der Europäischen Union (EU) eingeführt wurde, um die Cybersicherheit und die Betriebsstabilität kritischer Infrastrukturen und digitaler Diensteanbieter zu verbessern. NIS2 baut auf der ursprünglichen Richtlinie über Netz- und Informationssysteme (NIS) auf und erweitert deren Anwendungsbereich auf eine größere Bandbreite von Sektoren und Einrichtungen, um der sich wandelnden digitalen Landschaft und den zunehmenden Cyberbedrohungen Rechnung zu tragen.

## Überblick

* **Segment**: IT Sicherheit für Anbieter digitaler Dienste
* **Verabschiedet / Veröffentlicht**: 14. / 27. Dezember 2022
* **Gültig ab**:
  * Jeweilige Implementierung in der Landesgesetzgebung. Eigentlich hätte die NIS2 im Januar 2025 in Deutschland umegsezt werden sollen, jedoch hat der Abgang der Ampel-Koalition das Vorhaben nicht mehr durchgebracht. Der Gesetzesentwurf liegt vor, eine neue Terminierung zur Verabschiedung ist jedoch noch nicht bekannt. 
* **Gültig für**:
  * Internet-Dienstleister und Service-Anbieter
  * KRITIS-Unternehmen
* **Nicht gültig für**:
  * Produkt-Anbieter
* **Grauzone**:
  * k.A.



## Zentrale Forderungen

* **Verbessertes Risikomanagement**:

  Die Richtlinie verpflichtet Unternehmen zur Implementierung robuster Risikomanagementpraktiken zur Identifizierung, Bewertung und Minderung von Cybersicherheitsrisiken. Dazu gehören die Entwicklung von Notfallplänen, die Durchführung regelmäßiger Risikobewertungen und die Gewährleistung der Geschäftskontinuität.

* **Meldung von Vorfällen**:

  NIS2 verpflichtet Unternehmen, schwerwiegende Cybersicherheitsvorfälle innerhalb strenger Fristen an die nationalen Behörden zu melden. Dies gewährleistet die rechtzeitige Erkennung, Reaktion und Abwehr von Cyberbedrohungen und erhöht die allgemeine Cybersicherheitsresilienz.

* **Sicherheit der Lieferkette**:

  Die Richtlinie betont die Bedeutung der Sicherheit der Lieferkette und verpflichtet Unternehmen, die mit ihren Lieferanten und Dienstleistern verbundenen Risiken zu bewerten und zu managen. Dazu gehören die Durchführung von Due-Diligence-Prüfungen und die Sicherstellung, dass Drittanbieter die gleichen Sicherheitsstandards einhalten.

* **Governance und Rechenschaftspflicht**:

  NIS2 legt großen Wert auf Governance und Rechenschaftspflicht und verpflichtet Unternehmen, klare Rollen und Verantwortlichkeiten für das Cybersicherheitsmanagement festzulegen. Die Geschäftsleitung und der Vorstand sind für die Umsetzung wirksamer Cybersicherheitsmaßnahmen verantwortlich.

* **Aufsicht und Durchsetzung**:

  Die Richtlinie führt Aufsichts- und Durchsetzungsmechanismen ein, um die Einhaltung der Vorschriften zu gewährleisten. Die nationalen Behörden sind befugt, Inspektionen durchzuführen, Sanktionen zu verhängen und Durchsetzungsmaßnahmen gegen nicht konforme Unternehmen zu ergreifen.

* **Informationsaustausch und Zusammenarbeit**:

  NIS2 fördert den Informationsaustausch und die Zusammenarbeit zwischen Unternehmen sowie zwischen Unternehmen und Behörden. Dazu gehört die Einrichtung von Mechanismen für den Austausch von Bedrohungsinformationen, bewährten Verfahren und Vorfallmeldungen, um die kollektive Cybersicherheitsresilienz zu verbessern.

* **Kritische und wichtige Unternehmen**:

  NIS2 klassifiziert Unternehmen anhand ihrer Rolle und ihrer Auswirkungen auf die Gesellschaft in „kritische“ und „wichtige“ Kategorien. Kritische Unternehmen unterliegen strengeren Anforderungen und einer strengeren Aufsicht als wichtige Unternehmen.



## Lösungsansätze & Hilfestellungen

* Ein guter Leitfaden für die Analyse zur Implementierung findet sich beim BSI: [BSI NIS2-Umsetzung](https://www.bsi.bund.de/DE/Themen/Unternehmen-und-Organisationen/Standards-und-Zertifizierung/IT-Grundschutz/IT-Grundschutz-Kompendium/it-grundschutz-kompendium_node.html)
* ENISA bietet Leitfäden und Mapping-Tabellen für NIS2-Anforderungen: [ENISA NIS2](https://www.enisa.europa.eu/topics/cybersecurity-policy/nis-directive-new)

### Tools & Werkzeuge

#### GRC & Risikomanagement

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [MONARC](https://github.com/monarc-project/MonarcAppFO) | Open Source (AGPL) | Strukturierte Risikoanalyse nach ISO 27005; entwickelt von CASES Luxemburg | NIS2 Art. 21: Risikomanagementmaßnahmen |
| [Eramba](https://www.eramba.org/) | Open Source Community / Kommerziell | GRC-Plattform: Risikoregister, Controls, Compliance-Mapping | NIS2 Art. 20–21, ISO 27001 |
| [OpenRMF](https://github.com/Cingulara/openrmf-oss) | Open Source (GPL-3.0) | RMF-Dokumentation, STIG-Checklisten, Compliance-Tracking | IT-Risikomanagement |
| [Vanta](https://www.vanta.com/) | Kommerziell (SaaS) | Automatisiertes Compliance-Monitoring für ISO 27001, NIS2, SOC 2 | NIS2, ISO 27001 |

#### Incident Management & Threat Intelligence

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [TheHive](https://thehive-project.org/) | Open Source (AGPL) | Security Incident Response Plattform; strukturierte Vorfallbearbeitung und Reporting | NIS2 Art. 23: Meldepflicht schwerwiegender Vorfälle |
| [MISP](https://www.misp-project.org/) | Open Source (AGPL) | Threat Intelligence Sharing; Austausch von IoCs zwischen Organisationen und Behörden | NIS2 Art. 29: Informationsaustausch |
| [Cortex](https://github.com/TheHive-Project/Cortex) | Open Source (AGPL) | Automatisierte Analyse von Observables; ergänzt TheHive | Unterstützt Incident-Response-Prozesse |
| [Deming](https://github.com/dbarzin/deming) | Open Source (GPL) | Web-basiertes IT-Sicherheits-Audit-Management nach ISO 27001; Maßnahmen-Tracking, Reifegradmessung und Compliance-Nachweise | NIS2 Art. 21: Risikomanagement-Maßnahmen dokumentieren und nachweisen |

#### Monitoring & Schwachstellenmanagement

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [Wazuh](https://wazuh.com/) | Open Source (GPL) | SIEM, Intrusion Detection, Log-Analyse, Schwachstellenerkennung | NIS2 Art. 21: Sicherheit von Netz- und Informationssystemen |
| [OpenVAS / Greenbone](https://www.greenbone.net/) | Open Source (GPL) | Schwachstellenscanner für Netzwerke und Systeme | NIS2: Schwachstellenmanagement |
| [Zabbix](https://www.zabbix.com/) | Open Source (GPL-2.0) | Infrastruktur-Monitoring und Alerting | Betriebsstabilität, Frühwarnung |
