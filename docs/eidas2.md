---
tags:
   - identity
   - authentication
   - general
   - digital identity
---

# eIDAS 2.0 / European Digital Identity Wallet (EUDIW)

Die überarbeitete eIDAS-Verordnung (eIDAS 2.0) erweitert den europäischen Rahmen für elektronische Identifizierung und Vertrauensdienste um eine zentrale Neuerung: die **European Digital Identity Wallet (EUDIW)**. Damit erhalten EU-Bürgerinnen und -Bürger sowie Unternehmen eine einheitliche digitale Brieftasche, mit der sie sich grenzüberschreitend sicher identifizieren und Nachweise (Qualifikationen, Zertifikate, Attribute) vorzeigen können — ohne übermäßige Datenweitergabe.

## Überblick

* **Segment**: Digitale Identität, Vertrauensdienste, Authentifizierung
* **Verabschiedet / Veröffentlicht**: 11. April 2024 (ABl. EU), Verordnung (EU) 2024/1183
* **Gültig ab**:
  * Sofortige Geltung der Verordnung ab Mai 2024
  * **Mitgliedstaaten** müssen die EUDIW ihren Bürgern spätestens **24 Monate** nach Inkrafttreten der Durchführungsrechtsakte anbieten (Durchführungsrechtsakte werden schrittweise bis 2026 erwartet)
  * **Großplattformen** und bestimmte Diensteanbieter (Banken, Telekommunikation, Gesundheit, öffentliche Dienste) müssen die EUDIW als Authentifizierungsmittel akzeptieren
* **Gültig für**:
  * EU-Mitgliedstaaten (Pflicht zur Bereitstellung der Wallet)
  * Vertrauensdiensteanbieter (TSP) — qualifizierte und nicht-qualifizierte
  * Diensteanbieter, die eine starke Nutzer-Authentifizierung verlangen (Pflicht zur Akzeptanz der EUDIW)
  * Sehr große Online-Plattformen (VLOP) im Sinne des Digital Services Act
* **Nicht gültig für**:
  * Rein interne Unternehmenssysteme ohne Außenwirkung
  * Dienste, die keine Identifizierung oder Authentifizierung von Nutzern erfordern
* **Grauzone**:
  * Genaue Abgrenzung, welche Dienste zur Akzeptanz der EUDIW verpflichtet sind (abhängig von Durchführungsrechtsakten)
  * Zusammenspiel mit bestehenden nationalen eID-Lösungen (z.B. der deutschen Online-Ausweisfunktion)
  * Datenschutzrechtliche Ausgestaltung beim Einsatz durch private Diensteanbieter



## Zentrale Forderungen

### Bereitstellung der Wallet durch Mitgliedstaaten (Art. 5a)

* Jeder Mitgliedstaat muss mindestens **eine EUDIW** anbieten oder anerkennen
* Die Wallet muss **kostenlos für natürliche Personen** sein
* Unterstützung von **qualifizierten elektronischen Attributsbescheinigungen (QEAA)** — d.h. amtlich bestätigte digitale Nachweise (Führerschein, Diplom, etc.)
* Die Wallet muss das **Minimalitätsprinzip** technisch durchsetzen: Nutzer geben nur die Daten frei, die für den jeweiligen Zweck erforderlich sind (Selective Disclosure)

### Qualifizierte Vertrauensdienste (Art. 45a ff.)

* Neue Vertrauensdienste werden eingeführt: qualifizierte elektronische Attributsbescheinigungen (QEAA), qualifizierte elektronische Archivierungsdienste, qualifizierte Verwaltung von Remote-Signiervorrichtungen
* Vertrauensdiensteanbieter müssen sich zertifizieren lassen und stehen unter Aufsicht der nationalen Aufsichtsbehörden
* **Qualifizierte Zertifikate für Website-Authentifizierung (QWAC)** werden gestärkt: Browser müssen QWACs künftig anzeigen und respektieren

### Pflicht zur Akzeptanz der EUDIW (Art. 5b)

* Folgende Sektoren sind verpflichtet, die EUDIW als Identifizierungsmittel zu akzeptieren:
  * Öffentliche Online-Dienste
  * Banken und Finanzdienstleister (im Rahmen der Kundenidentifizierung / KYC)
  * Telekommunikationsanbieter (bei SIM-Registrierung)
  * Sehr große Online-Plattformen (VLOP gemäß DSA)
  * Gesundheitsdienstleister (für den Zugang zu Patientendaten)

### Technische Anforderungen (Art. 5a Abs. 4, Durchführungsrechtsakte)

