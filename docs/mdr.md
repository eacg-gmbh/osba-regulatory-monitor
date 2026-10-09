---
tags:
   - cybersecurity
   - security
   - safety
   - product safety
   - medical
---

# Medical Device Regulation (MDR)

Die Europäische Medizinprodukteverordnung (MDR), offiziell Verordnung (EU) 2017/745, ist der Rechtsrahmen für das Inverkehrbringen, die Bereitstellung auf dem Markt und die Inbetriebnahme von Medizinprodukten in der Europäischen Union ([Art. 1 Abs. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#art_1)). Sie hat die Richtlinien 90/385/EWG (aktive implantierbare Medizinprodukte) und 93/42/EWG (Medizinprodukte) abgelöst ([Art. 122](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_122)) und gilt als EU-Verordnung unmittelbar in allen Mitgliedstaaten. **Software kann selbst ein Medizinprodukt sein** ([Art. 2 Nr. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#art_2), [Erwägungsgrund 19](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#rct_19)). Damit gelten für Hersteller von Medizinprodukte-Software auch die Anforderungen an Software-Lebenszyklus und IT-Sicherheit aus Anhang I.

> [!NOTE]
>
> Alle Artikelverweise beziehen sich, sofern nicht anders angegeben, auf die [Verordnung (EU) 2017/745](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745) und führen direkt zum jeweiligen Artikel. Links auf Artikel, die durch Änderungsrechtsakte betroffen sind (u. a. Art. 10, 10a, 120, 123), führen zur [konsolidierten Fassung vom 10.01.2025](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110); die übrigen zum Amtsblatt-Text. Die Wortlaute wurden mit der konsolidierten deutschen Fassung vom 10.01.2025 (eine neuere konsolidierte Fassung wurde nicht gefunden) abgeglichen; Änderungsrechtsakte, Beschlüsse und Leitlinien stehen im Abschnitt [Quellen](#quellen). Stand: 09.10.2026. Die Seite ist eine Orientierung und keine Rechtsberatung.

## Überblick

* **Segment**: Medizin Produktsicherheit

* **Verabschiedet / Veröffentlicht**:
    * Verordnung (EU) 2017/745 vom 05.04.2017, veröffentlicht im Amtsblatt der EU (L 117) am 05.05.2017
    * Parallel: Verordnung (EU) 2017/746 über In-vitro-Diagnostika (IVDR), die nach [Art. 1 Abs. 6 lit. a](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#art_1) nicht von der MDR erfasst werden. Die Software- und Cybersicherheitsanforderungen sind dort vergleichbar aufgebaut; diese Seite behandelt nur die MDR.

* **Gültig ab** ([Art. 123](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_123)):
    * In Kraft getreten: 25.05.2017 (20. Tag nach Veröffentlichung, Abs. 1)
    * Anwendbar: **26.05.2021** (Abs. 2). Ursprünglich war der 26.05.2020 vorgesehen; die Verschiebung um ein Jahr erfolgte wegen COVID-19 durch die [Verordnung (EU) 2020/561](https://eur-lex.europa.eu/eli/reg/2020/561/oj).
    * Einzelne Vorschriften galten früher oder gelten später (z. B. Benannte Stellen ab 26.11.2017 nach Abs. 3 lit. a; EUDAMED-Pflichten stufenweise, siehe [EUDAMED und UDI](#eudamed-und-udi)).
    * Hinweis: Der 17.01.2023, der in früheren Fassungen dieser Seite genannt war, ist **kein** MDR-Datum.

* **Übergangsfristen für Altprodukte** ([Art. 120](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_120), geändert durch die [Verordnung (EU) 2023/607](https://eur-lex.europa.eu/eli/reg/2023/607/oj)):

    Produkte mit gültiger Bescheinigung nach der Richtlinie 90/385/EWG oder 93/42/EWG dürfen unter den Bedingungen des Abs. 3c noch in Verkehr gebracht oder in Betrieb genommen werden bis:

    | Datum | Produkte (Art. 120 Abs. 3a, 3b) |
    |-------|---------------------------------|
    | **31.12.2027** | alle Produkte der Klasse III und implantierbare Produkte der Klasse IIb (ausgenommen Nahtmaterial, Klammern, Zahnfüllungen, Zahnspangen, Zahnkronen, Schrauben, Keile, Zahn- bzw. Knochenplatten, Drähte, Stifte, Klemmen und Verbindungsstücke) |
    | **31.12.2028** | übrige Produkte der Klasse IIb, Klasse IIa sowie Klasse I in sterilem Zustand oder mit Messfunktion; außerdem Produkte, die nach der Richtlinie 93/42/EWG ohne Benannte Stelle konformitätsbewertet wurden (Eigenerklärung vor dem 26.05.2021) und nach der MDR eine Benannte Stelle benötigen |

    * Voraussetzungen ([Art. 120 Abs. 3c](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_120)): Produkt entspricht weiterhin den Richtlinien, keine wesentlichen Änderungen von Auslegung und Zweckbestimmung, kein unannehmbares Risiko, Qualitätsmanagementsystem nach Art. 10 Abs. 9 spätestens seit 26.05.2024, förmlicher Antrag bei einer Benannten Stelle bis 26.05.2024 und schriftliche Vereinbarung bis 26.09.2024.
    * Bereits in Verkehr gebrachte Produkte dürfen weiter bereitgestellt oder in Betrieb genommen werden ([Abs. 4](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_120); die frühere Abverkaufsfrist von einem Jahr ist entfallen).
    * Für diese Altprodukte gelten Überwachung nach dem Inverkehrbringen, Marktüberwachung, Vigilanz und Registrierung bereits nach der MDR ([Abs. 3d](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_120)).
    * **Software-Bezug**: Ein Update, das Auslegung oder Zweckbestimmung wesentlich verändert, kann den Altproduktstatus gefährden (Abs. 3c lit. b). Ob eine Änderung „wesentlich" ist, ist im Einzelfall zu prüfen (siehe MDCG-Leitlinien im Abschnitt [Lösungsansätze](#losungsansatze-hilfestellungen)).
    * Implantierbare Sonderanfertigungen der Klasse III durften nur bis 26.05.2026 ohne Bescheinigung in Verkehr gebracht werden ([Abs. 3f](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_120)); diese Frist ist abgelaufen.

* **Gültig für** ([Art. 1 Abs. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#art_1), [Art. 2 Nr. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#art_2)):
    * Hersteller von Medizinprodukten und Zubehör für den menschlichen Gebrauch, einschließlich **Software mit medizinischer Zweckbestimmung** (Diagnose, Verhütung, Überwachung, Vorhersage, Prognose, Behandlung oder Linderung von Krankheiten u. a.)
    * Bevollmächtigte, Importeure und Händler ([Art. 11 bis 14](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#art_11))
    * Ab Geltungsbeginn der Gemeinsamen Spezifikationen auch die Produktgruppen ohne medizinische Zweckbestimmung nach Anhang XVI ([Art. 1 Abs. 2](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#art_1))

* **Nicht gültig für**:
    * In-vitro-Diagnostika im Sinne der Verordnung (EU) 2017/746 ([Art. 1 Abs. 6 lit. a](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#art_1))
    * Software für allgemeine Zwecke, auch wenn sie in Einrichtungen des Gesundheitswesens eingesetzt wird, sowie Software für Lifestyle und Wohlbefinden ([Erwägungsgrund 19](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#rct_19)). Maßgeblich ist die vom Hersteller festgelegte Zweckbestimmung ([Art. 2 Nr. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#art_2)).
    * Produkte, die ausschließlich innerhalb von Gesundheitseinrichtungen in der Union hergestellt und verwendet werden, mit Ausnahme der Anforderungen aus Anhang I und unter weiteren Voraussetzungen ([Art. 5 Abs. 5](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_5))
    * Weitere Ausnahmen listet [Art. 1 Abs. 6](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#art_1) auf.

* **Grauzone**:
    * Qualifizierung von Software als Medizinprodukt (Zweckbestimmung, Abgrenzung zu Wellness- und Allzweck-Software). Hilfestellung: [MDCG 2019-11 Rev.1](#losungsansatze-hilfestellungen).
    * Verhältnis zu Cyber Resilience Act, NIS2 und AI Act (siehe [Wechselwirkungen](#wechselwirkungen-mit-anderen-eu-regularien)).
    * Der Status der Normen IEC 62304 und IEC 81001-5-1 als harmonisierte Normen (siehe [Normen](#normen-iec-62304-und-iec-81001-5-1)).
    * Die Revision von MDR und IVDR ist nur vorgeschlagen, nicht beschlossen (siehe [Revisionsvorschlag](#revisionsvorschlag-der-kommission)).

* **Ziel**:
  Ein hohes Gesundheitsschutzniveau für Patienten und Anwender bei gleichzeitigem Funktionieren des Binnenmarkts für Medizinprodukte ([Art. 1 Abs. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#art_1)). Gegenüber den Vorgängerrichtlinien schärft die MDR Klassifizierung, klinische Bewertung, Überwachung nach dem Inverkehrbringen und Rückverfolgbarkeit.

* **Neuerungen / Anforderungen**:
    * **Klassifizierung nach Risiko** in die Klassen I, IIa, IIb und III nach Anhang VIII ([Art. 51 Abs. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#art_51)). Für Software gilt insbesondere Regel 11 (siehe unten). Ob und welche Benannte Stelle beteiligt wird, richtet sich nach der Klasse ([Art. 52](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#art_52)).
    * **Risikomanagementsystem und Qualitätsmanagementsystem** als Herstellerpflichten ([Art. 10 Abs. 2 und 9](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_10)).
    * **Klinische Bewertung** und klinische Nachbeobachtung nach dem Inverkehrbringen ([Art. 10 Abs. 3](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_10), [Art. 61](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_61), Anhang XIV); für implantierbare Produkte und Produkte der Klasse III ein öffentlich zugänglicher Kurzbericht über Sicherheit und klinische Leistung ([Art. 32](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_32)).
    * **Überwachung nach dem Inverkehrbringen** und **Vigilanz** mit festen Meldefristen ([Art. 83 bis 92](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_83)).
    * **Eindeutige Produktidentifikation (UDI)** ([Art. 27](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#art_27)) und die **Europäische Datenbank für Medizinprodukte (EUDAMED)** ([Art. 33](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#art_33)).
    * **Benannte Stellen** mit strengeren Benennungs- und Überwachungsanforderungen ([Art. 35 bis 50](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#art_35)).
    * **Für die Einhaltung der Regulierungsvorschriften verantwortliche Person** (PRRC) in der Organisation des Herstellers ([Art. 15](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#art_15)).
    * **Ausreichende finanzielle Deckung** der potenziellen Haftung ([Art. 10 Abs. 16](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_10)).
    * **Pflichten bei Lieferunterbrechung oder -beendigung** bestimmter Produkte, in der Regel mindestens sechs Monate vorab ([Art. 10a](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_10a), eingefügt durch die [Verordnung (EU) 2024/1860](https://eur-lex.europa.eu/eli/reg/2024/1860/oj)).
    * **Sanktionen** legen die Mitgliedstaaten fest ([Art. 113](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#art_113)); in Deutschland ergänzt das [Medizinprodukterecht-Durchführungsgesetz (MPDG)](https://www.gesetze-im-internet.de/mpdg/) die Verordnung.

## Zentrale Forderungen

### Software und Cybersicherheit (Anhang I)

Die MDR enthält **keinen eigenen Cybersicherheitsabschnitt**. Cybersicherheit ist Teil der grundlegenden Sicherheits- und Leistungsanforderungen (GSPR) in [Anhang I](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#anx_I), die jedes Produkt erfüllen muss ([Art. 5 Abs. 2](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_5)). Die Nachweisführung läuft über das Risikomanagement und die technische Dokumentation (Anhänge II und III).

| Anforderung | Fundstelle | Inhalt |
|-------------|------------|--------|
| Sicherheit, Wirksamkeit, Stand der Technik | [Anhang I Kapitel I Nr. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#anx_I) | Produkte erzielen die vorgesehene Leistung und sind sicher und wirksam; der allgemein anerkannte Stand der Technik ist zugrunde zu legen |
| Risikomanagement über den Lebenszyklus | Anhang I Kapitel I Nr. 3 | kontinuierlicher iterativer Prozess über den gesamten Lebenszyklus, einschließlich Auswertung der Daten aus der Überwachung nach dem Inverkehrbringen |
| Rangfolge der Risikokontrolle | Anhang I Kapitel I Nr. 4 | sichere Auslegung vor Schutzmaßnahmen vor Information der Anwender |
| Wechselwirkung Software und IT-Umgebung | Anhang I Kapitel II Nr. 14.2 lit. d | Risiken durch negative Wechselwirkung zwischen Software und der IT-Umgebung, in der sie eingesetzt wird, sind auszuschließen oder so weit wie möglich zu reduzieren |
| Zuverlässigkeit programmierbarer Systeme und Software | Anhang I Kapitel II Nr. 17.1 | Wiederholbarkeit, Zuverlässigkeit und Leistung; Vorkehrungen für das Erstauftreten eines Defekts |
| Software-Lebenszyklus und Informationssicherheit | Anhang I Kapitel II Nr. 17.2 | Entwicklung nach dem Stand der Technik unter Berücksichtigung der Grundsätze des Software-Lebenszyklus, des Risikomanagements **einschließlich der Informationssicherheit**, der Verifizierung und der Validierung |
| Mobile Plattformen | Anhang I Kapitel II Nr. 17.3 | Berücksichtigung der Eigenschaften der mobilen Plattform und der äußeren Einflüsse |
| Mindestanforderungen an IT-Umgebung | Anhang I Kapitel II Nr. 17.4 | Hersteller legen Mindestanforderungen an Hardware, Eigenschaften von IT-Netzen und **IT-Sicherheitsmaßnahmen einschließlich des Schutzes vor unbefugtem Zugriff** fest |
| Schutz vor unbefugtem Zugriff (aktive Produkte) | Anhang I Kapitel II Nr. 18.8 | Produkte sind so weit wie möglich vor unbefugtem Zugriff geschützt, der das bestimmungsgemäße Funktionieren behindern könnte |
| Information an Anwender | Anhang I Kapitel III Nr. 23.4 lit. ab | Die Gebrauchsanweisung enthält die Mindestanforderungen an Hardware, IT-Netze und IT-Sicherheitsmaßnahmen einschließlich Schutz vor unbefugtem Zugriff |

* **Einordnung der Abschnitte 14.2 und 14.4**: Abschnitt 14.2 lit. d betrifft die Wechselwirkung zwischen Software und IT-Umgebung. Abschnitt 14.4 behandelt dagegen Einstellung, Kalibrierung und Instandhaltung und ist **kein** IT-Sicherheitsabschnitt. Die zentralen IT-Sicherheitsanforderungen stehen in den Abschnitten 17.2, 17.4, 18.8 und 23.4 lit. ab.
* Die MDR nennt keine konkreten technischen Maßnahmen (z. B. Verschlüsselung, SBOM, Schwachstellenmanagement) und keine feste Frist für Sicherheitsupdates. Diese Konkretisierung leisten Leitlinien und Normen (siehe unten).

### Klassifizierung von Software (Regel 11)

Software gilt als aktives Produkt ([Art. 2 Nr. 4](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#art_2)) und wird nach [Anhang VIII](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#anx_VIII) klassifiziert:

* **Durchführungsvorschrift 3.3**: Software, die ein Produkt steuert oder dessen Anwendung beeinflusst, wird derselben Klasse zugerechnet wie das Produkt. Unabhängige Software wird für sich allein klassifiziert.
* **Regel 11** (Kapitel III Nr. 6.3):
    * Software, die Informationen für Entscheidungen zu diagnostischen oder therapeutischen Zwecken liefert, gehört zur **Klasse IIa**, außer die Entscheidungen können
        * Tod oder eine irreversible Verschlechterung des Gesundheitszustands verursachen: **Klasse III**,
        * eine schwerwiegende Verschlechterung des Gesundheitszustands oder einen chirurgischen Eingriff verursachen: **Klasse IIb**.
    * Software zur Überwachung physiologischer Prozesse gehört zur **Klasse IIa**, bei der Kontrolle vitaler physiologischer Parameter, deren Änderung zu einer unmittelbaren Gefahr für den Patienten führen könnte, zur **Klasse IIb**.
    * Sämtliche andere Software gehört zur **Klasse I**.
* Folge: Software ab Klasse IIa benötigt in der Regel eine Benannte Stelle ([Art. 52 Abs. 4 und 6](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#art_52)); Klasse I wird durch die EU-Konformitätserklärung des Herstellers erklärt ([Art. 52 Abs. 7](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#art_52)). Das ist auch für den AI Act relevant (siehe unten).

### Herstellerpflichten ([Art. 10](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_10))

* Risikomanagementsystem nach Anhang I Abschnitt 3 (Abs. 2), klinische Bewertung (Abs. 3), technische Dokumentation nach Anhang II und III (Abs. 4), EU-Konformitätserklärung und CE-Kennzeichnung (Abs. 6)
* **Qualitätsmanagementsystem** (Abs. 9), das u. a. Produktrealisierung einschließlich Planung, Auslegung und Entwicklung (lit. g), Risikomanagement (lit. e), Überwachung nach dem Inverkehrbringen (lit. i), Vigilanzverfahren (lit. k) und die Auswahl und Kontrolle von Zulieferern und Unterauftragnehmern (lit. d) umfasst. Letzteres ist für zugekaufte Software und Open-Source-Komponenten relevant.
* Aufbewahrung der Dokumentation mindestens zehn Jahre, bei implantierbaren Produkten mindestens 15 Jahre nach Inverkehrbringen des letzten Produkts (Abs. 8)
* Sofortige **Korrekturmaßnahmen** bei Nichtkonformität (Abs. 12) und ein System für die Aufzeichnung und Meldung von Vorkommnissen (Abs. 13)

### Überwachung nach dem Inverkehrbringen ([Art. 83 bis 86](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_83))

* Pro Produkt ein System, das aktiv und systematisch Daten über Qualität, Leistung und Sicherheit während der gesamten Lebensdauer sammelt, aufzeichnet und analysiert ([Art. 83 Abs. 1 und 2](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_83)). Die Daten fließen u. a. in das Risikomanagement nach Anhang I Kapitel I ein (Abs. 3 lit. a). Für Software sind damit auch bekannt gewordene Schwachstellen und Sicherheitsvorfälle Gegenstand der Überwachung, soweit sie Sicherheit oder Leistung des Produkts betreffen.
* Plan zur Überwachung nach dem Inverkehrbringen als Teil der technischen Dokumentation ([Art. 84](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#art_84), Anhang III Abschnitt 1)
* Klasse I: Bericht über die Überwachung nach dem Inverkehrbringen ([Art. 85](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#art_85)); Klassen IIa, IIb und III: regelmäßig aktualisierter Sicherheitsbericht (PSUR), bei IIb und III mindestens jährlich, bei IIa bei Bedarf, mindestens alle zwei Jahre ([Art. 86 Abs. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_86))

### Vigilanz und Meldefristen ([Art. 87 bis 92](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_87))

Hersteller melden schwerwiegende Vorkommnisse und Sicherheitskorrekturmaßnahmen im Feld ([Art. 87 Abs. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_87)). Die Fristen gestaffelt nach Schwere:

| Fall | Frist | Fundstelle |
|------|-------|------------|
| Schwerwiegendes Vorkommnis (Regelfall) | unverzüglich nach Feststellung eines (möglichen) Kausalzusammenhangs, spätestens **15 Tage** nach Kenntnis | [Art. 87 Abs. 3](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_87) |
| Schwerwiegende Gefahr für die öffentliche Gesundheit | unverzüglich, spätestens **2 Tage** nach Kenntnis | Art. 87 Abs. 4 |
| Tod oder unvorhergesehene schwerwiegende Verschlechterung des Gesundheitszustands | unverzüglich, spätestens **10 Tage** nach Kenntnis | Art. 87 Abs. 5 |
| Sicherheitskorrekturmaßnahme im Feld | ohne ungebührliche Verzögerung **vor** Ergreifen der Maßnahme (außer in dringenden Fällen) | Art. 87 Abs. 8 |

* Bei Eilbedürftigkeit ist eine vorläufige Meldung mit nachfolgender vollständiger Meldung möglich (Abs. 6). Bei Unsicherheit, ob ein Vorkommnis meldepflichtig ist, wird fristgerecht gemeldet (Abs. 7).
* **Trendmeldung** bei statistisch signifikantem Anstieg nicht schwerwiegender Vorkommnisse ([Art. 88](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_88)); Untersuchung und Abschlussbericht ([Art. 89 Abs. 1 und 5](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_89)); Sicherheitsanweisung im Feld an die Anwender, mit UDI und SRN ([Art. 89 Abs. 8](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_89)).
* Die Meldung erfolgt über das elektronische System nach [Art. 92](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_92). Dessen Pflichten gelten erst sechs Monate nach der Kommissionsmitteilung, dass das Vigilanz-Modul funktionsfähig ist ([Art. 123 Abs. 3 lit. d](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_123)); bis dahin gelten die Vigilanzvorschriften der Richtlinien fort. Ob eine solche Mitteilung zum Vigilanz-Modul inzwischen veröffentlicht wurde, ist **nicht verifiziert** (siehe [EUDAMED und UDI](#eudamed-und-udi)).
* Die Meldefristen der MDR betreffen Vorkommnisse mit dem Produkt und sind getrennt von den Meldepflichten einer Einrichtung nach NIS2 zu sehen (siehe [Wechselwirkungen](#wechselwirkungen-mit-anderen-eu-regularien)).

### EUDAMED und UDI

* **UDI-System** ([Art. 27](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#art_27)): UDI-DI und UDI-PI (Abs. 1), Zuteilung vor Inverkehrbringen (Abs. 3), UDI-Träger auf Kennzeichnung und höheren Verpackungsebenen (Abs. 4), Basis-UDI-DI in der EU-Konformitätserklärung (Abs. 6). Staffelung der Kennzeichnungspflicht nach [Art. 123 Abs. 3 lit. f](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_123): implantierbare Produkte und Klasse III ab 26.05.2021, Klassen IIa und IIb ab 26.05.2023, Klasse I ab 26.05.2025.
* **UDI für Software** ([Anhang VI Teil C Nr. 6.5](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#anx_VI)): Die UDI wird auf Systemebene der Software zugeteilt. Die Software-Identifikation (Version) ist Teil der UDI-PI. Eine neue UDI-DI ist erforderlich, wenn sich ursprüngliche Leistung, Sicherheit oder bestimmungsgemäße Verwendung oder die Auswertung der Daten ändern. Geringfügige Änderungen (Fehlerbehebungen, Sicherheitspatches, Betriebseffizienz) erfordern eine neue UDI-PI, aber keine neue UDI-DI.
* **EUDAMED** ([Art. 33](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#art_33)): Die Pflichten zu den einzelnen elektronischen Systemen gelten gestaffelt, sechs Monate nach der Mitteilung der Kommission, dass das jeweilige System funktionsfähig ist ([Art. 123 Abs. 3 lit. d](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_123), neu gefasst durch die [Verordnung (EU) 2024/1860](https://eur-lex.europa.eu/eli/reg/2024/1860/oj)).
    * Mit dem [Beschluss (EU) 2025/2371](https://eur-lex.europa.eu/eli/dec/2025/2371/oj) (veröffentlicht am 27.11.2025) bestätigte die Kommission vier Systeme als funktionsfähig: Akteursregistrierung, UDI-Datenbank und Produktregistrierung, Benannte Stellen und Bescheinigungen sowie Marktüberwachung. Die Pflichten dazu gelten daher sechs Monate nach der Veröffentlichung, also seit Ende Mai 2026 (in Veröffentlichungen Dritter mit 28.05.2026 angegeben; das genaue Datum wurde nicht gegen eine Primärquelle verifiziert).
    * Die Registrierungspflicht der Hersteller für die Produktdaten gilt nach [Art. 123 Abs. 3 lit. e](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_123) spätestens 12 Monate nach der Veröffentlichung der Mitteilung (also bis Ende November 2026) für die dort genannten Produkte.
    * Die Systeme für Vigilanz und Überwachung nach dem Inverkehrbringen sowie für klinische Prüfungen waren nicht Teil dieses Beschlusses. Ob inzwischen weitere Mitteilungen ergangen sind, wurde hier nicht verifiziert.

### Wechselwirkungen mit anderen EU-Regularien

| Regelwerk | Verhältnis zur MDR |
|-----------|--------------------|
| **Cyber Resilience Act (CRA)** | Der CRA gilt **nicht** für Produkte mit digitalen Elementen, auf die die Verordnungen (EU) 2017/745 (MDR) oder 2017/746 (IVDR) Anwendung finden ([CRA Art. 2 Abs. 2 lit. a und b](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32024R2847#art_2)). Begründung: Die MDR/IVDR behandeln Cybersicherheit bereits über grundlegende Anforderungen und die Leitlinie MDCG 2019-16 ([CRA Erwägungsgrund 25](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32024R2847#rct_25)). Nicht erfasste Software (z. B. Allzweck-Software ohne medizinische Zweckbestimmung) kann dagegen unter den CRA fallen; wearables zur Gesundheitsüberwachung, die nicht unter MDR/IVDR fallen, nennt der CRA ausdrücklich in [Anhang III Klasse I Nr. 19](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32024R2847#anx_III). Siehe [CRA](cra.md). |
| **NIS2** | Hersteller von Medizinprodukten und In-vitro-Diagnostika sind Sektor „Verarbeitendes Gewerbe" in [Anhang II Nr. 5 lit. a](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#anx_II) der Richtlinie (EU) 2022/2555 und damit bei mindestens mittlerer Größe grundsätzlich **wichtige Einrichtungen** ([Art. 2 Abs. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_2), [Art. 3 Abs. 2](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_3)). Hersteller von Medizinprodukten, die in einer Notlage im Bereich der öffentlichen Gesundheit als kritisch gelistet sind, stehen zusätzlich in [Anhang I Nr. 5](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#anx_I) (Gesundheitswesen). NIS2 betrifft die Einrichtung (Risikomanagement, Meldepflichten), die MDR das Produkt. Siehe [NIS2](nis2.md). |
| **EU AI Act** | Medizinprodukte sind in [Anhang I Abschnitt A Nr. 11](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32024R1689#anx_I) (MDR) und Nr. 12 (IVDR) des AI Act aufgeführt. Ein KI-System ist hochriskant, wenn es Sicherheitsbauteil eines solchen Produkts oder selbst ein solches Produkt ist **und** das Produkt einer Konformitätsbewertung durch Dritte (Benannte Stelle) unterliegt ([Art. 6 Abs. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32024R1689#art_6)). KI-Software der MDR-Klasse I ohne Benannte Stelle erfüllt diese Voraussetzung nicht. Die Pflichten für diese Systeme gelten seit der Änderung durch die [Verordnung (EU) 2026/1744](https://eur-lex.europa.eu/eli/reg/2026/1744/oj) ab dem **02.08.2028** (ursprünglich 02.08.2027); die MDR selbst bleibt unverändert maßgeblich für das Produkt. Siehe [AI Act](aiact.md). |
| **Produkthaftung** | Hersteller haften für fehlerhafte Produkte nach Unionsrecht und nationalem Recht ([Art. 10 Abs. 16](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:02017R0745-20250110#art_10)). Siehe [PLD](pld.md). |

> [!NOTE]
>
> Die Verordnung (EU) 2026/1744 verschiebt Medizinprodukte **nicht** von Anhang I Abschnitt A nach Abschnitt B des AI Act (die geprüfte Fassung ändert die Liste in Anhang I nicht). Sie fügt aber einen neuen [Art. 2 Abs. 13](https://eur-lex.europa.eu/eli/reg/2026/1744/oj) in den AI Act ein: Für Hochrisiko-KI-Systeme nach Art. 6 Abs. 1 kann die Anwendung der Art. 9 bis 15 und 17 bis 25 beschränkt werden, soweit die Rechtsvorschriften nach Anhang I Abschnitt A (also auch die MDR) ein gleichwertiges oder höheres Schutzniveau bieten. Die Kommission soll dazu bis zum 02.08.2027 delegierte Rechtsakte erlassen. Solche Rechtsakte lagen nach den hier geprüften Quellen noch nicht vor.

### Normen: IEC 62304 und IEC 81001-5-1

* Harmonisierte Normen begründen die Konformitätsvermutung für die damit abgedeckten Anforderungen, auch für System- und Prozessanforderungen wie Qualitäts- und Risikomanagement ([Art. 8 Abs. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32017R0745#art_8)). Voraussetzung ist die Veröffentlichung der Fundstelle im Amtsblatt.
* [IEC 62304](iec62304.md) (Software-Lebenszyklus) und [IEC 81001-5-1](iec81001-5-1.md) (Cybersicherheit im Lebenszyklus von Gesundheitssoftware) sind in der konsolidierten Fassung (Stand 17.06.2026) des [Durchführungsbeschlusses (EU) 2021/1182](https://eur-lex.europa.eu/eli/dec_impl/2021/1182/oj) **nicht** gelistet. Sie begründen damit nach hier geprüftem Stand keine Konformitätsvermutung, sind aber als Stand der Technik für Anhang I Nr. 17.2 allgemein anerkannt. Neuere Beschlüsse nach dem 17.06.2026 wurden nicht geprüft.

### Revisionsvorschlag der Kommission

* Die Kommission hat am 16.12.2025 einen Vorschlag zur Vereinfachung von MDR und IVDR vorgelegt ([COM(2025) 1023](https://eur-lex.europa.eu/legal-content/DE/TXT/?uri=CELEX:52025PC1023), Verfahren [2025/0404(COD)](https://oeil.europarl.europa.eu/oeil/en/procedure-file?reference=2025/0404(COD))).
* Stand laut Legislative Observatory (abgerufen am 09.10.2026): Verfahren im Ausschuss (Ausschuss für öffentliche Gesundheit SANT, Berichterstatter Oliver Schenk), Verfahrensstufe „Awaiting committee decision", indikativer Termin für die Abstimmung im Plenum 14.12.2026. **Der Vorschlag ist nicht beschlossen** und hat keine Rechtswirkung. Die Inhalte dieser Seite beziehen sich weiter auf die geltende Verordnung.

## Lösungsansätze & Hilfestellungen

* Die EU-Kommission stellt Leitlinien und MDCG-Dokumente bereit: [MDCG Guidance](https://health.ec.europa.eu/medical-devices-sector/new-regulations/guidance-mdcg-endorsed-documents-and-other-guidance_en). Die Dokumente sind **nicht rechtsverbindlich**; verbindlich auslegen kann nur der Gerichtshof der Europäischen Union.
    * [MDCG 2019-16 Rev.1 „Guidance on Cybersecurity for medical devices"](https://health.ec.europa.eu/document/download/b23b362f-8a56-434c-922a-5b3ca4d0a7a1_en): Erstfassung Dezember 2019, Rev.1 Juli 2020. Nach dem Stand der MDCG-Übersicht (09.10.2026) ist Rev.1 die aktuelle Fassung. Das Dokument legt die Cybersicherheitsanforderungen aus Anhang I von MDR und IVDR aus (Abschnitt 1.3).
    * MDCG 2019-11 Rev.1 „Qualification and classification of software" (Juni 2025): Qualifizierung und Klassifizierung von Software nach MDR und IVDR (in der [MDCG-Übersicht](https://health.ec.europa.eu/medical-devices-sector/new-regulations/guidance-mdcg-endorsed-documents-and-other-guidance_en) aufgeführt)
    * [MDCG 2023-4](https://health.ec.europa.eu/document/download/b2c4e715-f2b4-4d24-af60-056b5d41a72e_en?filename=md_mdcg_2023-4_software_en.pdf) (Oktober 2023): Medical Device Software (MDSW) in Kombination mit Hardware
* Das BfArM (Bundesinstitut für Arzneimittel und Medizinprodukte) bietet nationale Informationen zu Medizinprodukten: [BfArM Medizinprodukte](https://www.bfarm.de/DE/Medizinprodukte/_node.html)
* Normen für Software und Cybersicherheit: [IEC 62304](iec62304.md), [IEC 81001-5-1](iec81001-5-1.md), ergänzend [IEC 62443](iec62443.md)
* [Verordnung (EU) 2017/745 im Volltext (EUR-Lex)](https://eur-lex.europa.eu/eli/reg/2017/745/oj)

### Tools & Werkzeuge

#### Software Lifecycle Management & Dokumentation (IEC 62304)

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [rdm (Regulatory Document Manager)](https://github.com/innolitics/rdm) | Open Source (MIT) | Dokumentation als Code: Markdown-Vorlagen und Python-Skripte erzeugen Dokumente für Medizinprodukte-Software (Word, PDF) aus einem Git-Repository; laut README besonders für Software nach IEC 62304 geeignet | Unterstützung bei IEC 62304-Dokumenten (Nachweis zu Anhang I Nr. 17.2). Die README nennt FDA-510(k)-Einreichungen; ein MDR-spezifischer Vorlagensatz (Anhang II/III) wird dort nicht belegt. Die Eignung für die technische Dokumentation nach MDR ist im Einzelfall zu prüfen. |

## Quellen

Alle Rechtstexte in der deutschen Fassung im Amtsblatt der EU (ELI-Links), Abgleich mit der konsolidierten Fassung vom 10.01.2025:

* [Verordnung (EU) 2017/745 (MDR)](https://eur-lex.europa.eu/eli/reg/2017/745/oj)
* [Verordnung (EU) 2017/746 (IVDR)](https://eur-lex.europa.eu/eli/reg/2017/746/oj)
* [Verordnung (EU) 2020/561](https://eur-lex.europa.eu/eli/reg/2020/561/oj): Verschiebung des Geltungsbeginns der MDR auf den 26.05.2021
* [Verordnung (EU) 2023/607](https://eur-lex.europa.eu/eli/reg/2023/607/oj): Verlängerung der Übergangsfristen (31.12.2027 / 31.12.2028)
* [Verordnung (EU) 2024/1860](https://eur-lex.europa.eu/eli/reg/2024/1860/oj): schrittweise Einführung von EUDAMED, Pflicht zur Information bei Lieferunterbrechung (Art. 10a)
* [Beschluss (EU) 2025/2371](https://eur-lex.europa.eu/eli/dec/2025/2371/oj): Funktionsfähigkeit der ersten vier EUDAMED-Systeme
* [Durchführungsbeschluss (EU) 2021/1182](https://eur-lex.europa.eu/eli/dec_impl/2021/1182/oj) in der Fassung vom 17.06.2026 (harmonisierte Normen zur MDR), geändert u. a. durch den [Durchführungsbeschluss (EU) 2026/1231](https://eur-lex.europa.eu/eli/dec_impl/2026/1231/oj)
* Für den Abschnitt „Wechselwirkungen": [CRA (EU) 2024/2847](https://eur-lex.europa.eu/eli/reg/2024/2847/oj), [NIS2 (EU) 2022/2555](https://eur-lex.europa.eu/eli/dir/2022/2555/oj), [AI Act (EU) 2024/1689](https://eur-lex.europa.eu/eli/reg/2024/1689/oj), [Digital-Omnibus-Verordnung zur KI (EU) 2026/1744](https://eur-lex.europa.eu/eli/reg/2026/1744/oj)
* [Vorschlag COM(2025) 1023](https://eur-lex.europa.eu/legal-content/DE/TXT/?uri=CELEX:52025PC1023) und [Verfahrensstand 2025/0404(COD) im Legislative Observatory](https://oeil.europarl.europa.eu/oeil/en/procedure-file?reference=2025/0404(COD))
* [MDCG-Leitlinien der Europäischen Kommission](https://health.ec.europa.eu/medical-devices-sector/new-regulations/guidance-mdcg-endorsed-documents-and-other-guidance_en), [MDCG 2019-16 Rev.1](https://health.ec.europa.eu/document/download/b23b362f-8a56-434c-922a-5b3ca4d0a7a1_en)
* [BfArM: Medizinprodukte](https://www.bfarm.de/DE/Medizinprodukte/_node.html), [Medizinprodukterecht-Durchführungsgesetz (MPDG)](https://www.gesetze-im-internet.de/mpdg/)
