---
tags:
   - data
   - cloud
   - iot
   - general
   - reporting
---

# EU Data Act

Der EU Data Act schafft einen harmonisierten Rahmen für den Zugang zu und die Nutzung von Daten, die durch vernetzte Produkte (IoT) und damit verbundene Dienste erzeugt werden. Er soll sicherstellen, dass Nutzende — sowohl Verbraucher als auch Unternehmen — die Kontrolle über ihre Daten zurückgewinnen und Daten fairer im Markt zirkulieren können.

## Überblick

* **Segment**: Datenwirtschaft, IoT, Cloud- und Datenverarbeitungsdienste
* **Verabschiedet / Veröffentlicht**: 27. November 2023 (ABl. EU), in Kraft seit 11. Januar 2024
* **Gültig ab**:
  * **12. September 2025**: Vollständige Anwendung für neue Produkte und Dienste
  * Für bereits vor dem 12. September 2025 in Verkehr gebrachte vernetzte Produkte gelten Übergangsfristen
* **Gültig für**:
  * Hersteller vernetzter Produkte (IoT-Geräte, Maschinen, Fahrzeuge, Haushaltsgeräte, etc.) und Anbieter damit verbundener Dienste, die in der EU verkauft oder genutzt werden
  * Anbieter von Datenverarbeitungsdiensten (Cloud, Edge)
  * Unternehmen, die auf Grundlage von Datennutzungsvereinbarungen Daten erhalten
  * Öffentliche Stellen der Mitgliedstaaten (unter bestimmten Bedingungen)
