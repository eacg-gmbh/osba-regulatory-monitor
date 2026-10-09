---
tags:
   - cybersecurity
   - saas
   - kritis
---

# EU Network & Information Security Directive v2 (NIS2)

Die Richtlinie (EU) 2022/2555 über Maßnahmen für ein hohes gemeinsames Cybersicherheitsniveau in der Union (NIS2) ersetzt die ursprüngliche NIS-Richtlinie (EU) 2016/1148 ([Art. 44](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_44)). Sie verpflichtet "wesentliche" und "wichtige" Einrichtungen aus den Sektoren der Anhänge I und II zu Risikomanagementmaßnahmen im Bereich der Cybersicherheit, zu Meldepflichten bei erheblichen Sicherheitsvorfällen und verpflichtet die Mitgliedstaaten zu Aufsicht und Durchsetzung ([Art. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_1)). Als EU-Richtlinie gilt sie nicht unmittelbar, sondern wirkt über die nationale Umsetzung (in Deutschland das BSI-Gesetz, BSIG).

> [!NOTE]
>
> Alle Artikelverweise ("Art.") beziehen sich, sofern nicht anders angegeben, auf die [Richtlinie (EU) 2022/2555](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555) und führen direkt zum jeweiligen Artikel. Verweise mit "§" beziehen sich auf das deutsche [BSI-Gesetz (BSIG)](https://www.gesetze-im-internet.de/bsig_2025/BJNR12D0B0025.html). Die Seite ist eine Orientierungshilfe und keine Rechtsberatung. Alle Quellen stehen im Abschnitt [Quellen](#quellen).

## Überblick

* **Segment**: IT Sicherheit / Betreiber kritischer und sonstiger wichtiger Dienste (Sektoren nach Anhang I und II, darunter Anbieter digitaler Infrastruktur und IKT-Dienste)

* **Verabschiedet / Veröffentlicht**:
    * Richtlinie (EU) 2022/2555 vom 14.12.2022, veröffentlicht im Amtsblatt der EU (L 333) am 27.12.2022

* **Gültig ab**:
    * In Kraft getreten: 16.01.2023 (20. Tag nach Veröffentlichung, [Art. 45](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_45))
    * Umsetzungsfrist der Mitgliedstaaten: 17.10.2024; die nationalen Vorschriften sind ab dem 18.10.2024 anzuwenden ([Art. 41 Abs. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_41)). Mit Wirkung vom 18.10.2024 ist die NIS-Richtlinie aufgehoben ([Art. 44](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_44)).
    * Deutschland: Das NIS-2-Umsetzungs- und Cybersicherheitsstärkungsgesetz hat das BSI-Gesetz neu gefasst (Ausfertigung 02.12.2025, verkündet in [BGBl. 2025 I Nr. 301](https://www.recht.bund.de/bgbl/1/2025/301/VO.html) am 05.12.2025). Es ist am 06.12.2025 in Kraft getreten (Art. 30 des Gesetzes, laut Fußnote im [BSIG](https://www.gesetze-im-internet.de/bsig_2025/BJNR12D0B0025.html)). Die Registrierungspflicht beim BSI besteht spätestens drei Monate, nachdem eine Einrichtung als besonders wichtig oder wichtig gilt ([§ 33 Abs. 1](https://www.gesetze-im-internet.de/bsig_2025/__33.html)); die Meldepflicht für Sicherheitsvorfälle gilt frühestens ab Einrichtung des Meldewegs ([§ 32 Abs. 1](https://www.gesetze-im-internet.de/bsig_2025/__32.html)). Die Details zum Registrierungsverfahren beschreibt das [BSI](https://www.bsi.bund.de/DE/Themen/Regulierte-Wirtschaft/NIS-2-regulierte-Unternehmen/nis-2-regulierte-unternehmen_node.html).

* **Gültig für** ([Art. 2](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_2), [Art. 3](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_3)):

    Öffentliche und private Einrichtungen der in [Anhang I](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#anx_I) (Sektoren mit hoher Kritikalität) oder [Anhang II](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#anx_II) (sonstige kritische Sektoren) genannten Arten, die mindestens mittlere Unternehmen im Sinne der Empfehlung 2003/361/EG sind und ihre Dienste in der Union erbringen ([Art. 2 Abs. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_2)). Die Richtlinie unterscheidet:

    * **Wesentliche Einrichtungen** ([Art. 3 Abs. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_3)): u. a. Einrichtungen nach Anhang I, die die Schwellenwerte für mittlere Unternehmen überschreiten (also große Unternehmen), qualifizierte Vertrauensdiensteanbieter sowie TLD-Namenregister und DNS-Diensteanbieter unabhängig von der Größe, mittlere Anbieter öffentlicher elektronischer Kommunikationsnetze und -dienste, Einrichtungen der öffentlichen Verwaltung der Zentralregierung und als kritisch eingestufte Einrichtungen nach der Richtlinie (EU) 2022/2557 (CER).
    * **Wichtige Einrichtungen** ([Art. 3 Abs. 2](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_3)): alle übrigen Einrichtungen der Anhänge I oder II, die nicht wesentlich sind (z. B. mittlere Unternehmen in Anhang I sowie mittlere und große Unternehmen in Anhang II).
    * **Größenunabhängig** erfasst sind u. a. Anbieter öffentlicher elektronischer Kommunikationsnetze und -dienste, Vertrauensdiensteanbieter, TLD-Namenregister und DNS-Diensteanbieter, Einzelanbieter eines für kritische gesellschaftliche oder wirtschaftliche Tätigkeiten unerlässlichen Dienstes sowie Einrichtungen, die Domänennamenregistrierungsdienste erbringen ([Art. 2 Abs. 2 bis 4](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_2)).
    * **Sektoren Anhang I**: Energie, Verkehr, Bankwesen, Finanzmarktinfrastrukturen, Gesundheitswesen, Trinkwasser, Abwasser, digitale Infrastruktur (u. a. Cloud-Computing, Rechenzentren, CDN, DNS, TLD, Vertrauensdienste, Kommunikationsnetze), Verwaltung von IKT-Diensten (B2B: Anbieter verwalteter Dienste und verwalteter Sicherheitsdienste), öffentliche Verwaltung, Weltraum.
    * **Sektoren Anhang II**: Post- und Kurierdienste, Abfallbewirtschaftung, Chemie, Lebensmittel, verarbeitendes Gewerbe (Medizinprodukte und In-vitro-Diagnostika, Datenverarbeitungsgeräte/Elektronik/Optik, elektrische Ausrüstungen, Maschinenbau, Kraftwagen, sonstiger Fahrzeugbau), Anbieter digitaler Dienste (Online-Marktplätze, Online-Suchmaschinen, Plattformen für soziale Netzwerke), Forschung.
    * **Deutschland**: Als "besonders wichtige" Einrichtung (entspricht der wesentlichen Einrichtung) gelten u. a. Betreiber kritischer Anlagen sowie Einrichtungen der Anlage 1 ab 250 Mitarbeitern oder mehr als 50 Mio. EUR Jahresumsatz und zugleich mehr als 43 Mio. EUR Bilanzsumme; als "wichtige" Einrichtung gelten Einrichtungen der Anlagen 1 und 2 ab 50 Mitarbeitern oder mehr als 10 Mio. EUR Jahresumsatz und Bilanzsumme ([§ 28](https://www.gesetze-im-internet.de/bsig_2025/__28.html)).

* **Nicht gültig für**:
    * Einrichtungen der öffentlichen Verwaltung, die ihre Tätigkeiten in den Bereichen nationale Sicherheit, öffentliche Sicherheit, Verteidigung oder Strafverfolgung ausüben ([Art. 2 Abs. 7](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_2)); die Mitgliedstaaten können weitere derartige Einrichtungen von den Pflichten aus [Art. 21](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_21) und [Art. 23](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_23) ausnehmen ([Art. 2 Abs. 8](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_2))
    * Kleinst- und kleine Unternehmen, sofern kein größenunabhängiger Tatbestand nach [Art. 2 Abs. 2 bis 4](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_2) vorliegt
    * Einrichtungen, die die Mitgliedstaaten nach Art. 2 Abs. 4 der DORA-Verordnung vom DORA-Anwendungsbereich ausgenommen haben ([Art. 2 Abs. 10](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_2))
    * Einrichtungen, für die ein **sektorspezifischer Rechtsakt** der Union mit mindestens gleichwertigen Anforderungen gilt: Die einschlägigen Bestimmungen der NIS2, einschließlich Aufsicht und Durchsetzung, finden dann keine Anwendung ([Art. 4](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_4)). Das betrifft insbesondere Finanzunternehmen unter [DORA](dora.md).
    * Reine Hersteller von Hard- und Software sind nicht als solche erfasst: Die Anhänge nennen keine allgemeine Softwarehersteller-Kategorie. Erfasst sind jedoch die in Anhang I und II aufgeführten Dienste und Herstellungsbereiche (z. B. Cloud-Computing, verwaltete Dienste, Online-Marktplätze sowie das verarbeitende Gewerbe nach Anhang II). Produktsicherheit regelt der [Cyber Resilience Act](cra.md).

* **Grauzone**:
    * Abgrenzung zu [DORA](dora.md): DORA gilt für Finanzunternehmen, die nach den nationalen Umsetzungsvorschriften zu [Art. 3](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_3) als wesentliche oder wichtige Einrichtungen ermittelt wurden, als sektorspezifischer Rechtsakt im Sinne von [Art. 4](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_4) (DORA Art. 1 Abs. 2, [Verordnung (EU) 2022/2554](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022R2554#art_1)). Voraussetzung für die Nichtanwendung der NIS2-Bestimmungen ist nach [Art. 4 Abs. 1 und 2](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_4) eine mindestens gleichwertige Wirkung der sektorspezifischen Anforderungen an das Risikomanagement oder an die Meldung erheblicher Vorfälle. Gilt der Rechtsakt nicht für alle Einrichtungen eines Sektors, bleibt die NIS2 für die nicht erfassten Einrichtungen anwendbar. In Deutschland sind die Pflichten nach [§§ 30, 31, 32, 35, 36, 38 und 39 BSIG](https://www.gesetze-im-internet.de/bsig_2025/__28.html) für Finanzunternehmen nach Art. 2 Abs. 2 der DORA-Verordnung ausgenommen ([§ 28 Abs. 6](https://www.gesetze-im-internet.de/bsig_2025/__28.html)). Konzerne mit gemischten Tätigkeiten sind im Einzelfall zu prüfen.
    * Dienstleister und Zulieferer, die selbst nicht in den Anhängen genannt sind, sind mittelbar über die Lieferkettenanforderungen ihrer Kunden betroffen ([Art. 21 Abs. 2 lit. d und Abs. 3](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_21)).
    * Verhältnis zur Cybersicherheit von Produkten: Die NIS2 regelt Einrichtungen und deren Betrieb; Anforderungen an Produkte mit digitalen Elementen stellt der [Cyber Resilience Act](cra.md).
    * Verhältnis zu kritischen Anlagen in Deutschland: [KRITIS-Dachgesetz](kritis-dachgesetz.md) (physische Resilienz, Richtlinie (EU) 2022/2557) und BSIG ergänzen sich; für die Einstufung als kritische Anlage nach BSIG gelten Übergangsregelungen ([§ 66](https://www.gesetze-im-internet.de/bsig_2025/__66.html)).

* **Ziel**:
  Ein hohes gemeinsames Cybersicherheitsniveau in der gesamten Union zur Verbesserung des Funktionierens des Binnenmarkts ([Art. 1 Abs. 1](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_1)).

* **Neuerungen / Anforderungen**:
    * Pflicht der Mitgliedstaaten zu nationalen Cybersicherheitsstrategien, zuständigen Behörden, zentralen Anlaufstellen und CSIRTs ([Art. 1 Abs. 2 lit. a](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_1))
    * Verantwortung der Leitungsorgane ([Art. 20](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_20))
    * Risikomanagementmaßnahmen im Bereich der Cybersicherheit ([Art. 21](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_21))
    * Gestuftes Meldeverfahren für erhebliche Sicherheitsvorfälle ([Art. 23](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_23))
    * Registrierung der Einrichtungen ([Art. 3 Abs. 3 und 4](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_3); für bestimmte digitale Anbieter zusätzlich das ENISA-Register nach [Art. 27](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_27))
    * Aufsicht, Durchsetzung und Geldbußen ([Art. 32](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_32) bis [Art. 34](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_34))
    * Konkretisierung für digitale Anbieter durch die [Durchführungsverordnung (EU) 2024/2690](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32024R2690): Sie gilt für DNS-Diensteanbieter, TLD-Namenregister, Cloud-Computing-Dienstleister, Rechenzentrumsdienste, Inhaltszustellnetze, Anbieter verwalteter Dienste und verwalteter Sicherheitsdienste, Online-Marktplätze, Online-Suchmaschinen, Plattformen für soziale Netzwerke und Vertrauensdiensteanbieter (Art. 1). Ihr Anhang legt die technischen und methodischen Anforderungen zu den Maßnahmen nach [Art. 21 Abs. 2 lit. a bis j](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_21) fest (Art. 2; z. B. Nr. 5 zur Sicherheit der Lieferkette); die Art. 3 bis 14 präzisieren, wann ein Sicherheitsvorfall als erheblich gilt (z. B. direkter finanzieller Verlust von mehr als 500 000 EUR oder 5 % des Jahresumsatzes, je nachdem, welcher Wert niedriger ist, Art. 3 Abs. 1 lit. a). Sie wurde am 18.10.2024 veröffentlicht und ist am 20. Tag danach (07.11.2024) in Kraft getreten (Art. 16).



## Zentrale Forderungen

* **Governance und Rechenschaftspflicht** ([Art. 20](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_20)):

    Die Leitungsorgane wesentlicher und wichtiger Einrichtungen müssen die Risikomanagementmaßnahmen nach [Art. 21](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_21) billigen, deren Umsetzung überwachen und können für Verstöße verantwortlich gemacht werden (Abs. 1). Die Mitglieder der Leitungsorgane müssen an Schulungen teilnehmen; den Beschäftigten sollen regelmäßig Schulungen angeboten werden (Abs. 2). Die natürlichen Personen in leitender Verantwortung können zudem für Verstöße haftbar gemacht werden ([Art. 32 Abs. 6](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_32), für wichtige Einrichtungen entsprechend nach [Art. 33 Abs. 5](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_33)). In Deutschland: Umsetzungs-, Überwachungs- und Schulungspflicht der Geschäftsleitung mit Haftung gegenüber der Einrichtung nach den gesellschaftsrechtlichen Regeln ([§ 38 BSIG](https://www.gesetze-im-internet.de/bsig_2025/__38.html)).

* **Risikomanagementmaßnahmen** ([Art. 21](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_21)):

    Einrichtungen müssen geeignete und verhältnismäßige technische, operative und organisatorische Maßnahmen ergreifen, die dem Stand der Technik entsprechen, auf einem gefahrenübergreifenden Ansatz beruhen und dem bestehenden Risiko angemessen sind (Abs. 1 und 2). Die Mindestmaßnahmen nach Abs. 2:

    * a) Konzepte zur Risikoanalyse und zur Sicherheit von Informationssystemen
    * b) Bewältigung von Sicherheitsvorfällen
    * c) Aufrechterhaltung des Betriebs (Backup-Management, Wiederherstellung nach einem Notfall) und Krisenmanagement
    * d) Sicherheit der Lieferkette einschließlich der Beziehungen zu unmittelbaren Anbietern und Diensteanbietern
    * e) Sicherheitsmaßnahmen bei Erwerb, Entwicklung und Wartung von Netz- und Informationssystemen, einschließlich Management und Offenlegung von Schwachstellen
    * f) Konzepte und Verfahren zur Bewertung der Wirksamkeit der Risikomanagementmaßnahmen
    * g) grundlegende Verfahren der Cyberhygiene und Schulungen
    * h) Konzepte und Verfahren für den Einsatz von Kryptografie und gegebenenfalls Verschlüsselung
    * i) Sicherheit des Personals, Zugriffskontrolle und Management von Anlagen
    * j) Multi-Faktor- oder kontinuierliche Authentifizierung, gesicherte Sprach-, Video- und Textkommunikation sowie gegebenenfalls gesicherte Notfallkommunikation

    Deutsche Umsetzung: [§ 30 Abs. 2 BSIG](https://www.gesetze-im-internet.de/bsig_2025/__30.html) (Nr. 1 bis 10 entsprechen lit. a bis j).

* **Sicherheit der Lieferkette** ([Art. 21 Abs. 2 lit. d und Abs. 3](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_21), [Art. 22](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_22)):

    Bei den Lieferkettenmaßnahmen sind die spezifischen Schwachstellen der einzelnen unmittelbaren Anbieter und Diensteanbieter, die Gesamtqualität ihrer Produkte und ihrer Cybersicherheitspraxis, einschließlich der Sicherheit ihrer Entwicklungsprozesse, sowie die Ergebnisse koordinierter Risikobewertungen kritischer Lieferketten auf EU-Ebene zu berücksichtigen (Art. 21 Abs. 3). Die Richtlinie selbst nennt weder eine SBOM-Pflicht noch Due-Diligence-Prüfungen im Einzelnen; die Durchführungsverordnung (EU) 2024/2690 (Anhang Nr. 5) konkretisiert dies für die dort genannten digitalen Anbieter.

* **Meldung von Vorfällen** ([Art. 23](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_23)):

    Erhebliche Sicherheitsvorfälle sind dem CSIRT oder der zuständigen Behörde zu melden (Abs. 1). Ein Vorfall ist erheblich, wenn er schwerwiegende Betriebsstörungen oder finanzielle Verluste verursacht hat oder verursachen kann oder andere Personen durch erhebliche materielle oder immaterielle Schäden beeinträchtigt hat oder beeinträchtigen kann (Abs. 3). Gestufte Fristen (Abs. 4):

    * unverzüglich, spätestens **24 Stunden** nach Kenntnisnahme: Frühwarnung (u. a. Verdacht auf rechtswidrige oder böswillige Handlung, grenzüberschreitende Auswirkungen)
    * unverzüglich, spätestens **72 Stunden** nach Kenntnisnahme: Meldung des Vorfalls mit erster Bewertung (Schweregrad, Auswirkungen, ggf. Kompromittierungsindikatoren); für Vertrauensdiensteanbieter gilt hierfür ebenfalls eine Frist von 24 Stunden
    * auf Ersuchen: Zwischenbericht
    * spätestens **einen Monat** nach der Meldung: Abschlussbericht (bei andauerndem Vorfall: Fortschrittsbericht und Abschlussbericht innerhalb eines Monats nach Behandlung des Vorfalls)

    Gegebenenfalls sind außerdem die Empfänger der Dienste zu unterrichten (Abs. 1 und 2). Die Meldung allein begründet keine höhere Haftung der meldenden Einrichtung (Abs. 1). Deutsche Umsetzung: Meldung an die gemeinsame Meldestelle von BSI und BBK mit denselben Fristen ([§ 32 BSIG](https://www.gesetze-im-internet.de/bsig_2025/__32.html)).

* **Registrierung** ([Art. 3 Abs. 3 und 4](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_3), [Art. 27](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_27)):

    Die Mitgliedstaaten erstellen Listen der wesentlichen und wichtigen Einrichtungen (bis 17.04.2025, danach mindestens alle zwei Jahre überprüft); die Einrichtungen übermitteln dafür Name, Kontaktdaten, Sektor und die betroffenen Mitgliedstaaten und melden Änderungen innerhalb von zwei Wochen (Art. 3 Abs. 4). Für DNS-Diensteanbieter, TLD-Namenregister, Cloud-, Rechenzentrums-, CDN-, Managed-Service-Anbieter, Online-Marktplätze, Suchmaschinen und soziale Netzwerke führt zudem die ENISA ein EU-Register (Art. 27). In Deutschland: Registrierung beim BSI ([§ 33 BSIG](https://www.gesetze-im-internet.de/bsig_2025/__33.html)).

* **Aufsicht und Durchsetzung** ([Art. 32](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_32), [Art. 33](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_33)):

    * Wesentliche Einrichtungen unterliegen einer umfassenden Aufsicht: Vor-Ort-Kontrollen, regelmäßige und gezielte Sicherheitsprüfungen, Ad-hoc-Prüfungen, Sicherheitsscans, Informations- und Nachweisanforderungen (Art. 32 Abs. 2). Durchsetzungsbefugnisse reichen von Warnungen und verbindlichen Anweisungen bis zur Benennung eines Überwachungsbeauftragten und zur Veröffentlichung von Verstößen (Abs. 4); bei Wirkungslosigkeit sind u. a. die vorübergehende Aussetzung von Zertifizierungen oder Genehmigungen und ein vorübergehendes Tätigkeitsverbot für Leitungspersonen vorzusehen (Abs. 5).
    * Wichtige Einrichtungen unterliegen nur einer nachträglichen (Ex-post-)Aufsicht, wenn Nachweise, Hinweise oder Informationen auf eine Nichterfüllung hindeuten (Art. 33 Abs. 1); die Befugnisse sind ähnlich ausgestaltet (Art. 33 Abs. 2 und 4).
    * Deutschland: [§ 61 BSIG](https://www.gesetze-im-internet.de/bsig_2025/__61.html) (besonders wichtige Einrichtungen), [§ 62 BSIG](https://www.gesetze-im-internet.de/bsig_2025/__62.html) (wichtige Einrichtungen).

* **Geldbußen** ([Art. 34](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_34)):

    Mindest-Höchstbeträge, die die Mitgliedstaaten vorsehen müssen, bei Verstößen gegen [Art. 21](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_21) oder [Art. 23](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_23):

    * wesentliche Einrichtungen: mindestens 10 000 000 EUR oder mindestens 2 % des weltweiten Vorjahresumsatzes des Unternehmens, je nachdem, welcher Betrag höher ist (Abs. 4)
    * wichtige Einrichtungen: mindestens 7 000 000 EUR oder mindestens 1,4 % des weltweiten Vorjahresumsatzes, je nachdem, welcher Betrag höher ist (Abs. 5)

    Deutschland ([§ 65 Abs. 5 bis 7 BSIG](https://www.gesetze-im-internet.de/bsig_2025/__65.html)): bis zu 10 Mio. EUR (besonders wichtige) bzw. 7 Mio. EUR (wichtige Einrichtungen); bei einem Gesamtumsatz von mehr als 500 Mio. EUR bis zu 2 % bzw. 1,4 % des Gesamtumsatzes.

* **Informationsaustausch und Zusammenarbeit** ([Art. 29](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_29), [Art. 30](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_30)):

    Freiwilliger Austausch von Cybersicherheitsinformationen (Bedrohungen, Beinahe-Vorfälle, Schwachstellen, Kompromittierungsindikatoren) innerhalb von Gemeinschaften wesentlicher und wichtiger Einrichtungen auf Basis von Vereinbarungen (Art. 29); zusätzlich freiwillige Meldungen an CSIRTs oder Behörden (Art. 30).

* **Zertifizierung und Normung** ([Art. 24](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_24), [Art. 25](https://eur-lex.europa.eu/legal-content/DE/TXT/HTML/?uri=CELEX:32022L2555#art_25)):

    Die Mitgliedstaaten können die Verwendung zertifizierter IKT-Produkte, -Dienste und -Prozesse vorschreiben; die Anwendung europäischer und internationaler Normen ist zu fördern.



## Lösungsansätze & Hilfestellungen


* Informationen des BSI zu NIS-2-regulierten Unternehmen, Registrierung und Meldepflicht: [BSI NIS-2](https://www.bsi.bund.de/DE/Themen/Regulierte-Wirtschaft/NIS-2-regulierte-Unternehmen/nis-2-regulierte-unternehmen_node.html)
* Der [IT-Grundschutz des BSI](https://www.bsi.bund.de/DE/Themen/Unternehmen-und-Organisationen/Standards-und-Zertifizierung/IT-Grundschutz/IT-Grundschutz-Kompendium/it-grundschutz-kompendium_node.html) kann als Methodik für Risikoanalyse und Maßnahmenumsetzung dienen (keine Konformitätsvermutung im Gesetz; siehe Art. 25 zur Normung).
* Überblick der Europäischen Kommission zur NIS2: [Kommission: NIS2-Richtlinie](https://digital-strategy.ec.europa.eu/en/policies/nis2-directive)

### Tools & Werkzeuge

#### GRC & Risikomanagement

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [MONARC](https://github.com/monarc-project/MonarcAppFO) | Open Source (AGPL) | Strukturierte Risikoanalyse nach ISO 27005; entwickelt von CASES Luxemburg | NIS2 Art. 21: Risikomanagementmaßnahmen |
| [Eramba](https://www.eramba.org/) | Open Source (AGPL, Community Edition) | GRC-Plattform: Risikoregister, Controls, Compliance-Mapping | NIS2 Art. 20–21, ISO 27001 |
| [OpenRMF](https://github.com/Cingulara/openrmf-oss) | Open Source (GPL-3.0) | RMF-Dokumentation, STIG-Checklisten, Compliance-Tracking | IT-Risikomanagement |

#### Incident Management & Threat Intelligence

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [TheHive](https://thehive-project.org/) | Open Source (AGPL) | Security Incident Response Plattform; strukturierte Vorfallbearbeitung und Reporting | NIS2 Art. 23: Meldepflicht schwerwiegender Vorfälle |
| [MISP](https://www.misp-project.org/) | Open Source (AGPL) | Threat Intelligence Sharing; Austausch von IoCs zwischen Organisationen und Behörden | NIS2 Art. 29: Informationsaustausch |
| [Cortex](https://github.com/TheHive-Project/Cortex) | Open Source (AGPL) | Automatisierte Analyse von Observables; ergänzt TheHive | Unterstützt Incident-Response-Prozesse |
| [Deming](https://github.com/dbarzin/deming) | Open Source (GPL) | Web-basiertes IT-Sicherheits-Audit-Management nach ISO 27001; Maßnahmen-Tracking, Reifegradmessung und Compliance-Nachweise | NIS2 Art. 21: Risikomanagement-Maßnahmen dokumentieren und nachweisen |

#### SBOM & Lieferkettensicherheit (Art. 21 Abs. 2 lit. d und e)

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [TrustSource ts-scan](https://github.com/TrustSource/ts-scan) | Open Source | Universeller SCA-Scanner: analysiert Abhängigkeiten aus Build-Systemen und Paketmanagern, erzeugt CycloneDX/SPDX-SBOMs und lädt Ergebnisse in die TrustSource-Plattform hoch | NIS2 Art. 21(2)(d): Lieferkettensicherheit — SBOM als Basis für kontinuierliches Schwachstellenmanagement der eingesetzten Komponenten |
| [TrustSource CE](https://github.com/trustsource/ts-core-ce) | AGPL (Community Edition) | Vollständige SCA-Plattform: SBOM-Versionierung, Vulnerability Management und CSAF-Kommunikation — schließt den Loop von der Komponentenanalyse bis zum Security Advisory | NIS2 Art. 21(2)(d)(e): Lieferkettensicherheit und Schwachstellenprozesse |
| [OWASP Dependency-Track](https://dependencytrack.org/) | Apache-2.0 | Kontinuierliche SBOM-Analyse: nimmt SBOMs entgegen, überwacht fortlaufend gegen NVD, OSV und weitere Datenbanken | NIS2 Art. 21(2)(d)(e): Zentrales SBOM-Lifecycle-Management und Schwachstellen-Monitoring |

#### Monitoring & Schwachstellenmanagement

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [Wazuh](https://wazuh.com/) | Open Source (GPL) | SIEM, Intrusion Detection, Log-Analyse, Schwachstellenerkennung | NIS2 Art. 21: Sicherheit von Netz- und Informationssystemen |
| [OpenVAS / Greenbone](https://www.greenbone.net/) | Open Source (GPL) | Schwachstellenscanner für Netzwerke und Systeme | NIS2: Schwachstellenmanagement |
| [Zabbix](https://www.zabbix.com/) | Open Source (GPL-2.0) | Infrastruktur-Monitoring und Alerting | Betriebsstabilität, Frühwarnung |


## Quellen

Alle EU-Rechtstexte in der deutschen Fassung im Amtsblatt der EU (ELI-Links):

* [Richtlinie (EU) 2022/2555 (NIS2)](https://eur-lex.europa.eu/eli/dir/2022/2555/oj)
* [Durchführungsverordnung (EU) 2024/2690](https://eur-lex.europa.eu/eli/reg_impl/2024/2690/oj): technische und methodische Anforderungen und erhebliche Sicherheitsvorfälle für digitale Anbieter
* [Verordnung (EU) 2022/2554 (DORA)](https://eur-lex.europa.eu/eli/reg/2022/2554/oj), Art. 1 Abs. 2: DORA als sektorspezifischer Rechtsakt im Sinne von NIS2 Art. 4
* [Richtlinie (EU) 2022/2557 (CER)](https://eur-lex.europa.eu/eli/dir/2022/2557/oj): kritische Einrichtungen
* [Empfehlung 2003/361/EG](https://eur-lex.europa.eu/eli/reco/2003/361/oj): KMU-Definition (Größenschwellen)
* [Richtlinie (EU) 2016/1148 (NIS-Richtlinie, aufgehoben)](https://eur-lex.europa.eu/eli/dir/2016/1148/oj)

Deutsche Umsetzung:

* [BSI-Gesetz (BSIG)](https://www.gesetze-im-internet.de/bsig_2025/BJNR12D0B0025.html), Artikel 1 des NIS-2-Umsetzungs- und Cybersicherheitsstärkungsgesetzes vom 02.12.2025, [BGBl. 2025 I Nr. 301](https://www.recht.bund.de/bgbl/1/2025/301/VO.html), in Kraft seit 06.12.2025
* [BSI: NIS-2-regulierte Unternehmen](https://www.bsi.bund.de/DE/Themen/Regulierte-Wirtschaft/NIS-2-regulierte-Unternehmen/nis-2-regulierte-unternehmen_node.html)
* [Europäische Kommission: NIS2-Richtlinie](https://digital-strategy.ec.europa.eu/en/policies/nis2-directive)