* Vollständige **Offline-Nutzbarkeit** für ausgewählte Anwendungsfälle
* **Interoperabilität** zwischen Wallets verschiedener Mitgliedstaaten (EU-weite Interoperabilitätsarchitektur, [ARF — Architecture Reference Framework](https://digital-strategy.ec.europa.eu/en/library/european-digital-identity-architecture-and-reference-framework-outline))
* **Kein Tracking**: Diensteanbieter und Wallet-Anbieter dürfen Nutzerverhalten nicht länderübergreifend nachverfolgen
* Sicherheitszertifizierung der Wallet nach anerkannten Standards (Common Criteria oder gleichwertig)

### Elektronische Signaturen und Siegel (Art. 26 ff., unverändert und erweitert)

* Qualifizierte elektronische Signaturen (QES) bleiben rechtlich der handschriftlichen Unterschrift gleichgestellt
* Erweiterte Möglichkeiten für qualifizierte Remote-Signaturen über die Wallet



## Lösungsansätze & Hilfestellungen

* Das **[Architecture Reference Framework (ARF)](https://digital-strategy.ec.europa.eu/en/library/european-digital-identity-architecture-and-reference-framework-outline)** der EU-Kommission beschreibt die technischen Grundlagen der EUDIW und wird laufend aktualisiert — Referenzimplementierungen sind geplant
* Der **OpenID for Verifiable Credentials (OID4VC)**-Standard und **ISO/IEC 18013-5** (mDL — Mobile Driving License) sind die zentralen technischen Protokolle für die EUDIW
* Für Diensteanbieter: Frühzeitig prüfen, ob man zur Pflichtgruppe gehört, und bestehende Authentifizierungslösungen auf EUDIW-Kompatibilität vorbereiten
* Für Identitätsprovider und SSO-Anbieter: EUDIW als zusätzlichen Identitätsanbieter (IdP) integrieren
* In Deutschland koordiniert das **Bundesamt für Sicherheit in der Informationstechnik (BSI)** und das **Bundesministerium des Innern** die nationale Umsetzung

### Tools & Werkzeuge

#### EUDIW Referenz-Implementierungen (Art. 5a)

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [EU Commission Reference Wallet](https://github.com/eu-digital-identity-wallet) | Apache-2.0 | Offizielle Referenz-Wallet (Android/iOS) der EU-Kommission inkl. modularer Bibliotheken für Issuer, Verifier und Core-Logik | Direktes Art. 5a-Referenzwerk; normative Grundlage für Mitgliedstaaten-Wallets; deckt ARF vollständig ab |
| [Walt.id Identity Kit](https://github.com/walt-id/waltid-identity) | Apache-2.0 | End-to-End SSI-Stack: DID-Management, VC-Ausstellung, OID4VC/OID4VP und mdoc; produktionsreif und in EBSI/deutschen Piloten eingesetzt | Wahrscheinlich vollständigster Open-Source-Stack für EUDIW; deckt alle ARF-Protokollschichten ab |
| [Sphereon Wallet](https://github.com/Sphereon-Opensource/mobile-wallet) | Apache-2.0 | Open-Source SSI-Wallet mit EUDIW-kompatiblem Credential-Support; OID4VC/OID4VP-Implementierung | Einsatz in EU-Pilotprojekten; interoperabel mit EBSI |

#### OID4VC / OID4VP Bibliotheken (Kernprotokolle der EUDIW)

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [Sphereon OID4VC Libraries](https://github.com/Sphereon-Opensource/OID4VC) | Apache-2.0 | Vollständige OID4VCI + OID4VP Client- und Server-Bibliotheken für TypeScript/Node.js | Implementiert den vorgeschriebenen EUDIW-Protokoll-Stack; in EU-Kommissions-Piloten verwendet |
| [Walt.id OID4VC Kit](https://github.com/walt-id/waltid-openid4vc) | Apache-2.0 | Kotlin/JVM-Toolkit für OID4VCI, OID4VP und SD-JWT VC; produktionsreif | Umfangreich in EBSI und EUDIW-Ökosystem eingesetzt; deckt Issuer-/Verifier-/Holder-Flows ab |
| [Veramo](https://github.com/decentralized-identity/veramo) | Apache-2.0 | JavaScript/TypeScript-Framework für DID- und VC-Operationen | Ausstellung, Speicherung und Verifikation von W3C VCs; in EBSI-kompatiblen Deployments eingesetzt |

#### SD-JWT & mdoc (Pflicht-Credential-Formate laut ARF)

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [SD-JWT Bibliotheken](https://github.com/openwallet-foundation-labs/sd-jwt-python) | Apache-2.0 / MIT | Selective Disclosure JWT: gibt Nutzer Kontrolle, welche Attribute offenbart werden (Python, Rust, Java, TS verfügbar) | SD-JWT VC ist laut ARF v1.4+ das Pflicht-Credential-Format der EUDIW; Selective Disclosure erfüllt Art. 5a(7) Datensparsamkeit |
| [OpenWallet Foundation mdoc](https://github.com/openwallet-foundation-labs) | Apache-2.0 | Plattformübergreifende mdoc/mDL-Implementierung nach ISO/IEC 18013-5 | ARF mandatiert mdoc als Credential-Format für PID und mDL; OWF-Bibliotheken auf EUDIW-Interoperabilität ausgerichtet |
| [Walt.id mdoc Library](https://github.com/walt-id/waltid-mdoc-credentials) | Apache-2.0 | Kotlin-Bibliothek für mdoc-Credential-Lifecycle (Ausstellung, Präsentation, Verifikation) | In Walt.id-Ökosystem integriert; EUDIW-kompatibel |

#### SSI-Frameworks & Trust-Infrastruktur

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [Hyperledger Aries / ACA-Py](https://github.com/hyperledger/aries-cloudagent-python) | Apache-2.0 | Vollständiges SSI-Agent-Framework mit DIDComm, VC-Ausstellung/-Verifikation; wird für OID4VC-Kompatibilität erweitert | Etablierter SSI-Stack; Basis für viele EUDIW-kompatible Deployments |
| [Credo-TS](https://github.com/openwallet-foundation/credo-ts) | Apache-2.0 | TypeScript/React-Native SSI-Agent (Nachfolger von Aries Framework JavaScript); EUDIW-kompatibel | Für mobile Wallet-Entwicklung; von Sphereon und anderen EU-Ecosystem-Wallets genutzt |
| [EBSI](https://ec.europa.eu/digital-building-blocks/wikis/display/EBSI) | Public / Open APIs | EU-gemanagtes DID-Register und VC-Trust-Framework | Art. 6a eIDAS 2.0 Trust-Framework-Backbone; Mitgliedstaaten verankern Trust-Anchors hier |
