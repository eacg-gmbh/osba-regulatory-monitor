---
tags:
   - cybersecurity
   - iot
   - hardware
   - documentation
---

# Radio Equipment Directive (RED)

Die Funkanlagenrichtlinie (Directive 2014/53/EU, RED) regelt das Inverkehrbringen von Funkgeräten auf dem EU-Markt. Eine Erweiterung durch die Delegierte Verordnung (EU) 2022/30 fügte ab 2025 verbindliche **Cybersicherheitsanforderungen** für internetfähige und an Kinder gerichtete Funkgeräte hinzu — und schließt damit eine langjährige Lücke bei vernetzten Alltagsgeräten.

## Überblick

* **Segment**: Produktsicherheit / Cybersicherheit für Funkgeräte (Radio Equipment)
* **Verabschiedet / Veröffentlicht**: Richtlinie 2014/53/EU; Cybersicherheitserweiterung durch Delegierte Verordnung (EU) 2022/30 (veröffentlicht Februar 2022)
* **Gültig ab**:
  * Grundanforderungen (Gesundheit, Sicherheit, Spektrum): bereits gültig seit Juni 2017
  * Cybersicherheitsanforderungen nach Art. 3(3)(d)(e)(f): **1. August 2025** (nach Verlängerung der ursprünglichen Frist von August 2024)
* **Gültig für**:
  * Alle **Funkgeräte**, die Funksignale senden oder empfangen — inkl. Smartphones, Tablets, Smartwatches, Laptops mit WLAN/Bluetooth, IoT-Geräte, Smart-Home-Geräte, Wearables, Kinderspielzeug mit Funktechnik, Drohnen, schnurlose Telefone
  * Speziell für Cybersicherheitsanforderungen: **internetfähige Funkgeräte** und **an Kinder gerichtete** Funkgeräte
* **Nicht gültig für**:
  * Funkanlagen, die ausschließlich für staatliche Sicherheits-, Verteidigungs- oder Strafverfolgungszwecke bestimmt sind
  * Luftfahrtgeräte (reguliert durch EASA-Verordnungen)
  * Amateurfunkgeräte (Bausätze)
  * Schifffahrtsausrüstung (reguliert durch MED-Richtlinie)
* **Grauzone**:
  * Abgrenzung „internetfähig" bei Geräten mit indirekter Netzwerkverbindung (z.B. nur Bluetooth zu einem Hub)
  * Anforderungen an Software-Updates nach dem Inverkehrbringen (Wechselwirkung mit CRA)
  * Zuständigkeit bei Kombinationsprodukten (Funkgerät + medizinisches Gerät)
  * Verhältnis zum Cyber Resilience Act: beide können gleichzeitig anwendbar sein; RED gilt speziell für Funkaspekte, CRA für die gesamte digitale Sicherheit



## Zentrale Forderungen

### Grundanforderungen (Art. 3, Richtlinie 2014/53/EU)

* **Art. 3(1)(a)**: Schutz von Gesundheit und Sicherheit — das Gerät darf keine Gefahr für Personen, Haustiere oder Sachgüter darstellen
* **Art. 3(1)(b)**: Elektromagnetische Verträglichkeit (EMV)
* **Art. 3(2)**: Effiziente Nutzung des Funkspektrums, Vermeidung von Störungen

### Cybersicherheitsanforderungen (Art. 3(3)(d)(e)(f), Delegierte VO (EU) 2022/30)

* **Art. 3(3)(d) — Netzwerkschutz**: Funkgeräte dürfen Netzwerke, in die sie eingebunden sind, nicht schädigen; Schutz vor unbeabsichtigten Eingriffen
* **Art. 3(3)(e) — Datenschutz**: Funkgeräte müssen Schutzmechanismen für personenbezogene Daten und die Privatsphäre der Nutzer enthalten; Schutz vor unbefugtem Datenzugriff und -übertragung
* **Art. 3(3)(f) — Betrugsprävention**: Funkgeräte müssen Merkmale aufweisen, die Betrug verhindern (z.B. sichere Authentifizierung, Integrität von Finanztransaktionen)

### Konformitätsbewertung & Markteinführung

* **CE-Kennzeichnung** und Ausstellung einer **EU-Konformitätserklärung** (DoC) verpflichtend
* Technische Dokumentation muss erstellt und 10 Jahre aufbewahrt werden
* Für sicherheitskritische Geräte oder bei Abweichung von harmonisierten Normen: Einschaltung einer **Benannten Stelle (Notified Body)**
* Registrierung in der **EUDAMED-ähnlichen** Funkanlagen-Datenbank (für bestimmte Kategorien)

### Harmonisierte Normen

* **ETSI EN 303 645**: Cybersicherheits-Basisanforderungen für Consumer IoT — de-facto Referenzstandard für Art. 3(3)(d)(e)(f)
* **ETSI TS 103 701**: Prüfspezifikation zu EN 303 645
* Weitere ETSI- und CEN/CENELEC-Normen werden im Rahmen des Normungsmandats erarbeitet



