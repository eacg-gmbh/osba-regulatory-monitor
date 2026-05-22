# TrustSource & EU AI Act — Analyse und Positionierung

*Erstellt: 2026-05-22 | Grundlage: Regulation (EU) 2024/1689 (EU AI Act)*

---

## 1. Ist TrustSource selbst ein KI-System im Sinne des AI Acts?

### Definition KI-System (Art. 3 Nr. 1 AI Act)

Ein KI-System ist ein maschinenbasiertes System, das aus Eingaben **ableiten** kann, wie es Ausgaben wie Vorhersagen, Empfehlungen oder Entscheidungen erzeugt, die Umgebungen beeinflussen können, und dabei einen gewissen Grad an **Autonomie** aufweist. Klassische regelbasierte Software, Datenbankabfragen und deterministische Filterung gelten ausdrücklich **nicht** als KI-Systeme.

### Bewertung der TrustSource-Kernfunktionen

| Funktion | KI-Anteil | Einordnung |
|----------|-----------|------------|
| SBOM-Erstellung und -Verwaltung | Keiner (automatisierte Extraktion aus Abhängigkeitsgraphen) | Kein KI-System |
| Vulnerability-Matching (CVE/NVD-Abgleich) | Keiner (Datenbank-Lookup, regelbasiert) | Kein KI-System |
| CVSS-Scoring | Keiner (deterministisches Berechnungsschema) | Kein KI-System |
| EPSS-basierte Priorisierung | **Grenzfall**: EPSS nutzt ein ML-Modell (Gradient Boosting), das Ausnutzungswahrscheinlichkeit vorhersagt | Potenziell KI-System, wenn als autonome Empfehlung ausgegeben |
| Lizenz-Compliance-Analyse | Regelbasiert (Lizenzdatenbank + Kompatibilitätsmatrix) | Kein KI-System |

### Fazit

**TrustSource ist in seiner Kernfunktion kein KI-System im Sinne des AI Acts.** Die primären Funktionen sind regelbasiert und deterministisch.

Ein **Grenzfall besteht bei der EPSS-Integration**: EPSS ist ein extern entwickeltes ML-Modell (Anbieter: FIRST.org). Solange TrustSource EPSS-Scores als Rohdaten weitergibt, liegt das KI-System beim Modellanbieter, nicht bei TrustSource. Sobald TrustSource autonome Priorisierungsempfehlungen auf Basis von EPSS ableitet, wäre eine erneute rechtliche Prüfung erforderlich.

**Falls doch als KI-System eingestuft: wahrscheinlichste Risikokategorie ist Minimal Risk** — Vulnerability-Priorisierung für Software-Entwickler fällt nicht in die Hochrisiko-Kategorien des Anhang III (biometrische Identifikation, kritische Infrastruktur, Beschäftigung, Kredit, Strafverfolgung etc.).

---

## 2. Was bedeutet der AI Act für TrustSource-Kunden?

Kunden, die selbst KI-Systeme entwickeln, sind als **Anbieter von KI-Systemen** unmittelbar dem AI Act unterworfen. Dabei entstehen direkte Berührungspunkte mit TrustSource:

### Hochrisiko-KI-Pflichten und TrustSource-Unterstützung

| AI-Act-Pflicht | Artikel | Wie TrustSource helfen kann |
|----------------|---------|----------------------------|
| Technische Dokumentation der Systemarchitektur | Art. 11, Anh. IV | SBOM als maschinenlesbarer Beleg aller Softwarekomponenten des KI-Systems |
| Cybersicherheit: Schutz vor bekannten Schwachstellen | Art. 15 | Kontinuierliches Vulnerability-Monitoring aller KI-Abhängigkeiten (PyTorch, TensorFlow, Transformers etc.) |
| Post-Market Monitoring | Art. 72 | Laufende CVE-Überwachung nach Deployment als Teil des gesetzlich geforderten Post-Market-Monitoring |
| Compliance-Nachweis gegenüber Behörden | Art. 43, 71 | SBOM-Exports als Nachweisdokumentation für Konformitätsbewertung |
| Lieferketten-Sicherheit (Drittanbieter) | Art. 25 | Abhängigkeitsanalyse für KI-Frameworks und Open-Source-Bibliotheken |

### KI-Systeme haben Open-Source-Abhängigkeiten

