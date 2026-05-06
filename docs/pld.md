---
tags:
   - liability
   - general
   - documentation
   - software
---

# EU Product Liability Directive (PLD)

Die überarbeitete EU-Produkthaftungsrichtlinie (Directive (EU) 2024/2853) modernisiert den europäischen Produkthaftungsrahmen grundlegend. Sie ersetzt die alte Richtlinie von 1985 (85/374/EWG) und schließt explizit digitale Produkte und Software ein — ein zentraler Schritt, da Software bisher weitgehend aus der Produkthaftung herausfiel.

## Überblick

* **Segment**: Produkthaftung / Zivilrecht
* **Verabschiedet / Veröffentlicht**: 23. Oktober 2024 (EP), November 2024 (ABl. EU), Directive (EU) 2024/2853
* **Gültig ab**:
  * Mitgliedstaaten haben **25 Monate** ab Inkrafttreten Zeit zur Umsetzung ins nationale Recht (voraussichtlich bis **Dezember 2026**)
* **Gültig für**:
  * Hersteller physischer Produkte, die in der EU in Verkehr gebracht werden
  * Anbieter von **Software** (inkl. eingebetteter Software, Apps, Betriebssystemen, KI-Systemen) — erstmals explizit erfasst
  * Importeure und Händler, wenn der Hersteller außerhalb der EU ansässig ist
  * Anbieter wesentlicher Änderungen an bestehenden Produkten (Updates, die neue Risiken einführen)
* **Nicht gültig für**:
  * Open-Source-Software, die **nicht im Rahmen einer kommerziellen Aktivität** bereitgestellt wird (z.B. reine Community-Projekte ohne Gewinnerzielungsabsicht)
  * Dienstleistungen (bleiben in der Dienstleistungshaftung)
  * Produkte, die vor dem Inkrafttreten in Verkehr gebracht wurden (keine Rückwirkung)
* **Grauzone**:
  * Abgrenzung zwischen kommerziellem und nicht-kommerziellem Open Source — insbesondere bei Unternehmen, die OS-Projekte sponsern oder Dual-Licensing betreiben
  * Haftung bei KI-Systemen, die sich nach dem Inverkehrbringen durch Lernen verändern
  * Verantwortungsverteilung in komplexen Lieferketten (wer haftet bei einem Fehler in einer Drittbibliothek?)
  * Software-as-a-Service (SaaS): ob kontinuierlich erbrachte Software als Produkt oder Dienstleistung gilt



## Zentrale Forderungen

### Software als Produkt (Art. 4)

* Software — einschließlich KI-Systemen, eingebetteter Firmware und SaaS-Produkten — fällt explizit unter den Produktbegriff
* Ein Produkt gilt als **fehlerhaft**, wenn es nicht die berechtigte Sicherheitserwartung bietet — bei Software z.B. durch unzureichende Sicherheitspatches oder bekannte, ungepatchte Schwachstellen

### Erweiterter Schadensbegriff (Art. 5)

* **Datenverlust und Datenbeschädigung** gelten erstmals als ersatzfähiger Schaden (nicht nur physische Personenschäden oder Sachschäden)
* Psychische Schäden können unter bestimmten Bedingungen ebenfalls geltend gemacht werden

### Beweislasterleichterung (Art. 9)

* Geschädigte können von Herstellern die **Offenlegung von Beweismitteln** (Dokumentation, Testergebnisse, SBOM, Logs) verlangen
* Verweigert der Hersteller die Herausgabe relevanter Unterlagen, kann das Gericht die **Fehlerhaftigkeit des Produkts vermuten**
* Bei technischer Komplexität: Gerichte können die Kausalität vermuten, wenn ein Produktfehler wahrscheinlich ist

### Haftungsdauer (Art. 14)

* Haftungsfrist: **10 Jahre** ab Inverkehrbringen (verlängerbar auf **15 Jahre** bei latenten Schäden mit langer Latenzzeit, z.B. durch Gesundheitsschäden)

### Pflichten für Wirtschaftsakteure (Art. 7–8)

* Hersteller müssen technische Unterlagen bereithalten, die belegen, dass ein Produkt zum Zeitpunkt des Inverkehrbringens den Sicherheitserwartungen entsprach
* Bei Software: Dokumentation des Entwicklungsprozesses, Testergebnisse, Release-Notes und Patch-Historie sind zentral



