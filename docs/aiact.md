---
tags:
   - ai
   - risk management
   - general
   - documentation
   - processes
---

# EU Artificial Intelligence Act (AI Act)

Der EU AI Act ist die weltweit erste umfassende gesetzliche Regulierung von Künstlicher Intelligenz. Er verfolgt einen risikobasierten Ansatz: Je höher das potenzielle Schadenspotenzial eines KI-Systems, desto strenger die Anforderungen. Ziel ist es, Vertrauen in KI zu schaffen, ohne Innovation unnötig zu bremsen.

## Überblick

* **Segment**: KI-Systeme und KI-Modelle mit allgemeinem Verwendungszweck (GPAI — General Purpose AI Model)
* **Verabschiedet / Veröffentlicht**: 13. März 2024 (EP), 21. Mai 2024 (Rat), veröffentlicht 12. Juli 2024 (ABl. EU)
* **Gültig ab** (stufenweise Anwendung):
  * **2. Februar 2025**: Verbote für unzulässige KI-Praktiken (Titel II)
  * **2. August 2025**: Regelungen für KI-Modelle mit allgemeinem Verwendungszweck (GPAI) und Governance
  * **2. August 2026**: Anforderungen für Hochrisiko-KI-Systeme (Anhang I & III), Transparenzpflichten
  * **2. August 2027**: Vollständige Anwendung, inkl. KI-Systeme in regulierten Produkten
* **Gültig für**:
  * Anbieter (Provider) von KI-Systemen und GPAI-Modellen, die in der EU in Verkehr gebracht werden
  * Betreiber (Deployer) von KI-Systemen, die in der EU eingesetzt werden
  * Importeure und Händler von KI-Systemen
  * Auch für Anbieter außerhalb der EU, sofern der Output in der EU genutzt wird
* **Nicht gültig für**:
  * KI-Systeme, die ausschließlich für militärische oder nationale Sicherheitszwecke entwickelt werden
  * KI-Systeme zur ausschließlich privaten, nicht-gewerblichen Nutzung
  * Open-Source-Modelle (mit Einschränkungen bei Hochrisiko-Verwendung)
* **Grauzone**:
  * Abgrenzung zwischen „KI-System" und klassischer Software (Definition in Art. 3 Nr. 1 und Anhang I)
  * Einordnung von Modellen, die sowohl GPAI als auch Hochrisiko-Anwendungen abdecken
  * Verantwortungsaufteilung zwischen Anbieter und Betreiber bei Feintuning oder Integration



## Zentrale Forderungen

### Verbotene KI-Praktiken (Art. 5)

* KI-Systeme zur unbewussten Beeinflussung von Personen (Subliminal Manipulation)
* Ausnützung von Schwächen vulnerabler Gruppen
* Social Scoring durch staatliche Stellen
* Echtzeit-biometrische Fernidentifikation im öffentlichen Raum (mit engen Ausnahmen für Strafverfolgung)
* Emotionserkennung am Arbeitsplatz und in Bildungseinrichtungen
* Biometrische Kategorisierung zur Ableitung sensibler Merkmale (Rasse, politische Meinung, etc.)

### Hochrisiko-KI-Systeme (Art. 6, Anhang III)

Betroffene Bereiche u.a.: biometrische Identifikation, kritische Infrastruktur, Bildung, Beschäftigung, wesentliche Dienstleistungen (Kredit, Sozialleistungen), Strafverfolgung, Migration, Justiz.

Pflichten für Anbieter von Hochrisiko-KI:

* **Risikomanagementsystem** einrichten und dokumentieren, s. Art. 9
* **Daten-Governance** sicherstellen: Trainings-, Validierungs- und Testdaten müssen geeignet, repräsentativ und frei von unzulässigen Verzerrungen sein, s. Art. 10
* **Technische Dokumentation** erstellen und aktuell halten (s. Art. 11, Anhang IV)
* **Automatische Protokollierung** (Logging) des Systemverhaltens sicherstellen, s. Art. 12
* **Transparenz** gegenüber Betreibern gewährleisten (Gebrauchsanweisung, Zweck, Grenzen), s. Art. 13
* **Menschliche Aufsicht** (Human Oversight) technisch ermöglichen, s. Art. 14
* **Genauigkeit, Robustheit und Cybersicherheit** sicherstellen, s. Art. 15
* **Konformitätsbewertung** durchführen (intern oder durch Dritte), s. Art. 43
* **EU-Konformitätserklärung** ausstellen und CE-Kennzeichen anbringen, s. Art. 47–49
* **Registrierung** in der EU-Datenbank (EUAI-Datenbank), s. Art. 71

