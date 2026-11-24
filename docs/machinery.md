---
tags:
   - cybersecurity
   - ai
   - risk management
   - documentation
   - general
---

# EU Maschinenverordnung (MVO)

Die Maschinenverordnung (Verordnung (EU) 2023/1230, englisch: Machinery Regulation) ist das Produktsicherheitsrecht der EU für Maschinen und löst die Maschinenrichtlinie 2006/42/EG ab. Für Software ist sie relevant, weil sie Software erstmals ausdrücklich als Sicherheitsbauteil erfasst, digitale Veränderungen einer Maschine regelt und Schutz gegen Korrumpierung sowie gegen böswillige Angriffe verlangt, soweit davon die Sicherheit von Personen abhängt.

> [!NOTE]
>
> Alle Artikel- und Erwägungsgrundverweise beziehen sich, sofern nicht anders angegeben, auf die [Verordnung (EU) 2023/1230](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230) und führen direkt zur jeweiligen Stelle (EUR-Lex, Ursprungsfassung vom 29.06.2023). Die Ursprungsfassung nennt als Anwendungsdatum noch den 14.01.2027; maßgeblich sind die durch die Berichtigung vom 04.07.2023 korrigierten Daten und die [konsolidierte Fassung vom 27.07.2026](https://eur-lex.europa.eu/legal-content/DE/TXT/?uri=CELEX:02023R1230-20260727). Anhänge sind in der Ursprungsfassung nicht einzeln verlinkbar. Die Seite ersetzt keine Rechtsberatung.

## Überblick

* **Segment**: Produktsicherheit (Binnenmarkt) / IT Sicherheit

* **Verabschiedet / Veröffentlicht**:
    * Verordnung (EU) 2023/1230 vom 14.06.2023, veröffentlicht im Amtsblatt der EU (L 165) am 29.06.2023
    * Inkrafttreten: 19.07.2023 (20. Tag nach Veröffentlichung, [Art. 54](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#art_54))
    * Berichtigung (ABl. L 169 vom 04.07.2023, S. 35): alle Datumsangaben um sechs Tage verschoben
    * Geändert durch die Verordnung (EU) 2024/2748 (Notfallverfahren, Kapitel IVa) und die [Verordnung (EU) 2026/1744](https://eur-lex.europa.eu/eli/reg/2026/1744/oj) (Verzahnung mit dem AI Act)

* **Gültig ab** ([Art. 54](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#art_54), in der berichtigten Fassung):
    * Notifizierung von Konformitätsbewertungsstellen ([Art. 26–42](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#art_26)): 20.01.2024
    * Sanktionsregeln der Mitgliedstaaten ([Art. 50 Abs. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#art_50)): 20.10.2026
    * Alle übrigen Bestimmungen: **20. Januar 2027**. Am selben Tag wird die Richtlinie 2006/42/EG aufgehoben ([Art. 51](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#art_51)).
    * Übergang ([Art. 52](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#art_52)): Produkte, die vor dem 20.01.2027 nach der Richtlinie in Verkehr gebracht wurden, dürfen weiter bereitgestellt werden; EG-Baumusterprüfbescheinigungen bleiben bis zu ihrem Ablauf gültig. Ein Wahlrecht zwischen altem und neuem Recht gibt es nicht.

* **Gültig für** ([Art. 2 Abs. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#art_2), [Art. 3](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#art_3)):
    * Maschinen und dazugehörige Produkte: auswechselbare Ausrüstungen, Sicherheitsbauteile, Lastaufnahmemittel, Ketten, Seile und Gurte, abnehmbare Gelenkwellen
    * Unvollständige Maschinen
    * **Software als Sicherheitsbauteil**: ein „physisches oder digitales Bauteil, einschließlich Software", das eine Sicherheitsfunktion gewährleistet und gesondert in Verkehr gebracht wird (Art. 3 Nr. 3)
    * Maschinen, bei denen „lediglich das Aufspielen" der anwendungsspezifischen Software fehlt, gelten bereits als Maschine (Art. 3 Nr. 1 lit. f)
    * Adressaten: Hersteller, Bevollmächtigte, Einführer, Händler sowie jede Person, die eine Maschine wesentlich verändert ([Art. 18](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#art_18))

* **Nicht gültig für** ([Art. 2 Abs. 2](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#art_2), Auswahl):
    * Sicherheitsbauteile als identische Ersatzteile des Originalherstellers
    * Waffen, Maschinen für militärische oder polizeiliche Zwecke, kerntechnische Spezialmaschinen
    * Luft-, Wasser- und Schienenfahrzeuge, Kraftfahrzeuge, zwei- und dreirädrige Fahrzeuge sowie land- und forstwirtschaftliche Zugmaschinen nach den jeweiligen Typgenehmigungsvorschriften (auf diesen Fahrzeugen angebrachte Maschinen sind dagegen erfasst)
    * Forschungsmaschinen zur vorübergehenden Verwendung in Laboratorien
    * Haushaltsgeräte, Audio- und Videogeräte, informationstechnische Geräte, gewöhnliche Büromaschinen, Niederspannungsschaltgeräte und Elektromotoren, soweit sie unter die Niederspannungsrichtlinie 2014/35/EU oder die [Funkanlagenrichtlinie](red.md) fallen

* **Grauzone**:
    * **Reine Software ohne Sicherheitsfunktion** (z. B. Leitstand, Fernwartungsportal, Auswertung von Maschinendaten) ist kein Produkt im Sinne der MVO. Sie kann die Maschine aber über eine Schnittstelle gefährden und ist dann Gegenstand der Risikobeurteilung des Maschinenherstellers (Anhang III Nr. 1.1.9) und meist eigenständig ein Produkt nach dem [CRA](cra.md).
    * **Open Source**: Die MVO enthält keine Sonderregel für freie Software. Maßgeblich ist, ob eine Abgabe „im Rahmen einer Geschäftstätigkeit" erfolgt, entgeltlich oder unentgeltlich (Art. 3 Nr. 11). Eine Rolle wie der Open-Source-Steward des CRA kennt die MVO nicht.
    * **Software-Updates als wesentliche Veränderung**: Ob ein Update eine „wesentliche Veränderung" ist, hängt davon ab, ob es vom Hersteller vorgesehen war und ob es eine neue Gefährdung schafft oder ein Risiko erhöht, das zusätzliche Schutzmaßnahmen verlangt (Art. 3 Nr. 16). Reparatur und Wartung ohne Einfluss auf die Konformität sind keine wesentliche Veränderung ([ErwG 26](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#rct_26)).
    * **Umfang der Cybersicherheit**: Verlangt sind nur verhältnismäßige Maßnahmen, die „auf den Schutz der Sicherheit" des Produkts begrenzt sind ([ErwG 25](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#rct_25)). Wo die Grenze zwischen sicherheitsrelevanter und sonstiger Software verläuft, legt der Hersteller in der Risikobeurteilung fest.
    * **Harmonisierte Normen** zu den Cyber-Anforderungen sind noch nicht im Amtsblatt zitiert (siehe [Lösungsansätze](#losungsansatze-hilfestellungen)).

* **Ziel**:
  Hohes Schutzniveau für Gesundheit und Sicherheit von Personen (sowie gegebenenfalls Haustieren, Sachen und Umwelt) bei Konstruktion und Bau von Maschinen und freier Warenverkehr für konforme Produkte ([Art. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#art_1)).

* **Neuerungen gegenüber der Maschinenrichtlinie 2006/42/EG**:
    * Verordnung statt Richtlinie: unmittelbare, einheitliche Geltung ohne nationale Umsetzung ([ErwG 4](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#rct_4))
    * Sicherheitsrisiken neuer digitaler Technologien (KI, IoT, Robotik) sind ausdrücklich erfasst ([ErwG 12](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#rct_12))
    * Software als Sicherheitsbauteil, wesentliche Veränderung „physisch oder digital", Schutz gegen Korrumpierung, Angriffsresistenz der Steuerung
    * Drittprüfung für Sicherheitsfunktionen mit maschinellem Lernen
    * Quellcode-Zugang für Behörden, digitale Betriebsanleitung
    * Ausdrückliche Pflichten für Einführer und Händler nach dem Muster des New Legislative Framework

## Zentrale Forderungen

* **Grundpflicht des Herstellers** ([Art. 10](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#art_10)): Konstruktion und Bau nach den grundlegenden Sicherheits- und Gesundheitsschutzanforderungen des Anhangs III, technische Unterlagen nach Anhang IV, Konformitätsbewertung ([Art. 25](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#art_25)), EU-Konformitätserklärung ([Art. 21](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#art_21)) und CE-Kennzeichnung ([Art. 23](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#art_23), [Art. 24](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#art_24)).

* **Risikobeurteilung** (Anhang III Teil B, Allgemeine Grundsätze): iterativer Prozess aus Festlegung der Grenzen der Maschine, Ermittlung der Gefährdungen, Abschätzung, Bewertung und Minderung der Risiken. Sie umfasst auch
    * künftige, beim Inverkehrbringen vorgesehene Aktualisierungen oder Weiterentwicklungen der installierten Software ([ErwG 32](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#rct_32)),
    * Gefährdungen aus selbstentwickelndem Verhalten und wechselnden Autonomiegraden,
    * Wechselwirkungen in einer Gesamtheit von Maschinen.

* **Schutz gegen Korrumpierung** (Anhang III Nr. 1.1.9):
    * Der Anschluss einer anderen Einrichtung oder eine kommunizierende Fernzugriffseinrichtung darf nicht zu einer gefährlichen Situation führen.
    * Hardware-Bauteile, die Signale oder Daten für den Zugriff auf sicherheitskritische Software übertragen, sind gegen unbeabsichtigte oder vorsätzliche Korrumpierung zu schützen; Eingriffe in diese Bauteile sind zu protokollieren.
    * Software und Daten, die für die Einhaltung der Sicherheitsanforderungen entscheidend sind, sind **als solche zu benennen** und gegen unbeabsichtigte oder vorsätzliche Korrumpierung zu schützen.
    * Die Maschine muss die für den sicheren Betrieb erforderliche **installierte Software kenntlich machen** und diese Information jederzeit leicht zugänglich bereitstellen.
    * Die Maschine muss **Nachweise für rechtmäßiges oder unrechtmäßiges Eingreifen** in die Software oder für Veränderungen der Software oder ihrer Konfiguration sammeln.

* **Sicherheit und Zuverlässigkeit von Steuerungen** (Anhang III Nr. 1.2.1):
    * Steuerungen müssen Fremdeinflüssen standhalten, „einschließlich vernünftigerweise vorhersehbare böswillige Versuche Dritter, die zu einer Gefährdungssituation führen" (lit. a).
    * Hardware- und Softwaredefekte, Logikfehler und vorhersehbare Bedienungsfehler dürfen nicht zu Gefährdungssituationen führen (lit. b, c, e).
    * Die Grenzen der Sicherheitsfunktionen werden in der Risikobeurteilung festgelegt; weder Bediener noch die Maschine selbst dürfen Einstellungen oder Regeln gefährdend ändern, auch nicht in einer Lernphase (lit. d).
    * **Rückverfolgungsprotokoll**: Daten zu Eingriffen und die Versionen der nach dem Inverkehrbringen aufgespielten Sicherheitssoftware müssen bis zu fünf Jahre nach dem Hochladen für Behörden zugänglich sein (lit. f).
    * Steuerungen mit selbstentwickelndem Verhalten: keine Handlungen außerhalb der festgelegten Aufgabe und des Bewegungsbereichs, Aufzeichnung der sicherheitsrelevanten Entscheidungsdaten für ein Jahr, jederzeitige Korrigierbarkeit.
    * Kabellose Steuerung: Ein Ausfall der Kommunikation darf nicht zu einer gefährlichen Situation führen.

* **Wesentliche Veränderung** (Art. 3 Nr. 16, [Art. 18](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#art_18)): Wer eine Maschine nach dem Inverkehrbringen physisch oder digital so verändert, dass eine neue Gefährdung entsteht oder ein Risiko steigt, gilt als Hersteller und muss die Konformitätsbewertung für die Maschine oder den betroffenen Teil erneut durchführen. Ausgenommen sind nichtgewerbliche Nutzer, die ihre eigene Maschine für den Eigengebrauch verändern.

* **Konformitätsbewertung** ([Art. 6](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#art_6), [Art. 25](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#art_25), Anhang I):
    * Nicht in Anhang I gelistet (Regelfall): interne Fertigungskontrolle (Modul A)
    * Anhang I Teil B (u. a. Logikeinheiten für Sicherheitsfunktionen, Schutzeinrichtungen zur Personendetektion): Modul A nur bei vollständiger Anwendung harmonisierter Normen oder gemeinsamer Spezifikationen, sonst notifizierte Stelle
    * Anhang I Teil A: immer notifizierte Stelle (Module B+C, H oder G). Dazu gehören **Sicherheitsbauteile und eingebettete Systeme „mit vollständig oder teilweise selbstentwickelndem Verhalten unter Verwendung von Ansätzen des maschinellen Lernens, die Sicherheitsfunktionen gewährleisten"** (Nr. 5 und 6). Software, die nicht lernfähig ist und nur automatisierte Funktionen ausführt, fällt nicht darunter ([ErwG 55](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#rct_55)).

* **Technische Unterlagen** (Anhang IV Teil A), u. a.:
    * Risikobeurteilung mit Liste der anwendbaren Anforderungen und der Schutzmaßnahmen
    * Quellcode oder Programmierlogik der sicherheitsrelevanten Software, auf begründeten Antrag einer Behörde (lit. m; ebenso [Art. 10 Abs. 3](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#art_10))
    * Bei sensorgesteuerten, ferngesteuerten oder autonomen Maschinen: Beschreibung der Merkmale, Fähigkeiten und Grenzen des Systems sowie der Daten-, Entwicklungs-, Test- und Validierungsprozesse (lit. n)
    * Aufbewahrung: mindestens zehn Jahre ([Art. 10 Abs. 3](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#art_10))

* **Betriebsanleitung und Konformitätserklärung** dürfen digital bereitgestellt werden: druck- und speicherbar, online für die erwartete Lebensdauer und mindestens zehn Jahre; auf Wunsch beim Kauf kostenlos in Papierform binnen eines Monats ([Art. 10 Abs. 7 und 8](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#art_10)).

* **Konformitätsvermutung** ([Art. 20](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#art_20)): über harmonisierte Normen, gemeinsame Spezifikationen der Kommission oder, für Nr. 1.1.9 und 1.2.1, über ein Zertifikat nach einem europäischen Schema für die Cybersicherheitszertifizierung (Verordnung (EU) 2019/881), soweit es diese Anforderungen abdeckt (Abs. 9).

* **Sanktionen** ([Art. 50](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#art_50)): Die Mitgliedstaaten legen wirksame, verhältnismäßige und abschreckende Sanktionen fest, die bei schweren Verstößen auch strafrechtlich sein können. Eine unionsweite Bußgeldobergrenze gibt es nicht. Die deutsche Regelung ist hier nicht geprüft.

### Konsequenzen für Software-Hersteller

| Situation | Folge nach der MVO |
|-----------|--------------------|
| Software mit Sicherheitsfunktion wird eigenständig vertrieben (z. B. Safety-Bibliothek, Überwachungssoftware) | Sicherheitsbauteil: Der Anbieter ist Hersteller mit Risikobeurteilung, technischen Unterlagen, Konformitätserklärung und CE-Kennzeichnung (Art. 3 Nr. 3, Art. 10) |
| Die Sicherheitsfunktion beruht auf maschinellem Lernen | Immer Konformitätsbewertung durch eine notifizierte Stelle (Anhang I Teil A Nr. 5 und 6) |
| Software wird in die Maschine eines Kunden integriert | Pflichten treffen den Maschinenhersteller. Er wird vom Zulieferer Angaben zu sicherheitsrelevanten Komponenten, Integritätsschutz, Protokollierung und Versionierung verlangen (Anhang III Nr. 1.1.9, 1.2.1) |
| Update oder Nachrüstung nach dem Inverkehrbringen | Prüfen, ob das Update vorgesehen war und in der Risikobeurteilung berücksichtigt ist. Andernfalls droht eine wesentliche Veränderung mit Herstellerpflichten für den, der sie vornimmt (Art. 18) |
| Fernwartung, Cloud-Anbindung, Schnittstellen | Dürfen nicht zu einer gefährlichen Situation führen; Verbindungsverlust muss beherrscht sein (Anhang III Nr. 1.1.9, 1.2.1) |
| Sicherheitsrelevante Software insgesamt | Benennen, gegen Korrumpierung schützen, auf der Maschine auslesbar machen, Eingriffe protokollieren, Versionen fünf Jahre rückverfolgbar halten; Quellcode auf begründeten Antrag an Behörden |

**Was die MVO nicht verlangt:** keine SBOM, keinen Prozess zur Schwachstellenbehandlung, keine koordinierte Offenlegung, keine Pflicht zu Sicherheitsupdates, keinen Unterstützungszeitraum und keine Meldung von Schwachstellen. Diese Pflichten ergeben sich für vernetzte Maschinen aus dem [CRA](cra.md).

### Verhältnis zum Cyber Resilience Act (CRA)

Beide Verordnungen gelten **nebeneinander**. Eine Maschine mit Datenverbindung ist zugleich ein Produkt mit digitalen Elementen. Der [CRA](cra.md) erwähnt die MVO nur in [Erwägungsgrund 53](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32024R2847#rct_53): Hersteller sollen beide Anforderungskataloge erfüllen und beide Konformitätsbewertungsverfahren durchführen. Die Einhaltung des CRA „könnte" die Einhaltung von Anhang III Nr. 1.1.9 und 1.2.1 erleichtern; diese Synergien muss der Hersteller nachweisen. Eine automatische Konformitätsvermutung in die eine oder andere Richtung gibt es nicht. Die MVO selbst hält in [ErwG 25](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230#rct_25) fest, dass andere Cybersicherheitsrechtsakte der Union anwendbar bleiben.

| | MVO | CRA |
|---|-----|-----|
| Schutzgut | Gesundheit und Sicherheit von Personen | Cybersicherheit des Produkts, seiner Nutzer und verbundener Netze |
| Umfang der Security | Nur Angriffe und Korrumpierung, die zu einer Gefährdungssituation führen | Alle Cybersicherheitsrisiken |
| Zeitlicher Bezug | Zustand beim Inverkehrbringen; Protokoll der Softwareversionen fünf Jahre | Gesamter Unterstützungszeitraum (mindestens fünf Jahre) |
| Schwachstellenbehandlung, SBOM, CVD, Updates | — | Anhang I Teil II |
| Meldepflichten | Risiko durch nichtkonformes Produkt an nationale Behörde (Art. 10 Abs. 9) | Ausgenutzte Schwachstellen und schwere Vorfälle binnen 24 h / 72 h (Art. 14) |
| Software-Inventar | Maschine macht sicherheitsrelevante Software kenntlich (Nr. 1.1.9) | SBOM in der technischen Dokumentation |
| Protokollierung | Nachweise für Eingriffe in Software und Konfiguration (Nr. 1.1.9, 1.2.1 lit. f) | Aufzeichnung sicherheitsrelevanter Aktivitäten (Anhang I Teil I Nr. 2 lit. l) |
| Anwendung | **20.01.2027** | Meldepflichten seit 11.09.2026, übrige Pflichten ab **11.12.2027** |

Praktisch heißt das: Die MVO greift knapp elf Monate vor den Produktanforderungen des CRA. Eine für den CRA angelegte Bedrohungs- und Risikoanalyse, in der die sicherheitsrelevanten Komponenten markiert sind, kann als Nachweis für Nr. 1.1.9 und 1.2.1 dienen, wenn der Bezug zu Gefährdungssituationen ausdrücklich hergestellt wird. Komponenten wie Steuerungen, Antriebe, Bediengeräte oder Gateways sind unabhängig von ihrer Einordnung nach der MVO eigenständige CRA-Produkte.

### Verhältnis zum AI Act

Die [Verordnung (EU) 2026/1744](https://eur-lex.europa.eu/eli/reg/2026/1744/oj) hat die MVO mit dem [AI Act](aiact.md) verzahnt (konsolidierte Fassung, Art. 8 Unterabs. 3 und Art. 20 Abs. 10):

* Die Kommission ergänzt Anhang III per delegiertem Rechtsakt um Sicherheits- und Gesundheitsschutzanforderungen für KI-Systeme, die nach Art. 6 Abs. 1 AI Act hochriskant sind, weil sie Sicherheitsbauteil eines Produkts der MVO oder selbst ein solches Produkt sind. Die Anforderungen sollen Kapitel III Abschnitt 2 sowie Art. 17, 19, 72 und 73 des AI Act widerspiegeln und sind bis zum 02.08.2028 anzuwenden.
* Bis eigene Normen vorliegen, begründen die harmonisierten Normen und gemeinsamen Spezifikationen des AI Act die Konformitätsvermutung für die KI-bezogenen Anforderungen.

Unabhängig davon enthält die MVO eigene Anforderungen an lernende Systeme: Risikobeurteilung über den Lebenszyklus, Grenzen für selbstentwickelndes Verhalten, Aufzeichnung der Entscheidungsdaten und Drittprüfung (siehe oben).

### Zeitplan

| Datum | Ereignis |
|-------|----------|
| 29.06.2023 | Veröffentlichung im Amtsblatt |
| 19.07.2023 | Inkrafttreten |
| 20.01.2024 | Regeln für notifizierte Stellen anwendbar |
| 11.09.2026 | CRA-Meldepflichten gelten (auch für vernetzte Maschinen) |
| 20.10.2026 | Sanktionsregeln der Mitgliedstaaten |
| **20.01.2027** | **MVO vollständig anwendbar, Richtlinie 2006/42/EG aufgehoben** |
| 11.12.2027 | CRA vollständig anwendbar |
| 02.08.2028 | Delegierte Rechtsakte zu KI-Anforderungen in Anhang III anzuwenden |

## Lösungsansätze & Hilfestellungen

Die MVO schreibt keine Werkzeuge oder Formate vor. Für die Software-Anforderungen aus Anhang III Nr. 1.1.9 und 1.2.1 lassen sich Bausteine nutzen, die auch für den [CRA](cra.md) gebraucht werden.

### Normen und Leitfäden

* **prEN 50742 „Sicherheit von Maschinen – Schutz gegen Korrumpierung"**: Normentwurf von CENELEC zu Anhang III Nr. 1.1.9 und Teilen von Nr. 1.2.1. Der Entwurf lag Anfang 2026 zur öffentlichen Umfrage aus ([DIN Media](https://www.dinmedia.de/en/draft-standard/din-en-50742/399142141)); eine Fundstelle im Amtsblatt und damit eine Konformitätsvermutung war bei der letzten Prüfung nicht zu ermitteln.
* **ISO/TR 22100-4** (Leitfaden für Maschinenhersteller zu IT-Sicherheitsaspekten) und **IEC TS 63074** (Security-Aspekte funktional sicherer Steuerungen): technische Berichte ohne Konformitätsvermutung.
* **[IEC 62443](iec62443.md)**: gemeinsame technische Grundlage für industrielle Automatisierung, anschlussfähig an MVO und CRA.

### Software-Inventar und Integrität

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [Syft](https://github.com/anchore/syft) | Apache-2.0 | Erzeugt ein Komponenteninventar (SBOM) aus Firmware-Images und Dateisystemen | Grundlage, um sicherheitsrelevante Software zu benennen und kenntlich zu machen (Anhang III Nr. 1.1.9); keine SBOM-Pflicht nach der MVO |
| [TrustSource ts-scan](https://trustsource.github.io/ts-scan) | Open Source | Scannt Quellcode, Builds und Images und liefert das Komponenteninventar | Wie oben; dasselbe Inventar dient der SBOM nach dem CRA |
| [TrustSource CE](https://github.com/trustsource/ts-core-ce) | AGPL (Community Edition) | Versioniertes Repository für Komponentenstände je Produktversion | Rückverfolgbarkeit der aufgespielten Softwareversionen (Anhang III Nr. 1.2.1 lit. f) |
| [Sigstore / cosign](https://github.com/sigstore/cosign) | Apache-2.0 | Signiert und verifiziert Software-Artefakte | Schutz sicherheitskritischer Software gegen Korrumpierung (Anhang III Nr. 1.1.9) |
| [RAUC](https://github.com/rauc/rauc) | LGPL-2.1 | Signierte, atomare Updates für Embedded Linux | Schutz gegen Korrumpierung beim Update; nachvollziehbare Versionsstände (Nr. 1.1.9, 1.2.1 lit. f) |
| [SWUpdate](https://github.com/sbabic/swupdate) | GPL-2.0 | Update-Framework für Embedded-Systeme mit Signaturprüfung | Wie RAUC |

### Risikobeurteilung

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [OWASP Threat Dragon](https://github.com/OWASP/threat-dragon) | Apache-2.0 | Bedrohungsmodellierung mit Datenflussdiagrammen | Ermittlung „vernünftigerweise vorhersehbarer böswilliger Versuche" (Anhang III Nr. 1.2.1 lit. a) als Teil der Risikobeurteilung |

## Quellen

* [Verordnung (EU) 2023/1230 (Maschinenverordnung)](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R1230), ELI: [eur-lex.europa.eu/eli/reg/2023/1230/oj](https://eur-lex.europa.eu/eli/reg/2023/1230/oj)
* [Konsolidierte Fassung vom 27.07.2026](https://eur-lex.europa.eu/legal-content/DE/TXT/?uri=CELEX:02023R1230-20260727) mit Berichtigung (ABl. L 169 vom 04.07.2023, S. 35) und den Änderungen durch die Verordnungen (EU) 2024/2748 und (EU) 2026/1744
* [Verordnung (EU) 2024/2847 (Cyberresilienz-Verordnung)](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32024R2847), Erwägungsgrund 53
* [Verordnung (EU) 2026/1744](https://eur-lex.europa.eu/eli/reg/2026/1744/oj) (Digital-Omnibus-Verordnung zur KI)
* Bei der letzten Prüfung (24.11.2026) nicht geprüft: Wortlaut der Notfallverfahren in Kapitel IVa, nationale Sanktionsregeln, Stand der delegierten Rechtsakte nach Art. 8 Unterabs. 3 und der harmonisierten Normen
