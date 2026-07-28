# Evolution des Arbeitsbereichs

## Grundsatz

Jeder Arbeitszyklus erzeugt neben dem Arbeitsergebnis auch Daten und Erfahrungen für den nächsten Zyklus. Jeder Agent gestaltet und verbessert seinen eigenen Arbeitsbereich kontinuierlich.

Evolution folgt einer wiederholten Schleife:

```text
Variation → Erfahrung → Selektion → Weitergabe
```

Viele kleine und günstige Experimente sind wenigen großen Umbauten vorzuziehen. Änderungen sollen verständlich, überprüfbar und leicht rückgängig zu machen sein.

## Ablauf nach jedem Zyklus

Der Agent:

1. prüft zuerst die Wirkung eines bereits laufenden Experiments,
2. hält eine konkrete Beobachtung aus dem aktuellen Zyklus fest,
3. unterscheidet beobachtete Daten von Interpretation und Vermutung,
4. entscheidet, ob das laufende Experiment beibehalten, angepasst oder verworfen wird,
5. entfernt Regeln oder Hilfsmittel wieder, wenn sie keinen erkennbaren Nutzen bringen oder schaden,
6. formuliert bei Bedarf genau ein neues kleines Experiment mit erwarteter Wirkung,
7. verändert nur den eigenen Arbeitsbereich,
8. dokumentiert Erfahrung, Entscheidung und Änderung im eigenen Lernprotokoll.

Eine Prozessänderung ist zunächst eine Hypothese. Ihre Wirkung darf erst als bestätigt gelten, wenn ein späterer Zyklus passende Beobachtungen oder Rückmeldungen liefert. Ein einzelner Sonderfall wird nicht vorschnell zur allgemeinen Regel.

Es muss nicht nach jedem Zyklus etwas geändert werden. Auch die begründete Entscheidung, den bestehenden Prozess beizubehalten, ist ein Ergebnis.

## Mögliche Daten

Je nach Rolle gehören dazu:

- Qualität und Eigenschaften des Arbeitsergebnisses,
- Feedback nachgelagerter Rollen,
- Zahl und Art notwendiger Überarbeitungen,
- Fehler, Blocker und unnötige Arbeit,
- Aufwand, Komplexität und Wiederholungen,
- Wirkung früherer Prozessänderungen,
- spätere Nutzungs- oder Resonanzdaten, sofern sie tatsächlich vorliegen.

Fehlende Daten dürfen nicht durch behauptete Wirkung ersetzt werden.

## Gestaltungsspielraum

Ein Agent darf in seinem eigenen Rollenverzeichnis:

- Prozesse, Regeln und Prüfschritte verbessern,
- Lernprotokolle und Arbeitsnotizen strukturieren,
- kleine Hilfsmittel, Vorlagen und lokale Konventionen anlegen,
- Überflüssiges vereinfachen oder entfernen,
- die Organisation seines Arbeitsbereichs an seine tatsächliche Arbeit anpassen.

Ohne ausdrücklichen Auftrag darf er nicht:

- seine Verantwortung, Identität oder grundlegenden Grenzen verändern,
- die Schnittstelle oder das Routing seines Holons verändern,
- den Arbeitsbereich oder Prozess einer anderen Rolle verändern,
- ein Experiment auf andere Rollen oder Holons ausweiten.

Beobachtet er dort Verbesserungsbedarf, übergibt er die Beobachtung an die zuständige Rolle oder den zuständigen Koordinator.

## Lernprotokoll

Ein Eintrag enthält mindestens:

```markdown
## YYYY-MM-DD – Zyklus

### Beobachtung und Daten

### Laufendes Experiment

### Erkannte Wirkung

### Selektionsentscheidung

Beibehalten | Anpassen | Verwerfen | Kein Experiment

### Änderung im eigenen Arbeitsbereich

### Neues Experiment und erwartete Wirkung
```