### KI-Modelle mit allgemeinem Verwendungszweck / GPAI (Art. 51–56)

* Bereitstellung technischer Dokumentation an nachgelagerte Anbieter
* Einhaltung von Urheberrechts-Verpflichtungen (s. Art. 53 c)
* Veröffentlichung einer Zusammenfassung der Trainingsdaten
* Für Modelle mit **systemischem Risiko** (> 10²⁵ FLOP): Adversarial Testing, Meldung schwerwiegender Vorfälle an die Kommission, Cybersicherheitsmaßnahmen

### Transparenzpflichten (Art. 50)

* KI-generierte Inhalte (Texte, Bilder, Audio, Video) müssen als solche maschinenlesbar gekennzeichnet sein (Watermarking)
* Chatbots müssen sich als KI zu erkennen geben
* Deepfakes müssen kenntlich gemacht werden



## Lösungsansätze & Hilfestellungen

* Die **EU AI Office** (zuständige Behörde der Kommission) veröffentlicht Leitlinien und Codes of Practice, insb. für GPAI-Anbieter
* Das **BSI** und die nationalen Marktüberwachungsbehörden sind die zuständigen Stellen in Deutschland
* Harmonisierte Normen (CEN/CENELEC) für Hochrisiko-KI werden derzeit erarbeitet — bis dahin können ISO/IEC 42001 (AI Management System) und ISO/IEC 23894 (AI Risk Management) als Orientierung dienen
* Für Open-Source-Anbieter: Prüfen, ob das Modell als GPAI mit systemischem Risiko eingestuft werden könnte — dann gelten auch für Open-Source-Anbieter umfangreichere Pflichten

### Tools & Werkzeuge