## Lösungsansätze & Hilfestellungen

* Die **[ETSI EN 303 645](https://www.etsi.org/deliver/etsi_en/303600_303699/303645/02.01.01_60/en_303645v020101p.pdf)** ist die wichtigste harmonisierte Norm für die Cybersicherheitsanforderungen und definiert 13 Sicherheitsprovisions (u.a. keine Standard-Passwörter, Schwachstellenoffenlegung, Software-Updates, sichere Kommunikation)
* Die **Bundesnetzagentur** ist die zuständige Marktüberwachungsbehörde in Deutschland
* Das **BSI** veröffentlicht Orientierungshilfen zur technischen Umsetzung der Cybersicherheitsanforderungen für IoT-Geräte

### Tools & Werkzeuge

#### Firmware-Sicherheitsanalyse (Art. 3(3)(d)(e))

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [EMBA](https://github.com/e-m-b-a/emba) | GPL-3.0 | Vollständige Firmware-Sicherheitsanalyse: extrahiert Dateisysteme, erkennt veraltete Komponenten, bekannte CVEs, hartcodierte Secrets und unsichere Konfigurationen | ETSI EN 303 645 Provision 5.3 (keine veralteten Software-Komponenten); Art. 3(3)(d): Netzwerkschutz durch sichere Firmware |
| [Binwalk](https://github.com/ReFirmLabs/binwalk) | MIT | Firmware-Extraktion und -Analyse; erkennt eingebettete Dateisysteme, komprimierte Archive und bekannte Binärformate | Vorbereitung für tiefergehende Sicherheitsanalyse von Firmware-Images |
| [Syft](https://github.com/anchore/syft) | Apache-2.0 | SBOM-Generierung aus Firmware-Images und Containern — auch für eingebettete Linux-Systeme (Buildroot, OpenWrt) | Komponentendokumentation für technische Unterlagen; Grundlage für CVE-Abgleich |
| [Grype](https://github.com/anchore/grype) | Apache-2.0 | CVE-Scanner auf SBOM-Basis; auch offline für abgeschottete Entwicklungsumgebungen nutzbar | ETSI EN 303 645 Provision 5.3: Nachweis, dass keine bekannten ausnutzbaren Schwachstellen vorliegen |

#### Netzwerk- & Protokollsicherheit (Art. 3(3)(d))

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [Wireshark](https://github.com/wireshark/wireshark) | GPL-2.0 | Netzwerk-Protokollanalyse; überprüft, welche Daten das Gerät sendet und empfängt | ETSI EN 303 645 Provision 5.8 (minimale Angriffsfläche): Nachweis, dass keine unerwarteten Kommunikationskanäle aktiv sind |
| [OWASP ZAP](https://github.com/zaproxy/zaproxy) | Apache-2.0 | Dynamischer Sicherheitsscanner für Geräteschnittstellen und begleitende Web-/App-Backends | Art. 3(3)(d)(e): Sicherheitstest der Gerätekommunikation und API-Schnittstellen |
| [OpenWRT](https://github.com/openwrt/openwrt) | GPL-2.0 | Referenz-Firmware-Plattform für WLAN-Router und IoT-Gateways; regelmäßige Sicherheitsupdates | ETSI EN 303 645 Provision 5.3: Modell für update-fähige, sichere Embedded-Linux-Basis |

#### Schwachstellen- & Patch-Management (EN 303 645 Provision 5.3)

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [TrustSource CE](https://github.com/trustsource/ts-core-ce) | AGPL (Community Edition) | SBOM-Versionierung und kontinuierliches Vulnerability Management über den Produktlebenszyklus; CSAF-Kommunikation für Security Advisories | EN 303 645 Prov. 5.3: Aktives Tracking bekannter Schwachstellen über die gesamte Nutzungsdauer; Prov. 5.2: koordinierte Schwachstellenoffenlegung |
| [Dependency-Track](https://dependencytrack.org/) | Apache-2.0 | Kontinuierliche SBOM-Analyse mit Vuln-Monitoring und VEX-Dokumentation | Nachweis laufender Schwachstellenüberwachung für die technische Dokumentation |

#### Koordinierte Schwachstellenoffenlegung (EN 303 645 Provision 5.2)

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [BSI CSAF-Tooling](https://github.com/csaf-poc/csaf_provider) | Apache-2.0 / MIT | CSAF-Server, Validator und Web-Editor für maschinenlesbare Security Advisories | EN 303 645 Prov. 5.2: Hersteller müssen einen öffentlichen Kanal für Schwachstellenmeldungen bereitstellen und Advisories veröffentlichen |
| [disclose.io Templates](https://disclose.io/) | CC0 | Standardisierte CVD-Policy-Vorlagen mit rechtlicher Safe-Harbor-Sprache | Einstiegspunkt für eine konforme Vulnerability-Disclosure-Policy nach EN 303 645 Prov. 5.2 |
