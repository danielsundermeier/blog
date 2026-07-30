# Liegengebliebene Blog-Arbeitsgegenstände nachholen

## Eingang

Ein ausdrücklicher menschlicher Auftrag verlangt, noch nicht abgeschlossene
Arbeitsgegenstände des Blog-Holons weiterzuverarbeiten.

## Inventur

1. Sichtbare Dateien unter `drafts/` sowie weitere Blogartikel mit einem
   Frontmatter-`status` erfassen.
2. Bereits veröffentlichte Artikel und Dateien ohne erkennbaren Artikelstatus
   außerhalb von `drafts/` nicht als Rückstand behandeln.
3. Für jeden Rückstand ausschließlich Pfad, `status`, `iteration` und vorhandene
   Editor-Änderungswünsche zur Übergabe bestimmen. Den Artikel nicht selbst
   schreiben oder bewerten.

## Routing je Arbeitsgegenstand

- Fehlendes oder ungültiges Artikel-Frontmatter unter `drafts/`: über
  `.agents/roles/autor/AGENTS.md` an den Autor übergeben.
- `status: entwurf`: über `.agents/roles/editor/AGENTS.md` an den Editor
  übergeben.
- `status: ueberarbeitung`: samt Editor-Feedback über
  `.agents/roles/autor/AGENTS.md` an den Autor übergeben.
- `status: freigabe` oder `status: abgeschlossen`: über
  `.agents/roles/herausgeber/AGENTS.md` an den Herausgeber übergeben.
- `status: blockiert`: nicht weitergeben, sondern den dokumentierten Grund
  melden.
- Unbekannter Status: nicht eigenmächtig deuten, sondern als Blocker melden.

Vor jeder Übergabe die verlinkte `AGENTS.md` der zuständigen Rolle vollständig
lesen. Die Rolle führt ihren eigenen bestehenden Prozess aus. Nach ihrer
Rückgabe den neuen Status erneut routen, bis der Arbeitsgegenstand veröffentlicht
oder konkret blockiert ist. Keine vierte Autor-Iteration beginnen.

Mehrere Rückstände werden einzeln und in stabiler Pfadreihenfolge verarbeitet,
damit Status, Änderungen und Übergaben eindeutig einem Arbeitsgegenstand
zugeordnet bleiben. Grenzen des Koordinators werden nicht auf nachgelagerte
Rollen übertragen; jede Rolle führt ihre eigene Verantwortung und ihren eigenen
Prozess vollständig aus.

## Abschluss

1. Für jede gefundene Datei Übergaben, Ergebnis und mögliche Blocker festhalten.
2. Den eigenen Durchgang nach `../../conventions/evolution.md` auswerten und in
   `lernen.md` dokumentieren.
3. Bestätigen, dass veröffentlichte Artikel und unabhängige Änderungen
   unangetastet blieben.

## Grenzen

- Der Koordinator übernimmt keine Facharbeit von Autor, Editor oder
  Herausgeber.
- Er leitet keinen Rückstand allein aus Alter, Thema oder Verzeichnisnamen ab.
- Er verändert keine anderen Holons.
