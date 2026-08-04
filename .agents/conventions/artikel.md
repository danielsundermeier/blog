# Artikelformat

Jeder neue Entwurf beginnt mit diesem YAML-Frontmatter:

```yaml
---
beschreibung: ""
was_ist_gut: []
was_kann_ueberarbeitet_werden: []
ton:
  ziel: ""
  bewertung: ""
dramaturgie:
  ziel: ""
  bewertung: ""
status: entwurf
iteration: 1
---
```

Danach folgt der Artikel:

```markdown
# Titel

Text
```

## Verantwortlichkeiten

Der Autor setzt:

- `beschreibung`
- `ton.ziel`: die beabsichtigte Wirkung und Haltung des Textes
- `dramaturgie.ziel`: Beobachtung, gemeinsame Entdeckungsreise, Erkenntnis und Rückkehr zur Beobachtung
- `status`
- `iteration`

Der Editor setzt oder aktualisiert:

- `was_ist_gut`
- `was_kann_ueberarbeitet_werden`
- `ton.bewertung`
- `dramaturgie.bewertung`
- `status`

## Statuswerte

- `entwurf`: noch nicht bewertet
- `ueberarbeitung`: der Editor verlangt Änderungen
- `freigabe`: keine wesentlichen Änderungen mehr erforderlich
- `abgeschlossen`: dritte Iteration erreicht; der lesbare und verständliche Stand beendet den Zyklus
- `blockiert`: dritte Iteration erreicht, aber der Text ist noch nicht ausreichend lesbar und verständlich
- `veroeffentlicht`: der freigegebene Entwurf wurde mit seinem Veröffentlichungstermin in den Blog-Stamm verschoben

## Regeln

- Listen bleiben Listen, auch wenn sie leer sind.
- Bewertungen müssen konkret und am Text nachvollziehbar sein.
- `iteration` darf höchstens den Wert `3` erreichen.
- Nach der dritten Iteration wird keine weitere Überarbeitung dieses Zyklus begonnen.
- Maßstab für den Abschluss ist ein lesbarer und verständlicher Text, nicht Perfektion.
- Nur `freigabe` und `abgeschlossen` dürfen an den Herausgeber übergeben werden.
- `ton.bewertung` prüft insbesondere, ob der Text inspiriert, ohne zu belehren.
- `dramaturgie.bewertung` prüft insbesondere die logische Gedankenkette und ob der Kreis zur anfänglichen Beobachtung geschlossen wird.
- Frühere Bewertungen dürfen bei einer neuen Iteration ersetzt werden;
  relevante neue Lernerfahrung wird separat in der gegenstandsbezogenen
  Lerndatei des Artikels festgehalten.
- Verknüpfungen zu Knowledge oder anderen Holons sind noch nicht Bestandteil dieses Formats.