#### Modell-Dokumentation & Model Cards (Art. 11, 13)

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [Hugging Face Model Cards](https://huggingface.co/docs/hub/model-cards) | Apache-2.0 | Strukturierte Dokumentation von ML-Modellen (Zweck, Limitierungen, Trainingsdaten, Evaluierungsergebnisse) in YAML + Markdown | Art. 13: Transparenz gegenüber Betreibern; Art. 11 + Anhang IV: Technische Dokumentation |
| [Google Model Card Toolkit](https://github.com/google/model-card-toolkit) | Apache-2.0 | Programmatische Erzeugung strukturierter Model Cards inkl. quantitativer Performance-Metriken | Art. 13: Automatisch generierte Transparenz-Dokumentation; Art. 15: Performance-Kennzahlen |
| [ALTAI Self-Assessment](https://futurium.ec.europa.eu/en/european-ai-alliance/pages/altai-assessment-list-trustworthy-artificial-intelligence) | Frei (EU-Kommission) | Online-Selbstbewertungs-Checkliste (96 Fragen) nach den EU Ethics Guidelines for Trustworthy AI | Art. 9: Initialer Gap-Assessment-Einstieg; gute Vorbereitung auf formelle Konformitätsbewertung |

#### Risikobewertung & Risikomanagement (Art. 9)

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [NIST AI RMF Playbook](https://airc.nist.gov/docs/AI_RMF_Playbook.pdf) | Frei (Public Domain) | Strukturiertes Risikomanagement für KI (GOVERN / MAP / MEASURE / MANAGE); Hunderte konkreter Maßnahmen | Art. 9: Iteratives Risikomanagement; lässt sich direkt auf EU AI Act-Artikel mappen |
| [MIT AI Risk Repository](https://airisk.mit.edu/) | Frei (Open Access) | Durchsuchbare Datenbank mit 700+ klassifizierten KI-Risiken nach Ursache und Domäne | Art. 9: Systematische Risikoidentifikation; Abgleich mit Annex III Hochrisiko-Kategorien |

#### Bias-Erkennung & Fairness (Art. 10, 15)

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [Fairlearn](https://github.com/fairlearn/fairlearn) | MIT | Fairness-Metriken (Demographic Parity, Equalized Odds) + Mitigationsalgorithmen für Klassifikatoren und Regression | Art. 10: Disparitäten in Trainingsdaten erkennen; Art. 9: Diskriminierungsrisiko quantifizieren |
| [IBM AI Fairness 360](https://github.com/Trusted-AI/AIF360) | Apache-2.0 | Umfangreiche Bibliothek mit 70+ Fairness-Metriken und 10+ Bias-Mitigationsalgorithmen (Pre/In/Post-Processing) | Art. 10: Pre-Processing gegen Trainingsdaten-Bias; Art. 15: Adversarial Debiasing für Robustheit |
| [Aequitas](https://github.com/dssg/aequitas) | MIT | Bias-Audit-Toolkit mit Gruppen-Disparitäts-Reports; besonders geeignet für Audit-Dokumentation | Art. 9: Audit-ready Disparity Reports für Konformitätsbewertung; Art. 13: Berichtsformat für technische Dokumentation |

#### Erklärbarkeit / XAI (Art. 13)

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [SHAP](https://github.com/shap/shap) | MIT | Modell-agnostische Feature-Attribution via Shapley Values; globale und lokale Erklärungen | Art. 13: Lokale Erklärungen („warum wurde diese Entscheidung getroffen?") für Hochrisiko-KI; Art. 9: Risikotreiber identifizieren |
| [Alibi](https://github.com/SeldonIO/alibi) | Apache-2.0 | Counterfactual Explanations, Anchors, Kernel SHAP; Companion `alibi-detect` für Drift- und Ausreißer-Erkennung | Art. 13: Counterfactuals direkt handlungsrelevant für betroffene Personen; Art. 15: `alibi-detect` für Robustheit im Betrieb |
| [InterpretML](https://github.com/interpretml/interpret) | MIT | Erklärbares Boosting (EBM = Glass-Box-Modell mit GBM-Genauigkeit) + Black-Box-Erklärungen (SHAP, LIME, PDP) | Art. 13: Glass-Box-EBMs bieten inhärente Transparenz ohne Post-hoc-Erklärung — in Konformitätsbewertungen leichter verteidigbar |
| [LIME](https://github.com/marcotcr/lime) | BSD-2-Clause | Lokale Surrogatmodelle für tabellarische, Text- und Bilddaten | Art. 13: Einzelentscheidungserklärungen, insb. für NLP-Modelle |

#### Logging, Experiment-Tracking & MLOps (Art. 12)

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [MLflow](https://github.com/mlflow/mlflow) | Apache-2.0 | End-to-End ML-Lifecycle: Experiment-Tracking, Model Registry mit Stage-Gates, Artefakt-Speicherung | Art. 12: Natürliches Audit-Log für Trainingsläufe, Hyperparameter, Datensatz-Versionen; Anhang IV: Entwicklungsnachweis |
| [DVC](https://github.com/iterative/dvc) | Apache-2.0 | Git-basierte Versionierung von Datensätzen und ML-Pipelines; reproduzierbare Trainingsläufe | Art. 10: Daten-Lineage und -Versionierung; Art. 12: Pipeline-Audit-Trail |
| [Evidently AI](https://github.com/evidentlyai/evidently) | Apache-2.0 | ML-Monitoring-Reports für Daten-Drift, Target-Drift und Modell-Performance im Betrieb; HTML/JSON-Output | Art. 12: Zeitgestempelte Monitoring-Reports als Audit-Artefakte; Art. 15: Drift-Erkennung für Robustheit |

#### Datenqualität & Governance (Art. 10)

| Tool | Lizenz | Problem / Zweck | Regulatorische Relevanz |
|------|--------|-----------------|------------------------|
| [Great Expectations](https://github.com/great-expectations/great_expectations) | Apache-2.0 | Datenvalidierungs-Framework mit definierbaren „Expectations"; erzeugt „Data Docs" als menschenlesbare Validierungsberichte | Art. 10: Nachweis, dass Trainingsdaten definierte Qualitätskriterien erfüllen (Vollständigkeit, Balance, Korrektheit) |
| [Cleanlab](https://github.com/cleanlab/cleanlab) | Apache-2.0 | Automatische Label-Qualitätsprüfung: findet fehlerhafte Labels, Duplikate und Ausreißer in Trainingsdaten | Art. 10: Direkte Umsetzung der Anforderung, dass Trainingsdaten „frei von Fehlern" sein sollen; Art. 15: Saubere Labels verbessern Robustheit |
| [OpenMetadata](https://github.com/open-metadata/OpenMetadata) | Apache-2.0 | Moderner Open-Source-Datenkatalog mit Lineage, Qualitäts-Checks und 50+ Konnektoren | Art. 10: Zentrale Dokumentation der Datenprovenienz; Art. 12: Datenzugriffs-Audit-Log |