## Lösungsansätze & Hilfestellungen

* Die Europäische Kommission und nationale Behörden werden Leitlinien zur Umsetzung veröffentlichen — insbesondere zur Abgrenzung von Software als Produkt vs. Dienstleistung
* Für Open-Source-Anbieter: Prüfen, ob die eigene Aktivität als kommerziell eingestuft werden könnte (Dual Licensing, Support-Verträge, gesponserte Entwicklung)
* Technische Dokumentation und nachvollziehbare Entwicklungsprozesse sind der wichtigste Schutz gegen Haftungsansprüche — "Secure by Design" zahlt sich direkt aus
* Die PLD hat starke Wechselwirkungen mit dem [CRA](/regmon/cra) (Nachweis sicherer Entwicklung) und dem [EU AI Act](/regmon/aiact) (Hochrisiko-KI-Dokumentation)

### Tools & Werkzeuge

#### Technische Dokumentation & Entwicklungsnachweis (Art. 7–8)

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [Syft](https://github.com/anchore/syft) | Apache-2.0 | Erzeugt SBOMs aus Container-Images und Quellcode — dokumentiert die Softwarezusammensetzung zum Zeitpunkt des Releases | Nachweis der Komponentenverantwortung bei Haftungsansprüchen; zeigt, welche Drittbibliotheken eingesetzt wurden |
| [TrustSource ts-scan](https://trustsource.github.io/ts-scan) | Open Source | SCA-Scanner: analysiert Abhängigkeiten und erzeugt CycloneDX/SPDX-SBOMs; CLI-Integration in CI/CD | SBOM als Dokumentationsartefakt für den Entwicklungsprozess; Grundlage für Offenlegung gegenüber Gerichten |
| [TrustSource CE](https://github.com/trustsource/ts-core-ce) | AGPL (Community Edition) | SBOM-Versionierung und -Management: bewahrt die genaue Komponentenzusammensetzung jeder Release-Version dauerhaft auf | Langfristige Nachvollziehbarkeit der Produktzusammensetzung über die 10-jährige Haftungsfrist |
| [MLflow](https://github.com/mlflow/mlflow) | Apache-2.0 | Experiment-Tracking und Model Registry für ML/KI-Systeme; versioniert Modelle, Datensätze und Trainingsläufe | Bei KI-Produkten: Nachweis des Entwicklungs- und Validierungsprozesses zum Zeitpunkt des Inverkehrbringens |

#### Schwachstellen- & Patch-Management (Fehlerhaftigkeit durch ungepatchte Schwachstellen)

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [Grype](https://github.com/anchore/grype) | Apache-2.0 | Schwachstellenscanner auf SBOM-Basis; erkennt bekannte CVEs in eingesetzten Komponenten | Nachweis, dass zum Release-Zeitpunkt keine bekannten ausnutzbaren Schwachstellen vorlagen |
| [Dependency-Track](https://dependencytrack.org/) | Apache-2.0 | Kontinuierliche SBOM-Analyse-Plattform: überwacht Schwachstellen über den Produktlebenszyklus und dokumentiert Behebungsmaßnahmen | Audit-Trail für Patch-Entscheidungen; zeigt, dass der Hersteller bekannte Schwachstellen aktiv verfolgt hat |
| [DefectDojo](https://github.com/DefectDojo/django-DefectDojo) | BSD-3-Clause | Vulnerability Management mit Remediation-Tracking und SLA-Dokumentation | Nachweisführung für zeitgerechte Fehlerbehebung; wichtig bei Haftungsansprüchen wegen bekannter Schwachstellen |

#### Qualitätssicherung & Testnachweis

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [SonarQube Community](https://github.com/SonarSource/sonarqube) | LGPL-3.0 (Community Edition) | Statische Code-Analyse: erkennt Bugs, Sicherheitslücken und Code-Smells; erzeugt historische Qualitätsberichte | Nachweis einer systematischen Qualitätsprüfung vor dem Inverkehrbringen; belegt Sorgfaltspflicht |
| [OWASP ZAP](https://github.com/zaproxy/zaproxy) | Apache-2.0 | Dynamischer Sicherheitsscanner (DAST) für Web-Applikationen | Nachweis durchgeführter Sicherheitstests; relevant bei Haftungsansprüchen wegen Sicherheitsmängeln |