KI-Systeme sind komplexe Softwareprodukte mit tiefen Abhängigkeiten: Python-Frameworks (TensorFlow, PyTorch, scikit-learn, Hugging Face Transformers), Datenverarbeitungsbibliotheken (pandas, NumPy), API-Clients, Container-Images. Diese Abhängigkeiten erzeugen:

- **Schwachstellen-Risiken**: Ein kompromittiertes Open-Source-Paket in einem Hochrisiko-KI-System verletzt Art. 15 (Cybersicherheit)
- **Lizenz-Compliance-Risiken**: Copyleft-Lizenzen (GPL) in kommerziellen KI-Produkten erzeugen rechtliche Haftung
- **Dokumentationspflichten**: Anhang IV verlangt Beschreibung der Systemarchitektur inkl. verwendeter Frameworks

---

## 3. Positionierung und Chancen

### 3.1 Kurzfristig: Bestehende Stärken im AI-Act-Kontext positionieren

**SBOM als Compliance-Artefakt für Hochrisiko-KI (ab August 2026)**

Art. 11 + Anhang IV fordern eine Beschreibung der Systemkomponenten und ihrer Interaktionen. Eine vollständige SBOM im CycloneDX- oder SPDX-Format ist de facto ein Kernbestandteil der technischen Dokumentation für Hochrisiko-KI. TrustSource sollte dies explizit kommunizieren:

> *„TrustSource SBOMs erfüllen die Dokumentationsanforderungen des EU AI Act Art. 11 + Anhang IV für Hochrisiko-KI-Systeme."*

**Continuous Vulnerability Monitoring als Art.-15-Nachweis**

Art. 15 fordert Cybersicherheit über den gesamten Lebenszyklus. Laufendes CVE-Monitoring mit Zeitstempeln, Statusänderungen und Remediierungs-Tracking ist ein direkter Nachweis. Empfehlung: AI-Act-spezifische Report-Exports einführen, die SBOM-Einträge auf konkrete Artikel mappen.

**Post-Market Monitoring (Art. 72) automatisieren**

Art. 72 verpflichtet Anbieter von Hochrisiko-KI zu einem Post-Market-Monitoring-System. Kontinuierliches CVE-Monitoring durch TrustSource erfüllt einen wesentlichen Teil dieser Anforderung — dieses Argument sollte in der Vermarktung genutzt werden.

### 3.2 Mittelfristig: AI Bill of Materials (AIBOM)

Das größte strategische Wachstumsfeld: Der AI Act — insbesondere für GPAI-Anbieter (Art. 53, Anhang XI) — fordert technische Dokumentation, die weit über klassische Software-SBOMs hinausgeht. Ein vollständiges **AI Bill of Materials (AIBOM)** nach CycloneDX ML-BOM v1.7 umfasst:

| AIBOM-Komponente | Inhalt | AI-Act-Relevanz |
|------------------|--------|-----------------|
| **Models** | Basismodell, Feintuning-Checkpoint, Version, Herkunft (Hugging Face, proprietär) | Art. 11, Art. 53 Anh. XI |
| **Datasets** | Trainingsdaten, Validierungsdaten, Testdaten — Herkunft, Lizenz, Größe | Art. 10, Art. 53 (Trainings-Zusammenfassung) |
| **Code** | Trainings-Code, Inference-Code, Preprocessing-Pipelines, alle OS-Abhängigkeiten | Art. 11, CRA |
| **Hardware** | GPU-Typen, Cloud-Provider, Recheninfrastruktur | Art. 11 |
| **Data Processing Pipelines** | Datenverarbeitungsketten, verwendete Bibliotheken | Art. 10, 11 |
| **Governance** | Verantwortlichkeiten, Freigabeprozesse, Änderungshistorie | Art. 9, 11 |

TrustSource hat mit dem bestehenden SBOM-Framework die technische Grundinfrastruktur für AIBOM-Funktionalität. Die bestehende CycloneDX-Unterstützung ist kompatibel mit CycloneDX ML-BOM v1.7.

**Konkreter Erweiterungsvorschlag:** Ein „AI Module" für TrustSource-Projekte, das zusätzlich zu Software-Komponenten auch ML-Modelle (Basismodell + Version + Quelle), Trainingsdatensätze (Name, Herkunft, Lizenz) und Feintuning-Checkpoints verwaltet — und diese gegen bekannte Modell-Vulnerabilities abgleicht (Modell-CVEs sind zunehmend in NVD erfasst, z.B. Pickle-Deserialisierungsprobleme).

