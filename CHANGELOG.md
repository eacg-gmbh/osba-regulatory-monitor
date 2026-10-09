# Regulatory Monitor Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/) and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

### Added
- **CRA**: Abschnitt „BSI TR-03183: Technische Richtlinie des BSI" mit Teil 1 (1.0.0), Teil 2 SBOM (2.1.0; CycloneDX ≥ 1.6, SPDX ≥ 3.0.1, Pflichtfelder), Teil 3 Schwachstellenmeldungen (1.0.0) und Teil H Modul H (1.1.0); Hinweis auf fehlende Konformitätsvermutung; Quellen aktualisiert. Kurzverweise in **NIS2** und **DORA**
- **Wissensbasis**: `wissensbasis/bsi-tr-03183.md` fasst die TR-03183 intern zusammen
- **Wissensbasis**: `wissensbasis/nis2-bsi-infopakete.md` fasst die BSI-#nis2know-Infopakete (Risikoanalyse, Incident Response, BCM, Lieferkette, Sicherheitsmaßnahmen/Schwachstellenmanagement, Wirksamkeit, Schulungen, Kryptografie, Personal/Zugriff/Assets, MFA, Meldepflicht, Geschäftsleitungsschulung, DORA, ISO/IEC 27001, Gesundheit) als internen Hintergrund zusammen (nicht Teil der veröffentlichten Website)
- **NIS2**: Abschnitt „Vorgaben des BSI (Deutschland)" auf Basis der BSI-Primärquellen (NIS-2-Pflichten, Registrierungspflicht, Meldepflicht, FAQ, Checkliste, Infopakete zu Risikomanagement, Lieferkette, Sicherheitsmaßnahmen/Schwachstellenmanagement, DORA und Geschäftsleitungsschulung); BSI-Portal seit 06.01.2026, keine allgemeine Übergangsfrist, Registrierung innerhalb von drei Monaten, Meldewege, Software- und Lieferkettenvorgaben; DORA-Abgrenzung um § 28 Abs. 7 BSIG (keine Doppelmeldung) und fortbestehende Registrierungspflicht ergänzt
- **DORA**: Seite vertieft — Verordnung (EU) 2022/2554 mit Verabschiedungs- und Anwendungsdaten, Geltungsbereich und Ausnahmen (Art. 2), Neuerungen, zentrale Forderungen mit Artikelverweisen (Art. 5–50), Meldefristen für Vorfälle (4 h / 72 h / 1 Monat), TLPT, Informationsregister und Mindestvertragsinhalte, Aufsicht über kritische IKT-Drittanbieter, Sanktionen, Abschnitt „Relevanz für Software-Hersteller und Open Source", Zeitplan der Level-2-Rechtsakte, Abschnitt „Wechselwirkungen mit anderen EU-Regularien" (NIS2, CRA, AI Act, PLD); SBOM-&-Lieferkettensicherheit-Tabelle (ts-scan, TrustSource CE, Dependency-Track)

### Changed
- **Alle Seiten DORA, CRA, NIS2, AI Act, PLD**: Aussagen gegen den Wortlaut im Amtsblatt der EU geprüft, Artikelverweise als Links zu EUR-Lex ergänzt, Abschnitt „Quellen" mit ELI-Links hinzugefügt
- **DORA**: Meldefristen der Delegierten Verordnung (EU) 2025/301 zugeordnet statt Art. 19; Art. 16 (vereinfachter Rahmen) und Art. 30 (Abs. 2 vs. Abs. 3) präzisiert; Delegierte Verordnung (EU) 2024/1774 (Open-Source-Bibliotheken, Quellcodeprüfung) ergänzt
- **CRA**: Anwendungsdaten (Kapitel IV ab 11.06.2026, Art. 14 ab 11.09.2026, Rest ab 11.12.2027), Ausnahmen, Produktklassen, Meldepflichten (Empfänger, Fristen, Abschlussberichte), Sanktionen und Support-Zeiträume korrigiert bzw. ergänzt; falsche Artikelverweise in Text und Tool-Tabellen berichtigt
- **NIS2**: Anwendungsdaten, Begriffe (wesentliche/wichtige Einrichtungen), Lieferkette (Art. 21 Abs. 2 lit. d statt lit. a), Aufsicht und Bußgelder belegt; deutsche Umsetzung (BSIG, BGBl. 2025 I Nr. 301) ergänzt; defekte Links ersetzt
- **AI Act**: Anwendungstermine nach der Digital-Omnibus-Verordnung (EU) 2026/1744 aktualisiert (Hochrisiko Anhang III ab 02.12.2027, Anhang I ab 02.08.2028); Art. 5, Open-Source-Ausnahme, GPAI, Art. 50, Sanktionen korrigiert; Wechselwirkungs-Tabelle (DORA, CRA, NIS2, PLD) neu belegt
- **PLD**: Verabschiedung, Geltung ab 09.12.2026, Haftende, Produktbegriff, Beweiserleichterungen, Fristen und Haftungsausschlüsse belegt; unbelegte Aussagen zu Höchstgrenze/Selbstbehalt abgeschwächt

### Fixed
- **DORA**: Tippfehler korrigiert

---

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
