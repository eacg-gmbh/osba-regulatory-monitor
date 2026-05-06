---
tags:
 - cybersecurity
 - general
 - reporting
 - documentation
 - risk management
 - processes
---

# EU Cyber Resilience Act (CRA)

Der EU Cyber Resilience Act (CRA) ist ein Meilenstein für die IT-Sicherheit in Europa. 

## Überblick

* **Segment**: IT Sicherheit
* **Verabschiedet / Veröffentlicht**: 30.10.2024 angenommen, bzw. 20.11.2024 publiziert
* **Gültig ab**:
    - Berichtswesen an zentrale Stellen: **11. September 2026**
    - Durchführung der Schwachstellenbehebung: **11. Dezember 2027** 

**Gültig für**:

* Alle, die netzwerkfähige Produkte mit digitalen Elementen herstellen oder innerhalb der EU vertreiben (Gewinnerzielungsabsicht) und in der folgenden Liste nicht aufgeführt werden.

**Nicht gültig für**:

* Lösungen in den Branchen Schiffahrt, Automobil und Luftfahrt (s. ...! )
* Medizintechnik (vergleichbare Anfordeurngen s. [MDR](/regmon/mdr.md) !)
* Anbieter von Cloud-Diensten (vergleichbare Anforderungen s. [NIS2](/regmon/nis2))
* Anbieter nicht-gewerblicher Open Source Software, (ACHTUNG! Definition *OS Steward* beachten!) 
* Individual-Entwicklungen 

**Grauzone**:

* Dual-Use-Güter, bspw. nutzbar für Schiffahrt und Haushalte (Annahme: Gültigkeit!)
* Logistik-Lösungen 
* SaaS-Lösungen, die IoT-Anteile haben (Annahme: SaaS => NIS2, IoT-Devices => CRA)

**Neuerungen / Anforderungen**:

* Anforderung ein aktives Risiko-Management einzuführen
* Zusätzliche Prozesse und Verantwortlichkeiten (Produktsicherheit, Vulnerability Disclosure, etc.)
* Neue Anforderungen an Produkt-Updates (freie Sicherheits-Patches für 10 Jahre)
* Konformitätserklärung und CE-Kennzeichen abgeben



## Zentrale Forderungen

* Bereitstellen eines Software Bill of Materials (SBOM), s. Annex I

* Regelmäßige Risikobetrachtungen von Sicherheitsbedrohungen sowie deren Dokumentation, s. Art. 13, III und IV

* Bereitstellen einer Konformitätserklärung, s. Art 13 XII, resp. Art. 28 I und Annex IV

* Bereitstellen des CE-Kennzeichens, s. Art. 12 XII, bzw. Art 30 I

* Defnieren einer Support-Dauer während derer der Anbieter Sicherheits-Updates bereitstellt (min 5 Jahre, bzw. erwartete Nutzungsdauer), s. Art. 13 VIII, S2 ff.

* Kostenfreie Sicherheits-Updates während dieser Periode, welche wiederum 10 Jahre verfügbar gehalten werden müssen, s. Art 13 IX

* Bereitstellen einer technischen Dokumentation, die folgendes beinhaltet (s. Art. 13 III & Annex VII) :

    * Beschreibung des regulären Gebrauchs sowie Fälle der fehlerhaften Nutzung und deren Einfluss auf die Risikobewertung
    * Die Unterstützungsdauer, bzw. einen End-of-life-Termin, ab dem keine Updates mehr zu erwarten sind 
    * Fähigkeiten des Produktes (bspw. "Kann Musik streamen und abspielen") 
    * Beschreibung, wie sich Updates installieren lassen

* Organisieren und Beschreiben eines Koordinieren Schwachstellen Enthüllungsvorgehens (coordinated vulnerability disclosure, CVD), s. Art. 13, VIII

* Bedienen folgender Berichtsanforderungen , s. Art. 14:

    * Aktiv ausgenutzte Schwachstellen innerhalb 24h nach Bekanntwerden an die ENISA und die nationale, Benannte Stelle (DE = BSI), s. Art 14 II a)
    * Innerhalb 72h eine präzise Beschreibung der Maßnahmen, die angestrebt werden, s. Art. 14 II b)
    * Spätestens einen Monat nach der Auflösung der Situation ein vollständiger Bericht , s. Art. 14 II c)
    * Die Benannten Stellen dürfen nach Zwischenberichten fragen, s. Art 14 VI
    * Die Benutzer müssen informiert werden, dass es eine Gefahr gibt und was sie dagegen tun sollten (CSAF Security Advisory), s. Art. 14 VIII.
    * Jeden *sicherheitsrelevanten Vorfall* - der dazu geeignet wäre, die Sicherheit der Software-Supply Chain zu gefährden, bspw. gehackte Admin Credentials - innerhalb  von 24h and die ENISA und die Benannte Stelle zu melden.

  

## Lösungsansätze & Hilfestellung