**Modell-Vulnerability-Tracking:** Aufbau einer Datenbank für Modell-spezifische Schwachstellen (Pickle-Exploits, Prompt-Injection-Klassen, Backdoor-Angriffe auf Modelle) — analog zur bestehenden CVE-Integration.

### 3.3 Langfristig: Multi-Regulation-Compliance-Suite

**GPAI-Compliance-Suite (ab 2027):** Für Kunden, die GPAI-Modelle entwickeln — Trainings-Zusammenfassung (Art. 53), Technische Dokumentation (Anhang XI), Adversarial-Testing-Nachweise (Art. 55) als integrierter Workflow.

**Multi-Regulation-Dashboard:** Unified View, der zeigt, ob ein Projekt-SBOM gleichzeitig AI Act, CRA, NIS2 und DORA-relevante Lücken hat — strategischer Differenziator gegenüber Single-Regulation-Tools.

---

## 4. PSIRT-Beratung durch EACG im AI-Act-Kontext

Die PSIRT-Beratung der EACG erhält durch den AI Act neuen regulatorischen Rückenwind:

| AI-Act-Anforderung | Artikel | PSIRT-Relevanz |
|--------------------|---------|----------------|
| Meldung schwerwiegender Vorfälle (GPAI mit systemischem Risiko) | Art. 55 | PSIRT-Prozesse sind hierfür unverzichtbar |
| Meldepflichten bei Hochrisiko-KI-Vorfällen | Art. 73 | Erfordert PSIRT-ähnliche interne Prozesse (BSI als nationale Behörde) |
| Post-Market Monitoring | Art. 72 | Systematische Überwachung nach Deployment — PSIRT-Expertise direkt anwendbar |
| CRA-Überschneidung: Vulnerability Handling, Security Updates | CRA Art. 13–14 | PSIRT-Strukturen für KI-Produkte erforderlich |

EACG kann PSIRT-Aufbau und -Betrieb für KI-Unternehmen anbieten, die gleichzeitig AI Act und CRA erfüllen müssen — ein stark wachsendes Marktsegment ab August/September 2026.

---

## 5. Kritische Zeitlinien für TrustSource-Kunden

| Datum | Ereignis | Handlungsbedarf |
|-------|----------|-----------------|
| **2. Feb. 2025** | Verbote (Art. 5) gelten | Prüfen, ob Kunden verbotene KI-Praktiken einsetzen |
| **2. Aug. 2025** | GPAI-Pflichten gelten (Art. 53, 55) | Kunden mit GPAI-Modellen müssen Dokumentation und CVD-Prozesse aufbauen |
| **Sep. 2026** | CRA gilt parallel | Integrierter SBOM+Vuln-Prozess für KI-Produkte notwendig |
| **2. Aug. 2026** | Hochrisiko-KI-Pflichten gelten (Art. 9–15, 43, 71) | Vollständige Compliance für alle Hochrisiko-KI-Anbieter |
| **2. Aug. 2027** | Vollständige Anwendung (inkl. Anhang-I-Produkte) | KI in Maschinen, Medizinprodukten, Fahrzeugen vollständig reguliert |

---

## 6. Empfehlungen

1. **Sofort**: Marketing-Materialien aktualisieren — SBOM und CVE-Monitoring explizit als AI-Act-Compliance-Artefakte (Art. 11, 15, 72) positionieren
2. **Q3 2026**: AI-Act-spezifische Report-Templates einführen (Mapping von SBOM-Einträgen auf AI-Act-Artikel)
3. **2026**: AIBOM-Konzept evaluieren — Pilotprojekt mit einem KI-entwickelnden Kunden
4. **2026**: PSIRT-as-a-Service für KI-Unternehmen als kombiniertes EACG-Angebot (AI Act + CRA) entwickeln
5. **Rechtliche Klarstellung**: Formale Prüfung durch einen auf AI Act spezialisierten Rechtsanwalt, ob die EPSS-Integration eine KI-System-Einordnung begründet

---

*Quellen: Regulation (EU) 2024/1689 ([EUR-Lex](https://eur-lex.europa.eu/legal-content/DE/TXT/?uri=CELEX%3A32024R1689)), [artificialintelligenceact.eu](https://artificialintelligenceact.eu), FIRST.org EPSS, CycloneDX ML-BOM v1.7*
