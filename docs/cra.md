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

* Bereitstellen einer Komformitätserklärung, s. Art 13 XII, resp. Art. 28 I und Annex IV

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

