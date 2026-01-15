# Eudaimonica – Narrative World Model Tweet Generator

## Metadata

- **Version**: 2.1
- **Erstellt**: 2025-12-21
- **Zweck**: Inspirierende Tweets zur Etablierung und Erinnerung des Eudaimonica-Weltmodells
- **Output**: JSON-Datei mit so vielen Tweets wie der Text sinnvolle Ideen hergibt
- **Funktion**: Öffentliche Beschreibung einer bewohnbaren, stimmigen Welt

---

## Prompt

Du erstellst Tweets, die **das Eudaimonica-Weltmodell beschreiben**.

Die Tweets:

- erklären nichts
- fordern nichts
- argumentieren nicht
- überzeugen nicht

Sie **zeigen**, wie diese Welt funktioniert —
so ruhig und selbstverständlich, dass Inspiration von selbst entsteht.

---

## Ton & Haltung (entscheidend)

- ruhig
- klar
- warm
- zugewandt
- inspirierend durch Stimmigkeit

Nicht:

- motivierend
- pushend
- belehrend
- missionierend

Die Sätze dürfen **tragen**, nicht ziehen.

---

## Sprachliche Leitplanken

### Verwenden

- beschreibende, positive Feststellungen
- sanfte Ursache–Wirkung
- Begriffe aus der Philosophie:
  - Gleichgewicht
  - Signale
  - Versorgung
  - Sicherheit
  - Aufgabe
  - Passung
  - Energie
- klare, einfache Sprache

### Vermeiden

- Ich / Wir
- Fragen
- Imperative
- Meta-Kommentare
- Rechtfertigungen

---

## Inhaltlicher Fokus (Eudaimonica-Kern)

Beschreibe eine Welt, in der:

- Versorgung den Zwang ersetzt
- Sicherheit klare Signale ermöglicht
- Gleichgewicht wichtiger ist als Wachstum
- Motivation aus Passung entsteht
- Handlung mühelos wird, wenn Grundlagen stimmen
- Erfüllung ein Signal funktionierender Systeme ist

Nicht als Ideal —
sondern als **gelebte Realität dieses Weltmodells**.

---

## Formale Vorgaben

- **So viele Tweets wie der Text sinnvolle Ideen hergibt**
- < 280 Zeichen
- 0–1 Emoji optional (sparsam, warm)
- 0–2 dezente Hashtags (z. B. #Eudaimonia #Gleichgewicht)
- Keine Interaktionsmarker

---

## Zeitplan

Ein Gedanke pro Tag.
Raum zum Nachwirken lassen.

Bei N Tweets: Tag 0 bis Tag N-1
(z.B. 5 Tweets → Tag 0, 1, 2, 3, 4)

---

## Beispiel-Output (inspirierend, weltmodellierend)

```json
[
  {
    "date": "2025-11-16",
    "message": "Wo Grundversorgung gesichert ist, verliert Eile ihre Macht. Entscheidungen werden ruhiger, weiter und erstaunlich leicht."
  },
  {
    "date": "2025-11-17",
    "message": "Sicherheit ist kein Luxus. Sie ist die Voraussetzung dafür, dass Signale klar werden und Energie wieder sinnvoll fließt. 🌱"
  },
  {
    "date": "2025-11-18",
    "message": "In funktionierenden Systemen entsteht Motivation nicht durch Druck, sondern durch Passung zwischen Aufgabe und Fähigkeit. #Eudaimonia"
  }
]
```

---

**VORGEHEN:**

1. Analysiere den Blogartikel gründlich und identifiziere alle wesentlichen Ideen und Konzepte
2. Erstelle für jede eigenständige, wesentliche Idee einen wertvollen Tweet
3. Bewerte realistisch: Wie viele einzigartige, substanzielle Tweets lassen sich aus dem Text ziehen?
4. Sorge für thematische Diversität - verschiedene Blickwinkel und Aspekte abdecken
5. Verteile die Tweets auf aufeinanderfolgende Tage (1 Tweet pro Tag, beginnend ab Tag 0)
6. Formatiere als JSON-Array
7. Speichere die Datei als `[ARTIKELNAME].json` ohne `.md` im Verzeichnis `tweets/posts/`

---

## Qualitätssicherung (philosophisch)

- [ ] Der Tweet zeigt eine Welt, kein Argument
- [ ] Er fühlt sich ruhig und weit an
- [ ] Er erzeugt Orientierung, nicht Druck
- [ ] Er passt organisch in Eudaimonica
- [ ] Er könnte auch in 10 Jahren noch stehen
- [ ] JSON ist valide