### SBOM-Erstellung & Komponenten-Analyse

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [Syft](https://github.com/anchore/syft) | Apache-2.0 | Generiert SBOMs aus Container-Images, Dateisystemen und Quellcode in CycloneDX- und SPDX-Format; unterstützt 30+ Ökosysteme | CRA Annex I, Part II §1: Pflicht zur Komponentendokumentation; CRA Art. 13(4): SBOM bereitstellen |
| [cdxgen](https://github.com/CycloneDX/cdxgen) | Apache-2.0 | Erzeugt CycloneDX-SBOMs aus Quellcode und Build-Manifesten für 20+ Sprachen; unterscheidet Build- und Runtime-Dependencies | CRA Annex I, Part II §1; besonders geeignet für Hersteller, die mit Quellcode-Analysen argumentieren müssen |
| [Trivy](https://github.com/aquasecurity/trivy) | Apache-2.0 | All-in-One-Scanner: SBOM-Generierung + Schwachstellen + Fehlkonfigurationen + Secrets in einem Lauf; ideal für CI/CD | CRA Annex I, Part II §1+§2: SBOM und gleichzeitige Schwachstellenerkennung |
| [TrustSource CE](https://github.com/trustsource/ts-core-ce) | AGPL (Community Edition) | Vollständige SCA-Plattform: SBOM-Erstellung, -Versionierung und -Management, Vulnerability Management sowie CSAF-Kommunikation für Security Advisories; CLI-Clients für alle gängigen Build-Systeme | CRA Art. 13: Technische Dokumentation + SBOM; CRA Art. 14: CSAF-Advisories; NIS2 Art. 21(2)(a)(e): Lieferkettensicherheit |
| [SPDX Tools](https://github.com/spdx/tools-java) | Apache-2.0 | Referenzimplementierung für SPDX-Format: Validierung, Konvertierung, Generierung | CRA: SPDX ist ISO/IEC-Norm (ISO 5962:2021) — relevant für CE-Konformitätsdokumentation |

### Schwachstellen-Management

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [Grype](https://github.com/anchore/grype) | Apache-2.0 | Schwachstellenscanner auf Basis von Syft-SBOMs; gleicht Komponenten gegen NVD, GitHub Advisory DB und OSV ab | CRA Art. 13(6): Schwachstellen ohne ungebührliche Verzögerung beheben; Annex I, Part II §2: Keine bekannten ausnutzbaren Schwachstellen |
| [OSV-Scanner](https://github.com/google/osv-scanner) | Apache-2.0 | Scannt Dependency-Manifeste und SBOMs gegen die OSV-Datenbank (Google); hohe Abdeckung für Open-Source-Ökosysteme | CRA Art. 13(6); OSV-Datenbankqualität besonders hoch für npm, PyPI, Go, Rust |
| [Dependency-Track](https://dependencytrack.org/) | Apache-2.0 | Kontinuierliche SBOM-Analyse-Plattform (OWASP): nimmt SBOMs entgegen, überwacht fortlaufend gegen mehrere Vuln-Quellen, erzeugt VEX-Dokumente | CRA Art. 13 + Art. 14: Vollständiges Lifecycle-SBOM-Management und Meldeworkflows — de-facto Open-Source-Standard |
| [DefectDojo](https://github.com/DefectDojo/django-DefectDojo) | BSD-3-Clause | AppSec-Vulnerability-Management: aggregiert Scanner-Ergebnisse, dedupliziert, verfolgt Remediation und SLAs | CRA Art. 13(6): Dokumentierter Behebungsprozess mit Audit-Trail |

### Coordinated Vulnerability Disclosure (CVD) & Sicherheits-Advisories

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [BSI CSAF-Tooling](https://github.com/csaf-poc) | Apache-2.0 / MIT | CSAF-Referenz-Server (`csaf_provider`), Validator (`csaf_checker`) und Web-Editor (`secvisogram`) für maschinenlesbare Sicherheitsadvisories | CRA Art. 14(1): Pflicht zur Veröffentlichung von Sicherheitsadvisories; BSI TR-03191 empfiehlt CSAF als Standardformat |
| [OpenVEX](https://github.com/openvex/spec) | Apache-2.0 | Maschinenlesbares Format zur Kommunikation des Ausnutzbarkeitsstatus von Schwachstellen (affected / not-affected / fixed); `vexctl` CLI | CRA Art. 13(6) + Annex I: Hersteller müssen Schwachstellenstatus kommunizieren; reduziert False-Positive-Aufwand |
| [Vince](https://github.com/CERTCC/VINCE) | MIT | Open-Source-CVD-Case-Management-Plattform von CERT/CC: Intake, Triage, Koordination, Publikation | CRA Art. 14(1): Strukturierter CVD-Prozess mit Dokumentation |
| [disclose.io Templates](https://disclose.io/) | CC0 | Standardisierte CVD-Policy-Vorlagen mit rechtlicher Safe-Harbor-Sprache | CRA Art. 14(1): Einstiegspunkt für eine konforme CVD-Policy |

### Software Supply Chain Security

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [Sigstore / cosign](https://github.com/sigstore/cosign) | Apache-2.0 | Schlüsselloses Signieren und Verifizieren von Container-Images, SBOMs und anderen Artefakten; `cosign` kann signierte SBOMs direkt an Images anheften | CRA Annex I, Part II §3: Software-Integrität; NIS2 Art. 21(2)(a): Lieferkettensicherheit |
| [SLSA Framework](https://slsa.dev/) | Open Framework (OpenSSF) | Gestufte Anforderungen (L1–L4) für Build-Integrität mit verifizierbarer Provenance; `slsa-github-generator` für GitHub Actions | CRA Annex I, Part II: Sichere Entwicklungsprozesse; SLSA L2+ als praktisches Minimum für CRA-konforme CI/CD-Pipelines |
| [in-toto](https://in-toto.io/) | Apache-2.0 | Kryptografisch verifierbarer Nachweis jedes Build-Pipeline-Schritts (wer hat was ausgeführt, mit welchen Inputs) | CRA Annex I, Part II §4: Dokumentation des sicheren Entwicklungslebenszyklus |
| [GUAC](https://github.com/guacsec/guac) | Apache-2.0 | Verknüpft SBOM-, SLSA- und Schwachstellendaten in einem Graphen; ermöglicht Queries wie „welche unserer Produkte sind von CVE-X betroffen?" | CRA Art. 13 + NIS2 Art. 21(2)(a): Supply-Chain-weite Schwachstellenanalyse |