* **Nicht gültig für**:
  * Reine Software-Produkte ohne physische Komponente (außer wenn als „verbundener Dienst" eingestuft)
  * Daten, die bereits durch den EU Data Governance Act oder die DSGVO abgedeckt sind (Abgrenzung beachten)
  * Kleinstunternehmen bei bestimmten Pflichten (Art. 7 — Ausnahme für KMU)
* **Grauzone**:
  * Abgrenzung „vernetztes Produkt" vs. reine SaaS-Lösung
  * Umgang mit gemischten Datensätzen (personenbezogen + nicht-personenbezogen)
  * Verhältnis zu bestehenden Verträgen und Geschäftsgeheimnissen



## Zentrale Forderungen

### Datenzugang für Nutzer (Art. 3–6)

* Hersteller vernetzter Produkte müssen sicherstellen, dass vom Produkt erzeugte Daten für den Nutzer **leicht zugänglich** sind — direkt am Gerät oder über einen Online-Dienst, s. Art. 3–4
* Daten müssen **kostenfrei, in Echtzeit und kontinuierlich** bereitgestellt werden können
* Nutzer können die Daten an **Dritte ihrer Wahl** weitergeben (Portabilität), s. Art. 5

### Datenweitergabe an Dritte (Art. 5–12)

* Nutzer können von Herstellern verlangen, Daten an einen Dritten (z.B. Reparaturbetrieb, App-Anbieter) weiterzugeben
* Die Bedingungen für die Weitergabe müssen **fair, zumutbar und nicht diskriminierend** sein (FRAND-Prinzip), s. Art. 8
* Unfaire Vertragsbedingungen gegenüber KMU bei der Datenweitergabe sind unwirksam, s. Art. 13

### Datenzugang für öffentliche Stellen (Art. 14–22)

* In Ausnahmesituationen (öffentlicher Notstand, Naturkatastrophen) können Behörden Unternehmen zur Bereitstellung von Daten verpflichten
* Der Datenaustausch erfolgt auf Anfrage, ist zweckgebunden und zeitlich begrenzt

### Wechsel zwischen Datenverarbeitungsdiensten / Cloud Switching (Art. 23–31)

* Anbieter von Cloud- und Edge-Diensten müssen den Wechsel zu einem anderen Anbieter aktiv ermöglichen
* **Switching-Fristen**: Wechselprozess muss innerhalb von 30 Arbeitstagen abgeschlossen sein (ab 2027 auf 7 Tage reduziert)
* **Switching-Entgelte**: Übergangsweise erlaubt, aber bis September 2027 vollständig abzubauen; ab dann kostenloser Wechsel
* Technische und vertragliche Hindernisse beim Wechsel sind zu beseitigen (Lock-in-Verbot)
* Offene Interoperabilitätsspezifikationen und Standards müssen unterstützt werden, s. Art. 28–31

### Schutz von Geschäftsgeheimnissen (Art. 4, 8, 9)

* Berechtigte Geschäftsgeheimnisse können als Grund geltend gemacht werden, bestimmte Daten nicht offenzulegen — jedoch nur unter engen Voraussetzungen und mit entsprechender Begründung

### Interoperabilität (Art. 28–37)

* Datenverarbeitungsdienste müssen Mindestanforderungen an Interoperabilität erfüllen
* Europäische Standardisierungsorganisationen (CEN, CENELEC, ETSI) werden beauftragt, harmonisierte Standards zu entwickeln



## Lösungsansätze & Hilfestellungen

* **Datenstrategie überprüfen**: Welche Daten erzeugt das eigene Produkt? Wer hat laut Data Act Zugriffsrechte? Bereits bei Produktdesign berücksichtigen (Data by Design)
* **Vertragswerke anpassen**: Bestehende Datennutzungsverträge mit B2B-Partnern auf FRAND-Konformität und Klauselverbote (Art. 13) prüfen
* **Cloud-Anbieter evaluieren**: Erfüllen aktuelle Cloud-Verträge die Switching-Anforderungen? Gibt es Lock-in-Risiken?
* Die **Europäische Kommission** und nationale Behörden (DE: zuständig sind die Wettbewerbsbehörden und sektorspezifische Stellen) veröffentlichen laufend Leitlinien
* Für IoT-Hersteller: Technische Schnittstellen (APIs) zur Datenbereitstellung frühzeitig einplanen

### Tools & Werkzeuge

#### IoT-Datenzugang & Digital Twins (Art. 3–5)

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [Eclipse Ditto](https://github.com/eclipse-ditto/ditto) | Eclipse PL 2.0 | Digital-Twin-Framework für IoT-Geräte: verwaltet Gerätezustand und stellt standardisierte REST/WebSocket-APIs bereit | Art. 4–5: IoT-Produkte müssen Datenzugang für Nutzer ermöglichen — Ditto liefert die API-Schicht |
| [ThingsBoard](https://github.com/thingsboard/thingsboard) | Apache-2.0 (CE) | IoT-Plattform mit Geräteverwaltung, Datenerfassung, Dashboards und Rule Engine | Art. 4: Gibt Herstellern eine Plattform, um den gesetzlich geforderten Nutzer-Datenzugang umzusetzen |
| [FIWARE Orion Context Broker](https://github.com/telefonicaid/fiware-orion) | AGPL-3.0 | NGSI-LD Kontextdaten-Management für IoT und Smart City; weit verbreitet in EU-Behörden-Deployments | Art. 2(15) IoT-Daten; Kern vieler EU-Datenräume (GAIA-X, Smart Cities) |

#### Daten-Katalog & Lineage (Art. 4, 5)

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [DataHub](https://github.com/datahub-project/datahub) | Apache-2.0 | Moderne Metadata-Plattform: Datenerkennung, Lineage, Ownership und Qualität | Art. 4: Auffindbarkeit und Dokumentation von Datensätzen; Art. 5: Audit-Trail, wer wann Zugang hatte |
| [OpenMetadata](https://github.com/open-metadata/OpenMetadata) | Apache-2.0 | End-to-End Metadaten-Management mit Lineage, Qualitäts-Checks und 50+ Konnektoren | Art. 4: API-first Design; Lineage dokumentiert Datenherkunft und -transformationen |
| [Apache Atlas](https://atlas.apache.org/) | Apache-2.0 | Metadaten-Management und Lineage-Tracking für Enterprise Data Ecosystems | Art. 4: Daten-Governance und -Lineage; Art. 5: Nachvollziehbarkeit von Datenzugriffen |

#### Cloud-Wechsel & Daten-Portabilität (Art. 23–31)

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [GAIA-X / XFSC](https://gitlab.com/gaia-x/data-infrastructure-federation-services) | Apache-2.0 | Offenes Toolset für föderierte Cloud-Infrastruktur, Trust-Frameworks und Interoperabilität | Art. 23–35: Direkte Adressierung der Cloud-Switching-Anforderungen; GAIA-X als EU-Datenraum-Backbone |
| [Rclone](https://github.com/rclone/rclone) | MIT | CLI-Tool zur Datensynchronisierung und -migration zwischen 70+ Cloud-Storage-Anbietern | Art. 23: Praktisches Werkzeug zur Umsetzung des Cloud-Wechsels; unterstützt alle gängigen Anbieter |
| [Airbyte](https://github.com/airbytehq/airbyte) | MIT (core) | Datenintegration und strukturierter Datenexport zwischen 300+ Quellen und Zielen | Art. 5: Dritte-Weitergabe-Anforderungen umsetzen; strukturierter Datenexport bei Anbieterwechsel |
| [Velero](https://github.com/vmware-tanzu/velero) | Apache-2.0 | Kubernetes Backup und Migration zwischen Clustern/Cloud-Anbietern | Art. 23: Workload-Portabilität für Cloud-native Anwendungen ohne Datenverlust |

#### API-Design & Datenbereitstellung (Art. 4, 28–31)

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [OpenAPI / Swagger](https://github.com/OAI/OpenAPI-Specification) | Apache-2.0 | Standard für REST-API-Design, Dokumentation und Validierung | Art. 4–5: Maschinenlesbare, interoperable Datenzugangs-APIs für B2B/B2G-Datenweitergabe |
| [Backstage](https://github.com/backstage/backstage) | Apache-2.0 | Entwicklerportal mit API-Katalog und Service-Registry | Art. 4: „Data Access Portal"-Pattern für auffindbare, dokumentierte Datenzugangs-APIs |
