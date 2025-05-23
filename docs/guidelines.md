# Mitarbeit

Wir ermutigen jeden, der Erfahrung mit der einen oder anderen regulatorischen Vorgabe gemacht hat, diese Kenntnis und Erfahung hier einzubringen. Ob es um die Darstellung und Korrektheit der Inhalte oder um geeignete Lösungsansätze geht, alle Inhalte können hier ihren Platz finden. Aber wie läuft das ab?

## Organisatorisches

Wir nutzen das "[Fork & Pull](https://docs.github.com/de/pull-requests/collaborating-with-pull-requests/getting-started/about-collaborative-development-models)"- Modell für die Zusammenarbeit. Um eine Änderung oder Ergänzung beizutragen sind die folgenden Schritte erforderlich:

1. Github-Benutzer [anlegen](https://docs.github.com/de/get-started/start-your-journey/creating-an-account-on-github), bzw, anmelden
2. Repository [Fork erzeugen](https://docs.github.com/de/get-started/exploring-projects-on-github/contributing-to-a-project)
3. Einen Abzweig ([Branch](https://docs.github.com/de/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-and-deleting-branches-within-your-repository)) für die Änderung erzeugen
4. Aus dem Branch den [Pull Reuest starten](https://docs.github.com/de/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork)

Die WorkGroup Security hält [wöchetlich Meetings](/osba-regulatory-monitor/index#meetings) in denen die Pull-Requests gemeinsam diskutiert werden. Wir freuen uns, wenn der Autor zu den Meetings erscheint und ggf. Rückfragen beantworten kann. Dies its jedoch nciht erforderlich. Ist die Änderung/Ergänzung [gut kommentiert](https://docs.github.com/de/pull-requests/collaborating-with-pull-requests/getting-started/helping-others-review-your-changes), bzw. aufbereitet, geht sie auch so sicherlich durch. Sollten Rückfragen bestehen, die sich nicht gleich klären lassen, werden Sie über den PR geklärt. 

## Rechtliches

Wir akzeptieren nur Änderungen oder Beizträge, wenn diese unter der gleichen Lizenz veröffentlich werden, wie das gesamte Repository. Mit der Eröffnung eines Pull-requests gegen dieses Repository, erklärt sich der Autor damit einverstanden, dass er seinen Beitrag unter die Creative-Commons-Non-Commercial-Share-Alike-Lizenz ([CC BY-NC-SA-4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/)) stellt. Zudem stellt er sicher, dass sein Beitrag frei von Rechten Dritter ist.

## Redaktionelles

Eine Idee ist es, die einzelnen Texte in einer grundlegenden Gestaltungsform aufzubereiten, um den Einstieg zu vereinfachen. Dazu gehört die Struktur, wie sie in der Datei `template.md` im Basis-Verzeichnis des Repositories vorgesehen ist. in dem template sind ein paar Fragen verankert, um die Struktur zu erläutern.   

Wir strukturieren den Inhalt derzeit in die drei Bereiche (Töpfe):  

* EU-Regularien
* Non-EU-Regularien (das können auch mehr Bereiche werden, derzeit ist es aber alles in einem) 
* Standards 

Diese Zuordnung erfolgt über die Datei `mkdocs.yaml` im Root-Verzeichnis des Repositories. Dort gibt es einen Tag **nav:** , welcher die Hauptnavigation organisiert. Das können wir im Zuge des Pull Requests nachholen, und muss nicht Bestandteil des PRs sein. 

Als Weiteres Gestaltungsmerkmal nutzen wir Tags (s.u. Design). Daraus wird der Index auf der Vorderseite erstellt. Tags befinden sich am Kopf des templates und lassen sich einfach anpassen. Wir haben einige Tags vorgegeben. Diese kann jedoch auch beliebig erweitert werden, wenn sinnvoll. 

> [!NOTE]
>
> Wir begrüßen Hinweise auf Werkzeuge, die sich als hilfreich zur Bewältigung der Anforderungen erweisen. Jedoch behalten wir uns vor, Hinweise auf Werkzeuge auch abzulehnen, wenn der Bezug zum Nutzen für den Leser nicht klar ersichtlich oder im Vergleich mit bereits bezeichneten Werkzeugen als zu gering zu erachten ist. 

## Optisches

Wir nutzen für diesen Web-Auftritt [Github Pages](https://pages.github.com), das Theme [MKDocs](https://www.mkdocs.org) mit der Erweiterung [material design](https://squidfunk.github.io/mkdocs-material/) von [Martin Donath](https://github.com/squidfunk). Dieses verfügt unter anderem über das Plugin *tags*. Mit Hilfe der **Tags** wird der **Index** organisiert. 

> [!Note]
>
> Die Implementierung des Themes erfolgte mit Hilfe von Python. Das bedeutet für verschachtelete Listen, sie müssen wirklich 4 Characters Einzug haben, damit das Theme die neue Ebene erkennt.   

Wer **Bilder** ergänzen möchte, sollte diese im Ordner `/assets` ablegen. Idealerweise ist der Dateiname sprechend mit Bezug zur Regelung gewählt, sodass eine Dopplung des Namens höchst unwahrscheinlich sein wird.  Eine Referenz auf ein einzubindendes Bild `sprechenderName4CRA.jpg`erfolgt in der Regel mit `/osba-regulatory-monitor/assets/sprechenderName4CRA.jpg`. Unterstütze Formate sind die üblichen Web-Formate wie PNG, JPG oder SVN.

## Fragliches

Für alle Fragen stehen wir jederzeit in den Meetings oder auch via issues im Repo zur Verfügung. wir wollen hier einen Beitrag zur Vereinfachung der wirklich komplexen Regulatorik schaffen. Die Wahl von MD und Github-Pages soll es möglichst simpel halten und Vielen ermöglichen, zu unterstützen. Also keine Scheu, wir antworten gerne. 

Rechtsberatung können und dürfen wir jedoch nicht erteilen! 
