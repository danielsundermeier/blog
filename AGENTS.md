# Blog

Blog entwickelt aus Gesprächen eigenständige Artikel.

## Routing

Die Arbeit besteht zunächst aus zwei aufeinanderfolgenden Holons:

1. `holons/autor/` schreibt oder überarbeitet den Artikel.
2. `holons/editor/` bewertet den Artikel und gibt strukturiertes Feedback.

Nach dem Schreibzyklus steht ein drittes Holon bereit:

3. `holons/herausgeber/` verschiebt einen freigegebenen Entwurf mit dem frühesten freien Datum in den Blog.

Im Standardworkflow übernimmt der Herausgeber automatisch, sobald der Autor-Editor-Zyklus abgeschlossen ist und der Text die Mindestanforderungen erfüllt.

Jedes Holon liest vor seiner Arbeit seine eigene `AGENTS.md` und seinen eigenen `prozess.md`.
Kein Holon verändert den Prozess des anderen.

Das gemeinsame Artikelformat steht in `format/artikel.md`.

## Zyklus

```text
Gespräch
   ↓
Autor schreibt Entwurf
   ↓
Editor bewertet Entwurf
   ↓
Autor überarbeitet anhand des Feedbacks
   ↓
neue Bewertung
```

Ein Zyklus umfasst höchstens drei Autor-Iterationen.

Er endet, sobald der Text lesbar und verständlich ist, spätestens jedoch nach der dritten Iteration. Der Text muss nicht perfekt sein. Offene Verbesserungsmöglichkeiten werden als Erfahrung für kommende Texte genutzt, statt denselben Text unbegrenzt weiterzuarbeiten.

Ist der Text nach der dritten Iteration nicht lesbar und verständlich, setzt der Editor `status: blockiert`. Der Herausgeber wird dann nicht aktiv.

Nach jedem vollständigen Zyklus wertet jedes Holon ausschließlich seine eigene Arbeit aus und verbessert seinen eigenen Prozess. Änderungen müssen in seinem eigenen Lernprotokoll begründet werden.

Die Perfektion liegt im lernenden Prozess: Jeder abgeschlossene Text liefert Erfahrungen, durch die der nächste Text besser werden kann.

## Standardworkflow

Bei einem neuen Gespräch wird der vollständige Ablauf ausgeführt:

1. Autor erstellt den Entwurf.
2. Editor bewertet ihn.
3. Autor und Editor wiederholen ihre Schritte bei Bedarf, höchstens bis Iteration 3.
4. Bei `status: freigabe` oder `status: abgeschlossen` übernimmt der Herausgeber automatisch.
5. Bei `status: blockiert` endet der Ablauf in `drafts/` und der Grund wird gemeldet.

Der Standardworkflow endet erst nach Übernahme, Commit und Push durch den Herausgeber oder mit einem blockierten Entwurf.

## Einzelne Rollen aufrufen

Jede Rolle kann ausnahmsweise einzeln beauftragt werden:

- `Autor`: erstellt oder überarbeitet nur einen Entwurf und stoppt danach.
- `Editor`: bewertet nur den genannten Entwurf und stoppt danach.
- `Herausgeber`: übernimmt, committed und pusht nur den genannten freigegebenen oder abgeschlossenen Entwurf.

Bei einem Einzelauftrag keine nachfolgende Rolle automatisch starten.

## Herausgeber

Bei einem Auftrag wie „Veröffentliche `drafts/datei.md`“:

1. `holons/herausgeber/AGENTS.md` vollständig lesen.
2. `holons/herausgeber/prozess.md` vollständig lesen.
3. Nur den genannten Entwurf verarbeiten.

## Grenzen

- Keine vorhandenen veröffentlichten Artikel überschreiben.
- Neue, ungeprüfte Artikel unter `drafts/` speichern.
- Keine Änderungen an Knowledge oder d15r.
- Keine Tweets erstellen.
- Entwürfe nach einem abgeschlossenen Standardworkflow oder einem ausdrücklichen Einzelauftrag durch den Herausgeber übernehmen.
- Autor und Editor erstellen keine Commits oder Pushes.
- Der Herausgeber committed und pusht ausschließlich die von ihm veröffentlichte Artikeländerung nach seinem eigenen Prozess.
- Bestehende, nicht zur Aufgabe gehörende Änderungen bleiben unangetastet.
