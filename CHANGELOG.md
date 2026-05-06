# Regulatory Monitor Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/) and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [0.5.0] - 2026-05-07

### Added
- **RED** (Radio Equipment Directive): Seite vollständig ausgearbeitet — Überblick, zentrale Forderungen (Art. 3(3)(d)(e)(f), Delegierte VO (EU) 2022/30), ETSI EN 303 645 als Referenznorm, Tool-Tabellen für Firmware-Analyse, Netzwerksicherheit, Vulnerability Management und CVD
- **PLD** (Product Liability Directive): Seite vollständig ausgearbeitet — Directive (EU) 2024/2853, Software als Produkt, erweiterter Schadensbegriff inkl. Datenverlust, Beweislasterleichterung, 10-jährige Haftungsfrist, Tool-Tabellen
- **About**: OSBA vorgestellt, Taskforce CRA, EACG als Sponsoring-Organisation und TrustSource beschrieben
- **IEC 62443**: TrustSource ts-scan im SBOM- & Schwachstellenmanagement-Abschnitt ergänzt

### Changed
- **NIS2**: Deming korrekt in GRC & Risikomanagement eingeordnet (statt Incident Management); Vanta entfernt
- **KRITIS-DachG**: Deming und PILAR (kommerziell) aus Incident-Management-Liste entfernt
- **Navigation**: Non-EU-Sektion entfernt (kein Inhalt vorhanden)

### Fixed
- Redaktionelle Änderungen

---

## [0.4.0] - 2026-05-06

### Added
- **CRA**: TrustSource ts-scan und sbom2notice in SBOM-Sektion; TrustSource CE in Vulnerability Management, CVD und Software Supply Chain Security; MetaTrust CRA-Assessment-Link als Einstiegshilfe
- **NIS2**: TrustSource ts-scan und neuer SBOM & Lieferkettensicherheit-Abschnitt
- **IEC 62443**: Vollständige Tool-Sektion entlang des Umsetzungspfads (Asset-Inventar → Gap-Analyse → Bedrohungsmodellierung → Monitoring → SBOM/Vuln)
- **eIDAS 2.0**: Link zum Architecture Reference Framework (ARF) der EU-Kommission eingebaut

### Changed
- Alle Seiten: Kommerzielle Tools entfernt — konsequente Open-Source-only-Ausrichtung gemäß OSBA-Kontext
- TrustSource CE: Lizenz auf AGPL (Community Edition) aktualisiert, Fähigkeiten präzisiert (SBOM-Versionierung, Vulnerability Management, CSAF-Kommunikation)

### Fixed
- **AI Act**: GPAI erstmals eingeführt als „General Purpose AI Model"; fehlerhaften NIST AI RMF Playbook-Link korrigiert
- Tote Links und nicht existierende Tools entfernt (u.a. aus MDR, DORA, KRITIS-DachG)
- Redaktionelle Änderungen

---

## [0.3.0] - 2026-05-06

### Added
- Neue Regulierungsseiten: **EU AI Act**, **EU Data Act**, **eIDAS 2.0 / EUDIW**, **KRITIS-Dachgesetz**
- Tool-Sektionen für alle bestehenden Regulierungsseiten (CRA, NIS2, DORA, MDR, IEC 62304, IEC 62443, OpenChain/ISO 5230, IEC 18974, IEC 81001-5-1)
- Neue Navigationssektion „Deutschland" für das KRITIS-Dachgesetz

### Fixed
- Redaktionelle Änderungen

---

## [0.2.0] - 2025-07-10

### Added
- **CER** (Directive on the Resilience of Critical Entities): neue Seite
- **IEC 18974**: neue Seite
- **IEC 81001-5-1**: neue Seite und Verlinkungen korrigiert

### Fixed
- Tote Links bereinigt; Zusammenfassungen der IEC-Standards ergänzt
- Redaktionelle Änderungen

---

## [0.1.0] - 2025-06-09

### Added
- Erste inhaltliche Regulierungsseiten: NIS2, CRA, DORA, MDR, PLD, RED, IEC 62304, IEC 62443, ISO 5230 (OpenChain)
- Tag-basierter Index und Navigation
- Beitragsrichtlinien (guidelines.md)

### Fixed
- Redaktionelle Änderungen

---

## [0.0.1] - 2025-04-03

### New Features
- Added theme and basic pages
