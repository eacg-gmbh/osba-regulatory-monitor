---
tags:
   - cybersecurity
   - mobile 
---

# Radio Equipment Directive (RED)

Die Funkanlagenrichtlinie (Richtlinie 2014/53/EU, Radio Equipment Directive, RED) regelt die Bereitstellung von Funkanlagen auf dem Unionsmarkt und die Inbetriebnahme, also Geräte, die Funkwellen ausstrahlen oder empfangen, etwa Mobiltelefone, Smartwatches, Bluetooth- und WLAN-Geräte, Funkmäuse, Drohnen oder Spielzeug mit Funkfunktion. Cybersicherheitsanforderungen gelten dabei nicht pauschal, sondern über die [Delegierte Verordnung (EU) 2022/30](https://eur-lex.europa.eu/eli/reg_del/2022/30/oj) nur für bestimmte Kategorien von Funkanlagen. Diese Delegierte Verordnung wird zum 11.12.2027 durch die Delegierte Verordnung (EU) 2026/339 aufgehoben; danach gilt für die erfassten Produkte der [Cyber Resilience Act](cra.md).

> [!NOTE]
>
> Alle Artikelverweise beziehen sich, sofern nicht anders angegeben, auf die [Richtlinie 2014/53/EU](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053) und führen direkt zum jeweiligen Artikel. Die Delegierte Verordnung (EU) 2022/30 wird als „Delegierte VO 2022/30" bezeichnet. Die übrigen Rechtsakte und Quellen stehen im Abschnitt [Quellen](#quellen). Stand: 09.10.2026. Die Seite ist eine Orientierung und keine Rechtsberatung.

## Überblick

* **Segment**: IT Sicherheit / Produktregulierung (Funkanlagen)

* **Verabschiedet / Veröffentlicht**:
    * Richtlinie 2014/53/EU vom 16.04.2014, veröffentlicht im Amtsblatt der EU (L 153) am 22.05.2014; sie hebt die Richtlinie 1999/5/EG auf ([Art. 50](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_50))
    * Delegierte Verordnung (EU) 2022/30 vom 29.10.2021, veröffentlicht im Amtsblatt (L 7) am 12.01.2022; sie ergänzt die RED für Art. 3 Abs. 3 UAbs. 1 lit. d, e und f
    * Delegierte Verordnung (EU) 2023/2444 vom 20.07.2023, veröffentlicht am 27.10.2023: verschiebt den Anwendungsbeginn der Delegierten VO 2022/30 und berichtigt deren Art. 1 Abs. 2
    * Delegierte Verordnung (EU) 2026/339 vom 16.02.2026, veröffentlicht am 29.04.2026: hebt die Delegierte VO 2022/30 mit Wirkung vom 11.12.2027 auf

* **Gültig ab**:
    * Richtlinie: in Kraft getreten am 11.06.2014 (20. Tag nach Veröffentlichung, [Art. 51](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_51)); von den Mitgliedstaaten bis 12.06.2016 umzusetzen und ab 13.06.2016 anzuwenden ([Art. 49 Abs. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_49))
    * Delegierte VO 2022/30: in Kraft getreten am 01.02.2022 (20. Tag nach Veröffentlichung). **Anwendbar seit dem 01.08.2025.** Ursprünglich war der 01.08.2024 vorgesehen ([Art. 3](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022R0030#art_3)); die Delegierte VO 2023/2444 hat dies in [Art. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32023R2444#art_1) auf den 01.08.2025 verschoben, weil die harmonisierten Normen nicht rechtzeitig vorlagen (dort Erwägungsgründe 3 bis 5)
    * Ende der Anforderungen aus der Delegierten VO 2022/30: aufgehoben mit Wirkung vom **11.12.2027**, dem Tag des vollen Geltungsbeginns des CRA ([Delegierte VO 2026/339, Art. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32026R0339#art_1); CRA: [Art. 71 Abs. 2](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32024R2847#art_71)). Die Überwachung von Funkanlagen, die zwischen dem 01.08.2025 und dem 10.12.2027 in Verkehr gebracht wurden bzw. werden, bleibt unberührt (Erwägungsgrund 5 der Delegierten VO 2026/339)

* **Gültig für**:

    Funkanlagen, also elektrische oder elektronische Erzeugnisse, die zum Zweck der Funkkommunikation oder Funkortung bestimmungsgemäß Funkwellen ausstrahlen oder empfangen, einschließlich Erzeugnissen, die dafür Zubehör wie eine Antenne benötigen ([Art. 2 Abs. 1 Nr. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_2)). Adressaten sind Hersteller, Bevollmächtigte, Einführer und Händler ([Art. 2 Abs. 1 Nr. 12 bis 16](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_2)). Die **Cybersicherheitsanforderungen** (Art. 3 Abs. 3 UAbs. 1 lit. d, e, f) gelten nach der Delegierten VO 2022/30 nur für ([Art. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022R0030#art_1)):

    * **lit. d (Netzschutz)**: alle Funkanlagen, die selbst über das Internet kommunizieren können, direkt oder über andere Geräte („mit dem Internet verbundene Funkanlagen", Abs. 1)
    * **lit. e (Datenschutz und Privatsphäre)**, sofern die Anlage personenbezogene Daten, Verkehrs- oder Standortdaten verarbeiten kann (Abs. 2): mit dem Internet verbundene Funkanlagen, Funkanlagen ausschließlich für die Kinderbetreuung, Funkanlagen im Anwendungsbereich der Spielzeugrichtlinie 2009/48/EG sowie am Körper oder an Kleidung getragene Funkanlagen („tragbare Funkanlagen", z. B. Smartwatches, Kopfhörer). Kinderbetreuungs-, Spielzeug- und tragbare Funkanlagen sind auch ohne Internetverbindung erfasst (Erwägungsgrund 12)
    * **lit. f (Betrugsschutz)**: mit dem Internet verbundene Funkanlagen, die dem Besitzer oder Nutzer Übertragungen von Geld, monetären Werten oder virtuellen Währungen ermöglichen (Abs. 3)

    Die Anforderungen beziehen sich auf alle Aspekte und Teile der Anlage, nicht nur auf die funkbasierten Funktionen, also auch auf Software und Firmware (Erwägungsgrund 8 der Delegierten VO 2022/30).

* **Nicht gültig für**:
    * Die Richtlinie gilt nicht für die in [Anhang I](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#anx_I) genannten Geräte (u. a. Funkanlagen von Funkamateuren, die nicht auf dem Markt bereitgestellt werden, Schiffsausrüstung nach Richtlinie 96/98/EG, bestimmte Luftfahrtausrüstung, kundenspezifische Erprobungsmodule für Forschung und Entwicklung) sowie nicht für Funkanlagen, die ausschließlich für Tätigkeiten der öffentlichen Sicherheit, der Verteidigung, der Staatssicherheit oder im strafrechtlichen Bereich genutzt werden ([Art. 1 Abs. 2 und 3](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_1))
    * Die Cybersicherheitsanforderungen der Delegierten VO 2022/30 gelten ausnahmsweise nicht für Funkanlagen, die auch unter die Medizinprodukte-Verordnung (EU) 2017/745 oder die IVD-Verordnung (EU) 2017/746 fallen (lit. d, e, f). Für lit. e und f gilt zusätzlich eine Ausnahme bei Anwendbarkeit der Verordnung (EU) 2018/1139 (Luftfahrt), der Verordnung (EU) 2019/2144 (Typgenehmigung Kraftfahrzeuge) oder der Richtlinie (EU) 2019/520 (Mautsysteme) ([Art. 2](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022R0030#art_2))
    * Funkanlagen, die nicht in einer der oben genannten Kategorien der Delegierten VO 2022/30 liegen (z. B. nicht internetfähige, nicht tragbare Funkgeräte), unterliegen keiner Cybersicherheitsanforderung aus der RED

* **Grauzone**:
    * **Verhältnis zum CRA**: Der CRA nimmt Funkanlagen nicht generell aus; die Ausnahmen in [Art. 2 Abs. 2 bis 4](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32024R2847#art_2) nennen die RED nicht. Die RED-Cybersicherheitsanforderungen werden stattdessen durch Aufhebung der Delegierten VO 2022/30 abgelöst. Für Produkte, die in der Übergangszeit (01.08.2025 bis 10.12.2027) in Verkehr gebracht werden, gilt weiterhin die RED. Ob ein Produkt vor dem 11.12.2027 in Verkehr gebracht wurde, entscheidet über das anwendbare Regime. Für spätere wesentliche Änderungen siehe [Art. 69 Abs. 2](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32024R2847#art_69)
    * **Art. 3 Abs. 3 lit. i und Art. 4** (Software-Konformität bei Funkanlagen): Beide Vorschriften wirken nur, wenn die Kommission per delegiertem Rechtsakt Kategorien festlegt ([Art. 3 Abs. 3 UAbs. 2](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_3), [Art. 4 Abs. 2](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_4)). Nach Angaben der Kommission wurde die Initiative am 20.01.2026 aufgegeben, weil es an Belegen für einen Regelungsbedarf fehle ([Kommissionsseite zur RED](https://single-market-economy.ec.europa.eu/sectors/electrical-and-electronic-engineering-industries-eei/radio-equipment-directive-red_en)). Die Vorschriften bleiben im Richtlinientext, haben aber derzeit keine konkretisierte Wirkung (Schlussfolgerung aus dem Normtext)
    * **Harmonisierte Normen mit Einschränkungen**: EN 18031-1/-2/-3 begründen nur teilweise die Konformitätsvermutung (siehe unten). Die Frage, wann die Notifizierte-Stelle-Route zwingend ist, ist im Einzelfall zu prüfen
    * **Nationale Umsetzung**: Die RED ist eine Richtlinie und wirkt nicht unmittelbar gegenüber Herstellern, sondern über nationales Recht (siehe unten). Die Delegierte VO 2022/30 und ihre Aufhebung sind dagegen Verordnungen und gelten unmittelbar

* **Ziel**:
  Ein Regelungsrahmen für die Bereitstellung auf dem Markt und die Inbetriebnahme von Funkanlagen ([Art. 1 Abs. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_1)) mit Anforderungen an Gesundheit und Sicherheit, elektromagnetische Verträglichkeit ([Art. 3 Abs. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_3)) und effiziente Nutzung des Funkspektrums ([Art. 3 Abs. 2](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_3)). Mit der Delegierten VO 2022/30 sollen zusätzlich Risiken für Netze, personenbezogene Daten, Privatsphäre und Betrugsschutz bei vernetzten Funkanlagen adressiert werden (Erwägungsgründe 1, 7 und 9 bis 14 der Delegierten VO 2022/30).

* **Neuerungen / Anforderungen**:
    * Cybersicherheitsanforderungen für bestimmte Funkanlagen seit 01.08.2025 ([Art. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022R0030#art_1)), siehe „Gültig für"
    * Konformitätsbewertung, EU-Konformitätserklärung und CE-Kennzeichnung ([Art. 10 Abs. 3](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_10), [Art. 17](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_17), [Art. 18](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_18))
    * Harmonisierte Normen EN 18031-1/-2/-3 sind seit Januar 2025 mit Einschränkungen im Amtsblatt zitiert
    * Ablösung der Cybersicherheitsanforderungen durch den CRA zum 11.12.2027

## Zentrale Forderungen

* **Wesentliche Anforderungen** ([Art. 3](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_3)):

    Funkanlagen müssen durch ihr Baumuster Gesundheit und Sicherheit sowie elektromagnetische Verträglichkeit gewährleisten (Abs. 1) und das Funkspektrum effektiv nutzen (Abs. 2). In bestimmten Kategorien oder Klassen gelten zusätzliche Anforderungen (Abs. 3), deren Betroffene die Kommission per delegiertem Rechtsakt festlegt:

    * lit. d: keine schädlichen Auswirkungen auf das Netz oder seinen Betrieb, keine missbräuchliche Nutzung von Netzressourcen mit unannehmbarer Dienstbeeinträchtigung
    * lit. e: Sicherheitsvorrichtungen, die personenbezogene Daten und die Privatsphäre von Nutzer und Teilnehmer schützen
    * lit. f: Unterstützung bestimmter Funktionen zum Schutz vor Betrug
    * lit. a bis c sowie g bis i behandeln u. a. Zubehör, Interoperabilität, Zugang zu Rettungsdiensten, Barrierefreiheit und Software (lit. i). Auch sie gelten nur für Kategorien, die ein delegierter Rechtsakt festlegt; für lit. i ist dies nicht erfolgt (siehe Grauzone). Zu lit. g und h wurde der Stand nicht geprüft; lit. a wurde durch eine spätere Richtlinienänderung (Ladegeräte, vgl. § 4 Abs. 3 Nr. 1 FuAG mit Verweis auf Anhang Ia) ergänzt, die in dieser Seite nicht behandelt wird

* **Pflichten der Hersteller** ([Art. 10](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_10)):

    * Entwurf und Herstellung nach den wesentlichen Anforderungen (Abs. 1), technische Unterlagen nach [Art. 21](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_21) und Konformitätsbewertungsverfahren nach [Art. 17](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_17) (Abs. 3), EU-Konformitätserklärung und CE-Zeichen (Abs. 3)
    * Aufbewahrung von technischen Unterlagen und Konformitätserklärung für zehn Jahre ab Inverkehrbringen (Abs. 4)
    * Konformität in der Serienfertigung; Änderungen des Entwurfs, der Merkmale oder der angewandten Normen sind zu berücksichtigen (Abs. 5)
    * Gebrauchsanleitung und Sicherheitsinformationen, gegebenenfalls einschließlich der Beschreibung von Zubehör und Bestandteilen **inklusive Software**, die den bestimmungsgemäßen Betrieb ermöglichen (Abs. 8)
    * Unverzügliche Korrekturmaßnahmen bei erkannter Nichtkonformität und Information der Behörden bei Gefahr (Abs. 11)
    * Einführer und Händler gelten als Hersteller, wenn sie unter eigenem Namen vermarkten oder eine Funkanlage so verändern, dass die Konformität beeinträchtigt werden kann ([Art. 14](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_14)); Pflichten von Einführern und Händlern: [Art. 12](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_12), [Art. 13](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_13)

* **Konformitätsvermutung und Konformitätsbewertung** ([Art. 16](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_16), [Art. 17](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_17)):

    Entspricht eine Funkanlage harmonisierten Normen, deren Fundstellen im Amtsblatt veröffentlicht sind, wird Konformität mit den davon abgedeckten wesentlichen Anforderungen vermutet (Art. 16). Die Anwendung der Normen ist freiwillig (Erwägungsgrund 5 der Delegierten VO 2023/2444).

    * Wurden veröffentlichte harmonisierte Normen für Art. 3 Abs. 2 und 3 angewandt, genügt die interne Fertigungskontrolle ([Anhang II](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#anx_II)); alternativ EU-Baumusterprüfung ([Anhang III](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#anx_III)) oder umfassende Qualitätssicherung ([Anhang IV](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#anx_IV)) (Art. 17 Abs. 3)
    * Wurden solche Normen nicht oder nur teilweise angewandt oder gibt es sie nicht, ist eines der Verfahren nach Anhang III oder IV erforderlich, also unter Einbindung einer **Benannten (notifizierten) Stelle** (Art. 17 Abs. 4)
    * Wenn eine Funkanlage in unterschiedlichen Konfigurationen betrieben werden kann, ist die Konformität in allen möglichen Konfigurationen zu prüfen (Art. 17 Abs. 1)
    * Die technischen Unterlagen enthalten u. a. die **Software- oder Firmwareversionen**, durch die die Erfüllung der wesentlichen Anforderungen beeinflusst wird ([Anhang V](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#anx_V) lit. a Ziff. ii)

* **Rolle der Benannten Stellen** ([Art. 22 bis 38](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_22)):

    Die Mitgliedstaaten notifizieren Konformitätsbewertungsstellen, die als unabhängige Dritte tätig werden dürfen ([Art. 22](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_22)). Benannte Stellen sind nur dann einzubinden, wenn der Hersteller ein Verfahren nach Anhang III oder IV wählt oder wählen muss (Art. 17 Abs. 3 und 4). Bei Anhang IV folgt auf das CE-Zeichen die Kennnummer der Benannten Stelle ([Art. 20 Abs. 3](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_20)). Die Kommission führt die [Liste der Benannten Stellen für die RED](https://webgate.ec.europa.eu/single-market-compliance-space/notified-bodies/notified-body-list?filter=legislationId:154428,notificationStatusId:1). Nach dem Durchführungsbeschluss (EU) 2025/138 sind die Normen EN 18031 in bestimmten Konstellationen nicht ausreichend (siehe unten); dann bleibt nach Art. 17 Abs. 4 nur Anhang III oder IV (Schlussfolgerung).

* **Harmonisierte Normen EN 18031-1/-2/-3 und Amtsblatt** :

    Auf Basis des Normungsauftrags C(2022) 5637 vom 05.08.2022 (zitiert in Erwägungsgrund 3 der Delegierten VO 2023/2444) haben CEN und CENELEC die Normen erarbeitet. Die Kommission hat die Fundstellen mit dem [Durchführungsbeschluss (EU) 2025/138](https://eur-lex.europa.eu/eli/dec_impl/2025/138/oj) vom 28.01.2025 (veröffentlicht am 30.01.2025, in Kraft am Tag der Veröffentlichung) in Anhang I des [Durchführungsbeschlusses (EU) 2022/2191](https://eur-lex.europa.eu/eli/dec_impl/2022/2191/oj) aufgenommen, **mit Einschränkungen**:

    | Norm | Unterstützt | Einschränkungen (Konformitätsvermutung entfällt) |
    |------|-------------|--------------------------------------------------|
    | EN 18031-1:2024 | Art. 3 Abs. 3 UAbs. 1 lit. d (Funkanlagen mit Internetanschluss) | Abschnitte „rationale" und „guidance"; wenn nach Nr. 6.2.5.1 und 6.2.5.2 dem Nutzer erlaubt ist, kein Passwort festzulegen oder zu verwenden |
    | EN 18031-2:2024 | lit. e (Datenschutz und Privatsphäre; internetfähige, Kinderbetreuungs-, Spielzeug- und tragbare Funkanlagen) | wie oben; zusätzlich für Spielzeug- und Kinderbetreuungsfunkanlagen (Nr. 6.1.3 bis 6.1.6), wenn die Zugangssteuerung durch Eltern oder Erziehungsberechtigte nicht gewährleistet ist |
    | EN 18031-3:2024 | lit. f (Funkanlagen, die virtuelles Geld oder Geldwerte verarbeiten) | wie oben; die Beurteilungskriterien für **sichere Aktualisierungen** (Nr. 6.3.2.4) begründen generell keine Konformitätsvermutung |

    Die Normen selbst sind kostenpflichtig über die nationalen Normungsorganisationen erhältlich; hier werden daher nur die Amtsblatt-Fundstellen verlinkt. Der Durchführungsbeschluss 2022/2191 wurde seither mehrfach geändert, zuletzt (laut Kommissionsseite zu harmonisierten Normen für Funkanlagen) durch den Durchführungsbeschluss (EU) 2026/2003; die geprüften Änderungen 2025/893 und 2026/2003 enthalten keine Verweise auf EN 18031. Ob die Fundstellen nach dem 11.12.2027 gestrichen werden, ist nicht belegt.

* **Relevanz für Software, Firmware und Open Source**:

    * Die Delegierte VO 2022/30 erfasst die gesamte Funkanlage einschließlich nicht funkbezogener Funktionen (Erwägungsgrund 8); Firmware und Software des Geräts sind damit Teil der Konformitätsbewertung. Erwägungsgrund 10 nennt als Risiken u. a. Standardpasswörter, fehlende Verschlüsselung und fehlende starke Authentifizierung
    * Die RED verlangt, dass das Laden von Software die Konformität nicht beeinträchtigen darf (Erwägungsgrund 16); eine verbindliche Anforderung dazu (Art. 3 Abs. 3 lit. i) ist nicht aktiviert (siehe Grauzone). In den technischen Unterlagen sind konformitätsrelevante Software- und Firmwareversionen anzugeben (Anhang V)
    * EN 18031-3 schließt für Anwendungen mit Geldwerten die pauschale Konformitätsvermutung für sichere Updates aus (Nr. 6.3.2.4); dort sind daher ergänzende Nachweise erforderlich
    * Die RED enthält keine eigenen Vorschriften zu Open-Source-Software oder zu SBOMs. Verantwortlich ist der Hersteller der Funkanlage für das Gesamtprodukt; Komponenten Dritter, auch Open Source, liegen in seiner Verantwortung. Der CRA enthält mit [Art. 13 Abs. 5](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32024R2847#art_13) und Anhang I konkretere Vorgaben, siehe [CRA](cra.md)

* **Marktüberwachung und Sanktionen** ([Art. 39](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_39), [Art. 40](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_40), [Art. 46](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_46)):

    Marktüberwachung nach der Verordnung (EG) Nr. 765/2008; bei Verdacht auf Nichtkonformität fordern die Behörden Korrekturmaßnahmen, Rücknahme oder Rückruf. Die Mitgliedstaaten legen wirksame, verhältnismäßige und abschreckende Sanktionen fest (Art. 46).

* **Umsetzung in Deutschland (Richtlinie)**:

    Die RED ist eine Richtlinie und musste bis 12.06.2016 umgesetzt werden ([Art. 49](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_49)). In Deutschland erfolgte dies durch das [Funkanlagengesetz (FuAG)](https://www.gesetze-im-internet.de/fuag/). Die grundlegenden Anforderungen stehen in [§ 4 FuAG](https://www.gesetze-im-internet.de/fuag/__4.html), und zwar auch mit Verweis auf delegierte Rechtsakte nach Art. 44 der Richtlinie. Zuständig für Ausführung und Überwachung ist die Bundesnetzagentur ([§ 23 FuAG](https://www.gesetze-im-internet.de/fuag/__23.html)).

### Verhältnis zum Cyber Resilience Act (CRA)

* Die grundlegenden Cybersicherheitsanforderungen des CRA (Anhang I) umfassen nach Erwägungsgrund 30 des CRA alle Elemente der Anforderungen aus Art. 3 Abs. 3 lit. d, e und f RED. Dieselbe Aussage trifft Erwägungsgrund 3 der Delegierten VO 2026/339
* **Zeitliche Abgrenzung**:
    * Bis 10.12.2027 in Verkehr gebrachte Funkanlagen im Anwendungsbereich der Delegierten VO 2022/30 unterliegen den RED-Cybersicherheitsanforderungen (Anwendung seit 01.08.2025); der CRA gilt für vor dem 11.12.2027 in Verkehr gebrachte Produkte nur bei wesentlicher Änderung ([Art. 69 Abs. 2](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32024R2847#art_69))
    * Die **Meldepflichten** des CRA ([Art. 14](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32024R2847#art_14)) gelten seit dem 11.09.2026 auch für Altprodukte ([Art. 69 Abs. 3](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32024R2847#art_69), [Art. 71 Abs. 2](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32024R2847#art_71))
    * Ab 11.12.2027 ist die Delegierte VO 2022/30 aufgehoben (Delegierte VO 2026/339, Art. 1) und der CRA gilt vollumfänglich ([Art. 71 Abs. 2](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32024R2847#art_71)); die übrigen RED-Anforderungen (Gesundheit, EMV, Funkspektrum, CE) bleiben bestehen
    * Bereits ausgestellte EU-Baumusterprüfbescheinigungen zu Cybersicherheitsanforderungen aus anderen Harmonisierungsvorschriften bleiben bis 11.06.2028 gültig, sofern sie nicht früher ablaufen ([Art. 69 Abs. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32024R2847#art_69))
* **Benannte Stellen**: Stellen, die z. B. nach der Delegierten VO 2022/30 notifiziert wurden, müssen im Rahmen des CRA neu bewertet und notifiziert werden, wobei Synergien genutzt werden können (Erwägungsgrund 31 des CRA)
* **Normung**: Die Kommission und die europäischen Normungsorganisationen sollen die Arbeiten zum Normungsauftrag C(2022) 5637 berücksichtigen (Erwägungsgrund 30 des CRA). Der CRA verpflichtet die Kommission zudem, in der Übergangszeit Leitlinien für Hersteller zu geben, die sowohl dem CRA als auch der Delegierten VO 2022/30 unterliegen (Erwägungsgrund 30 des CRA)

### Zeitplan

| Datum | Meilenstein |
|-------|-------------|
| 22.05.2014 | Veröffentlichung der [Richtlinie 2014/53/EU](https://eur-lex.europa.eu/eli/dir/2014/53/oj) |
| 12.06.2016 / 13.06.2016 | Ende der Umsetzungsfrist / Anwendung der nationalen Vorschriften ([Art. 49](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32014L0053#art_49)) |
| 12.01.2022 | Veröffentlichung der [Delegierten VO 2022/30](https://eur-lex.europa.eu/eli/reg_del/2022/30/oj) |
| 27.10.2023 | Veröffentlichung der [Delegierten VO 2023/2444](https://eur-lex.europa.eu/eli/reg_del/2023/2444/oj) (Anwendungsbeginn auf 01.08.2025 verschoben) |
| 30.01.2025 | Veröffentlichung des [Durchführungsbeschlusses (EU) 2025/138](https://eur-lex.europa.eu/eli/dec_impl/2025/138/oj) (Fundstellen EN 18031-1/-2/-3 mit Einschränkungen) |
| 01.08.2025 | Anwendungsbeginn der Delegierten VO 2022/30 |
| 20.01.2026 | Die Kommission gibt die Initiative zu Art. 3 Abs. 3 lit. i und Art. 4 auf (Angabe der Kommission) |
| 29.04.2026 | Veröffentlichung der [Delegierten VO (EU) 2026/339](https://eur-lex.europa.eu/eli/reg_del/2026/339/oj) (Aufhebung der Delegierten VO 2022/30) |
| 11.09.2026 | CRA: Meldepflichten nach Art. 14 gelten |
| 11.12.2027 | Aufhebung der Delegierten VO 2022/30 wirksam; CRA gilt vollumfänglich |

## Lösungsansätze & Hilfestellungen

* [Richtlinie 2014/53/EU im Volltext (EUR-Lex)](https://eur-lex.europa.eu/eli/dir/2014/53/oj) und [Delegierte VO 2022/30 im Volltext (EUR-Lex)](https://eur-lex.europa.eu/eli/reg_del/2022/30/oj)
* Die Kommission stellt den [RED Guide](https://single-market-economy.ec.europa.eu/document/download/a0c7e4c5-27db-4c59-9c43-a380ed21563f_en?filename=RED%20Guide%20-%20version%2007.07.2026%20-%20with%20COVER.pdf) (Version 07.07.2026, laut Kommission ohne Rechtsverbindlichkeit) und weitere Leitfäden auf ihrer [Seite zur RED](https://single-market-economy.ec.europa.eu/sectors/electrical-and-electronic-engineering-industries-eei/radio-equipment-directive-red_en) bereit
* Aktueller Stand harmonisierter Normen: [Kommissionsseite zu harmonisierten Normen für Funkanlagen](https://single-market-economy.ec.europa.eu/single-market/goods/european-standards/harmonised-standards/radio-equipment_en)
* Vorgehen für Hersteller: (1) prüfen, ob die Funkanlage in eine Kategorie nach [Art. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022R0030#art_1) fällt und keine Ausnahme nach [Art. 2](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022R0030#art_2) greift; (2) EN 18031-1/-2/-3 anwenden und prüfen, ob eine der Einschränkungen aus dem Durchführungsbeschluss 2025/138 zutrifft; (3) andernfalls Verfahren nach Anhang III oder IV mit Benannter Stelle; (4) für Produkte mit Markteinführung nach dem 10.12.2027 den CRA vorbereiten, siehe [CRA](cra.md)
* Die TR-03183 des BSI zu SBOMs ist für die RED nicht vorgesehen; zur Einordnung siehe [CRA](cra.md#bsi-tr-03183-technische-richtlinie-des-bsi)

## Quellen

Alle Rechtstexte in der deutschen Fassung im Amtsblatt der EU (ELI-Links):

* [Richtlinie 2014/53/EU (RED)](https://eur-lex.europa.eu/eli/dir/2014/53/oj)
* [Delegierte Verordnung (EU) 2022/30](https://eur-lex.europa.eu/eli/reg_del/2022/30/oj): Anwendung der wesentlichen Anforderungen nach Art. 3 Abs. 3 lit. d, e, f
* [Delegierte Verordnung (EU) 2023/2444](https://eur-lex.europa.eu/eli/reg_del/2023/2444/oj): Verschiebung des Anwendungsbeginns auf 01.08.2025
* [Delegierte Verordnung (EU) 2026/339](https://eur-lex.europa.eu/eli/reg_del/2026/339/oj): Aufhebung der Delegierten VO 2022/30 mit Wirkung vom 11.12.2027
* [Durchführungsbeschluss (EU) 2025/138](https://eur-lex.europa.eu/eli/dec_impl/2025/138/oj): Fundstellen EN 18031-1/-2/-3 mit Einschränkungen
* [Durchführungsbeschluss (EU) 2022/2191](https://eur-lex.europa.eu/eli/dec_impl/2022/2191/oj): harmonisierte Normen für Funkanlagen (Grundakt)
* [Verordnung (EU) 2024/2847 (CRA)](https://eur-lex.europa.eu/eli/reg/2024/2847/oj)
* [Kommission: Seite zur RED](https://single-market-economy.ec.europa.eu/sectors/electrical-and-electronic-engineering-industries-eei/radio-equipment-directive-red_en), [RED Guide](https://single-market-economy.ec.europa.eu/document/download/a0c7e4c5-27db-4c59-9c43-a380ed21563f_en?filename=RED%20Guide%20-%20version%2007.07.2026%20-%20with%20COVER.pdf), [harmonisierte Normen für Funkanlagen](https://single-market-economy.ec.europa.eu/single-market/goods/european-standards/harmonised-standards/radio-equipment_en), [Liste der Benannten Stellen](https://webgate.ec.europa.eu/single-market-compliance-space/notified-bodies/notified-body-list?filter=legislationId:154428,notificationStatusId:1)
* [Funkanlagengesetz (FuAG)](https://www.gesetze-im-internet.de/fuag/)
