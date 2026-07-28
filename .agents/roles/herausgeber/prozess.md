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

## 5. Änderungen des Zyklus ermitteln

- Vor dem Staging den Git-Status prüfen.
- Den veröffentlichten Artikel und, falls die Quelldatei bereits versioniert war, deren Verschiebung aus `drafts/` aufnehmen.
- Zusätzlich alle `prozess.md`- und `lernen.md`-Dateien aufnehmen, die eine Rolle nachweislich während dieses Artikelzyklus verändert hat.
- Weitere Dateien dürfen nur aufgenommen werden, wenn ihre Änderung unmittelbar aus diesem Zyklus stammt und für dessen Prozess erforderlich ist.
- Vorhandene Änderungen, deren Herkunft nicht eindeutig diesem Zyklus zugeordnet werden kann, nicht aufnehmen.
- Jede aufzunehmende Datei einzeln stagen; niemals pauschal das gesamte Repository stagen.

## 6. Committen

- Den Titel aus der ersten `#`-Überschrift als Betreff der Commit-Message verwenden.
- Als Commit-Beschreibung knapp festhalten:
  - welcher Entwurf auf welchen Veröffentlichungstag und Zielpfad übernommen wurde,
  - welche Prozess- oder Lerndateien sich durch den Zyklus verändert haben.

Die Commit-Message hat dieses Format:

```text
<Titel des Artikels>

Veröffentlicht am <YYYY-MM-DD>: <Quellpfad> → <Zielpfad>.
Prozess verbessert: <kurze Beschreibung oder "keine Änderung">.
```

Wenn weder eine Veröffentlichungs- noch eine zugehörige Prozessänderung zu committen ist, nicht committen und den Grund melden.

## 7. Pushen

- Den aktuellen Branch zum bereits konfigurierten Upstream pushen.
- Niemals Force-Push verwenden.
- Schlägt Commit oder Push fehl, nicht ausweichen oder andere Änderungen einbeziehen; den Fehler melden.

## 8. Ergebnis melden

- Quell- und Zielpfad nennen.
- Den vergebenen Veröffentlichungstag nennen.
- Commit-ID und gepushten Branch nennen.
- Die mitgeführten Prozess- und Lerndateien nennen.
- Bestätigen, dass keine unabhängigen Änderungen committed wurden.
