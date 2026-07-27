# Prozess des Herausgebers

## 1. Entwurf prüfen

- Der Standardworkflow übergibt genau eine Datei unter `drafts/` oder ein Einzelauftrag nennt genau eine solche Datei.
- Das Frontmatter ist gültig.
- `status` ist `freigabe` oder `abgeschlossen`.
- Der Artikel besitzt eine Überschrift erster Ebene.

Wenn eine Bedingung nicht erfüllt ist, nicht verschieben und den Grund nennen.

## 2. Frühesten freien Tag bestimmen

- Das heutige lokale Datum in der Zeitzone `Europe/Berlin` verwenden.
- Alle Markdown-Artikel im Stamm des Blog-Repositories prüfen, deren Dateiname mit `YYYY-MM-DD ` beginnt.
- Mit dem heutigen Datum beginnen.
- Ist für dieses Datum bereits mindestens ein Artikel vorhanden, jeweils einen Kalendertag weitergehen.
- Den ersten Tag ohne Artikel verwenden.

Dadurch wird so früh wie möglich veröffentlicht, aber höchstens ein Artikel pro Tag. Es gibt keinen festen Wochenplan und keine künstlichen Pausen.

## 3. Dateinamen bilden

Das Format lautet:

`YYYY-MM-DD Titel.md`

- Das ermittelte Datum verwenden.
- Den Titel aus der ersten `#`-Überschrift übernehmen.
- Keine rückwirkenden Termine vergeben.
- Vor dem Verschieben sicherstellen, dass die Zieldatei nicht existiert.

## 4. Veröffentlichen

- Im Frontmatter `status: veroeffentlicht` setzen.
- Die Datei aus `drafts/` in den Stamm des Blog-Repositories verschieben und dabei den ermittelten Dateinamen vergeben.
- Keine inhaltlichen Änderungen vornehmen.

## 5. Änderung committen

- Vor dem Staging den Git-Status prüfen.
- Ausschließlich den veröffentlichten Artikel und, falls die Quelldatei bereits versioniert war, deren Verschiebung aus `drafts/` stagen.
- Keine anderen geänderten oder unversionierten Dateien aufnehmen.
- Den Titel aus der ersten `#`-Überschrift als Betreff der Commit-Message verwenden.
- Als Commit-Beschreibung knapp festhalten, was tatsächlich passiert ist: welcher Entwurf auf welchen Veröffentlichungstag und Zielpfad übernommen wurde.

Die Commit-Message hat dieses Format:

```text
<Titel des Artikels>

Veröffentlicht am <YYYY-MM-DD>: <Quellpfad> → <Zielpfad>.
```

Wenn keine publikationsbezogene Änderung zu committen ist, nicht committen und den Grund melden.

## 6. Pushen

- Den aktuellen Branch zum bereits konfigurierten Upstream pushen.
- Niemals Force-Push verwenden.
- Schlägt Commit oder Push fehl, nicht ausweichen oder andere Änderungen einbeziehen; den Fehler melden.

## 7. Ergebnis melden

- Quell- und Zielpfad nennen.
- Den vergebenen Veröffentlichungstag nennen.
- Commit-ID und gepushten Branch nennen.
- Bestätigen, dass keine unabhängigen Änderungen committed wurden.
