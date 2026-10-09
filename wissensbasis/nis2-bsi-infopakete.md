# NIS-2: Zusammenfassung der BSI-Infopakete (#nis2know)

**Zweck:** Interne Wissensbasis der OSBA WG Security. Das Dokument fasst die vom BSI veröffentlichten #nis2know-Infopakete zusammen, damit wir den Hintergrund zur deutschen NIS-2-Umsetzung (BSIG) kennen. Es ist **nicht** Teil der veröffentlichten Website (liegt außerhalb von `docs/`) und keine Rechtsberatung.

**Stand der Quellen:** Abruf am 09.10.2026 von bsi.bund.de. Die BSI-Seiten werden fortlaufend aktualisiert; der Gesetzestext ([BSIG](https://www.gesetze-im-internet.de/bsig_2025/BJNR12D0B0025.html)) hat Vorrang. Die für die öffentliche Seite relevanten Punkte stehen bereits in [docs/nis2.md](../docs/nis2.md) im Abschnitt „Vorgaben des BSI (Deutschland)".

**Lesetiefe:** Die Pakete Risikoanalyse, Incident Response, BCM, Wirksamkeit, Kryptografie, Schulungen, Sicherheitsmaßnahmen, Lieferkette, DORA, Geschäftsleitungsschulung, Meldepflicht und ISO/IEC 27001 habe ich im Wesentlichen vollständig gelesen. MFA, Personalsicherheit/Asset-Management und Gesundheit sind nur in ihren Kernabschnitten ausgewertet. Die verlinkten Hilfsmittel (BSI-Standards, Mappingtabellen, Onepager) habe ich nicht gelesen.

Alle Pakete haben denselben Aufbau: *Warum – Wer ist betroffen – Was ist zu beachten – Was tun – Welche Standards gibt es*. Die Basis-URL aller Pakete lautet
`https://www.bsi.bund.de/DE/Themen/Regulierte-Wirtschaft/NIS-2-regulierte-Unternehmen/NIS-2-Infopakete/`.

## Überblick: Pakete und Zuordnung zu § 30 Abs. 2 BSIG

| Nr. nach § 30 Abs. 2 BSIG | Maßnahme | BSI-Infopaket |
|---|---|---|
| 1 | Konzepte zur Risikoanalyse und Sicherheit in der IT | [Risikoanalyse](https://www.bsi.bund.de/DE/Themen/Regulierte-Wirtschaft/NIS-2-regulierte-Unternehmen/NIS-2-Infopakete/NIS-2-Risikoanalyse/NIS-2-Risikoanalyse_node.html) |
| 2 | Bewältigung von Sicherheitsvorfällen | [Incident Response](https://www.bsi.bund.de/DE/Themen/Regulierte-Wirtschaft/NIS-2-regulierte-Unternehmen/NIS-2-Infopakete/NIS-2-Incident-Response/NIS-2-Incident-Response_node.html) |
| 3 | Betriebsaufrechterhaltung, Backup, Krisenmanagement | [BCM](https://www.bsi.bund.de/DE/Themen/Regulierte-Wirtschaft/NIS-2-regulierte-Unternehmen/NIS-2-Infopakete/NIS-2-BCM/NIS-2-BCM_node.html) |
| 4 | Sicherheit der Lieferkette | [Sichere Lieferkette](https://www.bsi.bund.de/DE/Themen/Regulierte-Wirtschaft/NIS-2-regulierte-Unternehmen/NIS-2-Infopakete/NIS-2-Lieferkette/NIS-2-Lieferkette_node.html) |
| 5 | Erwerb, Entwicklung, Wartung, Schwachstellenmanagement | [Sicherheitsmaßnahmen und Schwachstellenmanagement](https://www.bsi.bund.de/DE/Themen/Regulierte-Wirtschaft/NIS-2-regulierte-Unternehmen/NIS-2-Infopakete/NIS-2-Sicherheitsmassnahmen/NIS-2-Sicherheitsmassnahmen_node.html) |
| 6 | Bewertung der Wirksamkeit der Maßnahmen | [Bewertung der Wirksamkeit](https://www.bsi.bund.de/DE/Themen/Regulierte-Wirtschaft/NIS-2-regulierte-Unternehmen/NIS-2-Infopakete/NIS-2-Bewertung-der-Wirksamkeit-von-Massnahmen/NIS-2-Bewertung-der-Wirksamkeit_node.html) |
| 7 | Schulungen und Sensibilisierung | [Grundlegende Schulungen](https://www.bsi.bund.de/DE/Themen/Regulierte-Wirtschaft/NIS-2-regulierte-Unternehmen/NIS-2-Infopakete/NIS-2-Schulungen/NIS-2-Schulungen_node.html) |
| 8 | Kryptografische Verfahren | [Kryptografische Verfahren](https://www.bsi.bund.de/DE/Themen/Regulierte-Wirtschaft/NIS-2-regulierte-Unternehmen/NIS-2-Infopakete/NIS-2-kryptografische-Verfahren/NIS-2-kryptografische-Verfahren_node.html) |
| 9 | Personal, Zugriffskontrolle, Asset-Management | [Personalsicherheit, Zugriffskontrolle, Assetmanagement](https://www.bsi.bund.de/DE/Themen/Regulierte-Wirtschaft/NIS-2-regulierte-Unternehmen/NIS-2-Infopakete/NIS-2-Personalsicherheit/NIS-2-Personalsicherheit_node.html) |
| 10 | MFA, gesicherte Kommunikation | [MFA und gesicherte Kommunikation](https://www.bsi.bund.de/DE/Themen/Regulierte-Wirtschaft/NIS-2-regulierte-Unternehmen/NIS-2-Infopakete/NIS-2-MFA/NIS-2-MFA_node.html) |
| – | Übersicht aller Maßnahmen | [Risikomanagementmaßnahmen](https://www.bsi.bund.de/DE/Themen/Regulierte-Wirtschaft/NIS-2-regulierte-Unternehmen/NIS-2-Infopakete/NIS-2-Risikomanagementmassnahmen/NIS-2-Risikomanagementmassnahmen_node.html) |
| – | Querschnitt | [Meldepflicht](https://www.bsi.bund.de/DE/Themen/Regulierte-Wirtschaft/NIS-2-regulierte-Unternehmen/NIS-2-Infopakete/NIS-2-Meldepflicht/NIS-2-Meldepflicht_node.html), [Geschäftsleitungsschulung](https://www.bsi.bund.de/DE/Themen/Regulierte-Wirtschaft/NIS-2-regulierte-Unternehmen/NIS-2-Infopakete/NIS-2-Geschaeftsleitungsschulung/NIS-2-Geschaeftsleitungsschulung_node.html), [DORA und NIS-2](https://www.bsi.bund.de/DE/Themen/Regulierte-Wirtschaft/NIS-2-regulierte-Unternehmen/NIS-2-Infopakete/NIS-2-DORA/NIS-2-DORA_node.html), [ISO/IEC 27001](https://www.bsi.bund.de/DE/Themen/Regulierte-Wirtschaft/NIS-2-regulierte-Unternehmen/NIS-2-Infopakete/NIS-2-ISO27001/NIS-2-ISO-27001_node.html), [Gesundheit](https://www.bsi.bund.de/DE/Themen/Regulierte-Wirtschaft/NIS-2-regulierte-Unternehmen/NIS-2-Infopakete/NIS-2-Gesundheit/NIS-2-Gesundheit_node.html) |

**Grundaussagen, die sich durch alle Pakete ziehen**
- Maßnahmen müssen geeignet, verhältnismäßig und wirksam sein, dem Stand der Technik entsprechen und europäische und internationale Normen berücksichtigen (§ 30 Abs. 1 BSIG).
- Jedes Paket enthält eine Tabelle, die BSI-Anforderungen auf Normen abbildet (EU-Durchführungsverordnung 2024/2690, ISO/IEC 27001:2022 Anhang A, TISAX, RUN, CyberRisikoCheck, teilweise IT-Grundschutz-Praktiken). Das BSI weist jeweils darauf hin, dass die Umsetzung nach einer dieser Normen **nicht automatisch** die BSIG-Anforderungen erfüllt.
- RUN (Reife- und Umsetzungsgradbewertung) gilt nur für Betreiber kritischer Anlagen. Der CyberRisikoCheck ist nur eine Ersteinschätzung und kein Konformitätsnachweis.
- Der IT-Grundschutz wird derzeit überarbeitet („Grundschutz++"). Mappings beziehen sich auf den Stand vom 01.10.2025 (Version 0.9.5), veröffentlicht in der [Stand-der-Technik-Bibliothek](https://www.github.com/BSI-Bund/Stand-der-Technik-Bibliothek) auf GitHub.

## 1. Risikoanalyse (§ 30 Abs. 2 Nr. 1)

- Pflicht zu einer regelmäßigen Risikoanalyse; die **Methodik ist frei**, empfohlen wird die Orientierung an Standards (BSI-Standard 200-3, 200-4, ISO 27001).
- Bestandteile: Bedrohungen und Schwachstellen identifizieren, Risiken bewerten (Eintrittswahrscheinlichkeit, Auswirkung), Wirksamkeit bestehender Maßnahmen bewerten, Ergebnisse dokumentieren, regelmäßig überprüfen (insbesondere bei neuer Bedrohungslage oder neuen Schwachstellen).
- Verhältnismäßigkeitsfaktoren: Normen, Stand der Technik, Kosten, Risikoexposition, Größe, Eintrittswahrscheinlichkeit, Schwere und Auswirkungen.
- Vereinfachter Ablauf: Kontext verstehen, Assets identifizieren und nach Vertraulichkeit/Integrität/Verfügbarkeit klassifizieren, Risiken bewerten (Risikomatrix, Akzeptanzkriterien, Risikoeigner), Risikobehandlung (vermeiden, verringern, übertragen, akzeptieren), dokumentieren, regelmäßig überprüfen.
- Hinweis: Das BSIG verlangt umgesetzte, wirksame Maßnahmen; ein pauschaler Risikotransfer oder eine generelle Risikoakzeptanz ist laut BSI-Paket zu ISO 27001 nicht zulässig (siehe dort).

## 2. Incident Response (§ 30 Abs. 2 Nr. 2)

- Pflicht, Maßnahmen zur Bewältigung von Sicherheitsvorfällen umzusetzen; die Meldepflicht (§ 32 BSIG) ist Teil des Incident-Response-Prozesses.
- Empfohlene Phasen: **Vorsorge** (Budget und Personal, ISMS mit Risikoanalyse, Notfallpläne, regelmäßige Krisenübungen, ausreichende Dokumentation der IT, Logdaten für die Forensik, regelmäßige Backups mit eingeübter Wiederherstellung), **Detektion**, **Vorfallsbewältigung** (Verdacht verifizieren, bestehende Konzepte nutzen, Kommunikation, Meldung nach NIS-2 und ggf. DSGVO, Strafanzeige, Kunden und Geschäftspartner informieren, kritische Systeme weiterbetreiben, Bereinigung, Dokumentation, bei Bedarf qualifizierte Incident-Response-Dienstleister laut QDL-Liste), **Nachsorge** (Lessons Learned, Schwachstellen schließen, ggf. Härtung wie MFA).
- Mapping auf ISO 27001: u. a. A.5.24 bis A.5.28, A.6.8, A.8.15 bis A.8.17.

## 3. Business Continuity Management (§ 30 Abs. 2 Nr. 3)

- Das Gesetz nennt BCM nicht ausdrücklich, verlangt aber Elemente davon (Backup-Management, Wiederherstellung nach Notfall, Krisenmanagement). Das BSI empfiehlt, ein BCMS einzuführen.
- Nutzen laut BSI: Geschäftsbetrieb sichern, Menschen und Ressourcen schützen, finanzielle Verluste vermeiden, Wettbewerbsvorteil.
- Hilfen: BSI-Standard 200-4 (BCM) mit Anforderungskatalog und Hilfsmitteln, Leitfaden „Einstieg in das BCM für KMU" (drei Stufen vom reaktiven bis zum standardisierten BCM).
- Mapping: ISO 27001 A.5.29, A.5.30, A.8.13, A.8.14, A.7.11; Grundschutz-Bausteine NOT.1 bis NOT.4.

## 4. Sichere Lieferkette (§ 30 Abs. 2 Nr. 4)

- Betroffene Einrichtungen müssen ihre Zulieferer zur Einhaltung entsprechender Sicherheitsanforderungen verpflichten. Das BSIG verpflichtet Zulieferer nicht unmittelbar; es kann aber dazu führen, dass betroffene Einrichtungen nicht mehr mit jedem Zulieferer zusammenarbeiten können.
- Besondere Herausforderungen: Kontrolle über Personal von Dienstleistern, Risikomanagement über mehrere Zuliefererebenen, Wirksamkeitsprüfung und Audits.
- **C-SCRM in fünf Schritten:** Beteiligte und Schnittstellen identifizieren, Richtlinien und Prozesse entwickeln, Hard- und Software und deren Bezugsquelle kennen, die gesamte Kette inklusive Sub-Zulieferern verstehen, Wirksamkeit bewerten und Auditfähigkeit sichern.
- Empfehlungen: SLAs mit Zulieferern zu Risikomanagement, Vorfallsbewältigung und Patchmanagement, Security by Design und Security by Default, Berücksichtigung von BSI-Empfehlungen, Aufbau eines ISMS (ISO 27001:2022, BSI-Standard 200-1).
- Hilfsmittel: Lieferketten-Katalog in der Stand-der-Technik-Bibliothek (GitHub), Management Blitzlicht „Grundlagen des C-SCRM".
- **Relevanz für OSBA:** Der Fokus auf Entwicklungsprozesse und Patchmanagement der Zulieferer entspricht den Anforderungen, die Open-Source-Projekte und Software-Hersteller künftig von Kunden hören werden (Bezug zu SBOM, CRA).

## 5. Sicherheitsmaßnahmen und Schwachstellenmanagement (§ 30 Abs. 2 Nr. 5)

- Gilt für alle Systeme, Komponenten und Prozesse, die für die Diensterbringung genutzt werden, auch OT, über den gesamten Lebenszyklus (Erwerb, Entwicklung, Betrieb/Wartung).
- **Erwerb:** Lieferanten und Produkte nach Sicherheitskriterien auswählen, vertragliche Regelungen, Audits, Komponenten ohne bekannte ausnutzbare Lücken anstreben.
- **Entwicklung:** sicherer Entwicklungszyklus, Defensive Security, Eingabevalidierung, Verschlüsselung, minimale Rechte, speichersichere Sprachen (z. B. Rust), Sicherheitstests, Code Reviews, Penetrationstests, Sicherheitskriterien für Bibliotheken und Drittsoftware, Usable Security, sichere Standardkonfiguration.
- **Betrieb/Wartung:** Konfigurationsmanagement (Härtung), Änderungsmanagement, regelmäßige Sicherheitsprüfungen, Patch- und Update-Management (priorisiert, sichere Updatemechanismen), Netzsegmentierung, Schutz vor Schadsoftware und nicht genehmigter Software, physischer Schutz.
- **Schwachstellenmanagement und Offenlegung:** regelmäßig scannen und bewerten, Behebung und Priorisierung, Dokumentation, Meldeprozess, öffentliche Meldemöglichkeit (z. B. `security.txt` nach RFC 9116), zeitnahe Mitteilung kritischer Schwachstellen, Meldung nach gesetzlichen Vorgaben (z. B. CRA), koordinierte Offenlegung, freiwillige Meldung an das BSI (auch anonym über das BSI-Portal). Exkurs: **CSAF** als Hilfsmittel für automatisiertes Schwachstellenmanagement.
- Mapping: ISO 27001 u. a. A.5.21, A.5.23, A.8.25, A.8.9, A.8.29 bis A.8.34.

## 6. Bewertung der Wirksamkeit (§ 30 Abs. 2 Nr. 6)

- Wirksamkeit ist ein fortlaufender Prozess im Sinne des PDCA-Zyklus. Unterschieden werden konzeptionelle Eignung, Umsetzungstreue und Ergebniswirksamkeit.
- Schritte: Messbarkeit herstellen (Kennzahlen und Grenzwerte, z. B. Patch-Quote, Reaktionszeiten), regelmäßige interne und externe Audits, Management-Berichte mit Bewertung durch die Unternehmensleitung, kontinuierlicher Verbesserungsprozess. Orientierung bietet das Reifegradmodell des BSI (Reifegrad 4 „messbar", Reifegrad 5 „kontinuierlich verbessert").
- Mapping: ISO 27001 Kap. 6.2, 9.1, 9.3; der CyberRisikoCheck deckt diesen Punkt laut BSI nicht ab.

## 7. Schulungen und Sensibilisierung (§ 30 Abs. 2 Nr. 7)

- Adressaten sind alle internen und externen Nutzenden von Systemen. Risiken: Phishing, schwache Passwörter, Ignorieren von Richtlinien, fehlende Sensibilisierung.
- Maßnahmen: Awareness-Schulungen (Ersteinweisung plus jährliche Auffrischung), Awareness-Programm (ENISA-Modell in acht Schritten), verständliche und praktikable Sicherheitsrichtlinien.
- **Getrennt davon** ist die Schulungspflicht der Geschäftsleitung nach § 38 Abs. 3 BSIG zu sehen (siehe Abschnitt 13).

## 8. Kryptografische Verfahren (§ 30 Abs. 2 Nr. 8)

- Pflicht zu Konzepten und Prozessen für den Einsatz von Kryptografie: Auswahl geeigneter Verfahren, sicherer Betrieb, kontinuierliche Überwachung und Anpassung, z. B. **Migration zu Post-Quanten-Kryptografie**.
- Beachten: Stand der Technik und Standards wie **BSI TR-02102** (jährlich aktualisiert; Teile 1 bis 4: Verfahren und Schlüssellängen, TLS, IPsec/IKEv2, SSH). Bestandsaufnahme (Verfahren, Schlüssel, Zertifikate), Risikoanalyse inklusive „Harvest now, decrypt later", Migrationsfähigkeit von Systemen, Dokumentation.
- Vorgehen in drei Schritten: inventarisieren, bewerten, umsetzen (Roadmap, Pilotumgebungen). Internationale PQC-Standards: NIST FIPS 203/204/205, ISO/IEC 14888 und 18033, IETF/IRTF-Arbeiten zu TLS, IPsec, S/MIME, OpenPGP, X.509, DNSSEC.
- **Relevanz für OSBA:** Ein Krypto-Inventar ähnelt dem SBOM-Gedanken (Kryptomaterial als Teil der Komponentenkenntnis).

## 9. Personalsicherheit, Zugriffskontrolle, Asset-Management (§ 30 Abs. 2 Nr. 9)

- **Personalsicherheit:** geregelte Einarbeitung, Qualifikation und Vertrauenswürdigkeit prüfen (bei erhöhtem Schutzbedarf ggf. Sicherheitsüberprüfung), laufende Weiterbildung, dokumentierte Zuständigkeiten, Vertretungsregelungen, Regeln für Fremdpersonal.
- **Zugriffskontrolle (IAM):** Identitäts- und Berechtigungsmanagement nach Least Privilege/Need-to-Know, Eindeutigkeit der Kennungen, Funktionstrennung. Risiken: Konten ausgeschiedener Mitarbeitender, fehlende zentrale Übersicht, Rechte-Wildwuchs, schwache oder mehrfach genutzte Passwörter.
- **Asset-Management:** vollständige Inventarisierung aller IT-Assets (Hardware, Software, Daten), Klassifizierung nach Schutzbedarf, klare Zuständigkeiten über den Lebenszyklus, regelmäßige Aktualisierung. Risiko „Shadow IT".
- Das Asset-Management bildet laut BSI die Grundlage für Betrieb und Wartung (siehe Abschnitt 5).

## 10. MFA und gesicherte Kommunikation (§ 30 Abs. 2 Nr. 10)

- Das BSIG nennt Multi-Faktor- oder kontinuierliche Authentifizierung sowie gesicherte Sprach-, Video- und Textkommunikation und ggf. gesicherte Notfallkommunikation.
- Das BSI empfiehlt **Multi-Faktor-Authentisierung** mit Faktoren aus verschiedenen Kategorien (Wissen, Besitz, Biometrie), die nicht unabhängig voneinander angreifbar sind; mehrstufige Anmeldeprozesse gelten als ungeeignet. Ein Vertrauensniveau schreibt das Gesetz nicht vor, die Wahl folgt aus der Risikoanalyse (Orientierung: BSI TR-03107, Niveaus normal, substanziell, hoch).
- **Passkeys** sind aus BSI-Sicht sehr sicher, werden aber im BSIG nicht erwähnt und sind keine Voraussetzung (siehe TR-03188 „Passkey Server").
- Gesicherte Kommunikation: TLS nach aktueller technischer Richtlinie, unsichere Versionen deaktivieren, Konfiguration nach BSI-Mindeststandard, regelmäßig prüfen und dokumentieren.

## 11. Übersicht der Risikomanagementmaßnahmen

- Fasst § 30 Abs. 1 und 2 BSIG zusammen: geeignete, verhältnismäßige, wirksame Maßnahmen gegen Störungen der Verfügbarkeit, Integrität und Vertraulichkeit; gefahrenübergreifender Ansatz (digital und physisch); die zehn Mindestmaßnahmen; Entsprechung zu Art. 21 der Richtlinie.
- Verantwortlich für Umsetzung und Überwachung ist die Geschäftsleitung.

## 12. Meldepflicht (§ 32 BSIG)

- Siehe ausführlich in [docs/nis2.md](../docs/nis2.md). Kernpunkte: 24 h früh, 72 h Folgemeldung, einen Monat nach der 72-h-Meldung Abschlussmeldung; Meldeweg BSI-Portal beziehungsweise MIP-Formular vor der Registrierung; Eingangsbestätigung in der Regel umgehend, spätestens nach 24 h; keine Stornierung; das BSI kann die Information der Nutzer anordnen.
- Zusätzliche Hilfsmittel laut BSI: Anleitung zur Meldung im BSI-Portal, Onepager Meldepflicht, Meldeprozess (PDF-Links zum Zeitpunkt des Abrufs nicht abrufbar).

## 13. Geschäftsleitungsschulung (§ 38 Abs. 3 BSIG)

- Geschäftsleitungen müssen sich regelmäßig schulen lassen. Das Gesetz nennt keine konkreten Vorgaben zu Intervall und Dauer.
- Die BSI-Handreichung (rechtlich nicht verbindlich) empfiehlt eine ausführliche Erstschulung mit regelmäßigen Folgeschulungen, abgestimmt auf Risikoexposition und Einrichtung, sowie eine nachvollziehbare Dokumentation der Teilnahme (Datum, Dauer, Inhalte). Behandelt werden Fragen zu Teilnehmerkreis, Häufigkeit, Format, Anbieter und Inhalten.

## 14. DORA und NIS-2

- Nach BSI hat DORA als sektorspezifischer Rechtsakt (Art. 1 Abs. 2 DORA, Art. 4 NIS-2) Vorrang vor der BSIG-Umsetzung beim Cybersicherheitsrisikomanagement und bei der Meldung erheblicher Vorfälle, **solange und soweit** die DORA-Regeln mindestens gleichwertig sind.
- DORA-Adressaten: die Finanzunternehmen nach DORA Art. 2 Abs. 1 sowie IKT-Dienstleister; Ausnahmen nach Art. 2 Abs. 3. Aufsicht in Deutschland: BaFin.
- Ergänzende Details aus der BSI-FAQ (Registrierungspflicht bleibt, keine Doppelmeldung, konzerninterne IT-Dienstleister) stehen in [docs/nis2.md](../docs/nis2.md).
- **Abweichung:** Das BSI-Paket nennt als Inkrafttreten von DORA den 17.01.2023. Nach Art. 64 der Verordnung ist es der 16.01.2023 (20. Tag nach Veröffentlichung am 27.12.2022); wir folgen dem Verordnungstext.

## 15. ISO/IEC 27001 im Kontext von NIS-2

- **Eine ISO-27001-Zertifizierung reicht allein nicht für NIS-2-Konformität.** Gründe: der Geltungsbereich (Scope) des ISMS ist frei wählbar, das BSIG verlangt die Umsetzung für den gesamten relevanten Einrichtungsbetrieb; ISO erlaubt Risikoakzeptanz und -transfer, das BSIG verlangt umgesetzte, wirksame Maßnahmen; gesetzliche Pflichten wie Meldung (§ 32), Registrierung (§ 33) und Geschäftsleitungshaftung/-schulung (§ 38) kommen in der Norm nicht vor.
- Als Nachweis nach § 61 beziehungsweise § 62 BSIG (Aufsicht bei besonders wichtigen beziehungsweise wichtigen Einrichtungen) kann die Zertifizierung die Anforderungen nur unvollständig abdecken.
- Sie liefert aber ein gutes Fundament: strukturierte Risikoanalyse, Risikobehandlung, Richtlinien, Incident Response, Zugriffssteuerung, Kryptokonzepte, Lieferantenmanagement und kontinuierliche Verbesserung haben große Schnittmengen mit § 30 BSIG.

## 16. Gesundheit (Sektorinformation)

- Erläutert die Betroffenheit im Gesundheitssektor nach den Anlagen 1 und 2 BSIG sowie die Abgrenzung zu Betreibern kritischer Anlagen (die als Teilmenge der besonders wichtigen Einrichtungen gelten und ihre bisherigen Pflichten im Wesentlichen behalten).
- **Hersteller von Medizinprodukten:** Als Hersteller im Sinne der Anlage 2 BSIG gilt nur, wer Medizinprodukte nach Art. 2 Nr. 1 MDR (Verordnung (EU) 2017/745) oder In-vitro-Diagnostika nach Art. 2 Nr. 2 der Verordnung (EU) 2017/746 herstellt. Je nach Produkt kann auch eine Einstufung als Betreiber kritischer Anlagen nach der BSI-KritisV in Betracht kommen; andernfalls ist die Größenschwelle nach § 28 BSIG zu prüfen.
- **Relevanz für OSBA:** Hersteller von Medizinprodukten-Software betrifft der Bezug zu [MDR](../docs/mdr.md) und den Normen IEC 62304 und IEC 81001-5-1.

## 17. Ergänzend: NIS-2 für IT und TK (Durchführungsverordnung (EU) 2024/2690)

- Kein Infopaket, aber eine zugehörige Sektorseite des BSI. Die Durchführungsverordnung gilt seit 07.11.2024 für DNS-Diensteanbieter, TLD-Namenregister, Cloud-Computing-Anbieter, Rechenzentrumsdienste, Inhaltszustellnetze, Anbieter verwalteter Dienste (MSP) und verwalteter Sicherheitsdienste (MSSP), Online-Marktplätze, Suchmaschinen, Plattformen sozialer Netzwerke und Vertrauensdiensteanbieter.
- Sie präzisiert die Mindestanforderungen an die Risikomanagementmaßnahmen (Art. 21 der Richtlinie) und legt fest, wann ein Vorfall nach Art. 23 als erheblich gilt. Die ENISA hat am 26.06.2025 eine Implementation Guidance dazu veröffentlicht.
- Die Mapping-Tabellen in den Infopaketen verwenden diese Durchführungsverordnung als Gliederung, auch für Einrichtungen, die sie rechtlich nicht adressiert.

## Offene Punkte und Beobachtungen

- Die BSI-Seiten sind teilweise inkonsistent (z. B. „30 Tage" statt „einen Monat" bei der Abschlussmeldung auf der Seite „NIS-2-Pflichten", DORA-Inkrafttreten 17.01.2023). Bei Zitaten immer den Gesetzes- oder Verordnungstext gegenprüfen.
- Die Grundschutz-Praktiken und die Stand-der-Technik-Bibliothek werden überarbeitet; Mappings können sich ändern.
- Noch nicht ausgewertet: BSI-Standards 200-1 bis 200-4, TR-02102, TR-03107, UP-KRITIS-Lieferantenanforderungen sowie die verlinkten Hilfsmittel und Onepager. Die TR-03183 ist separat in [bsi-tr-03183.md](bsi-tr-03183.md) zusammengefasst. Falls wir weitere Details für die Seiten zu CRA oder NIS-2 brauchen, lesen wir die jeweils gezielt nach.
