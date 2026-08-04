# Gespräch als Blogartikel verarbeiten

## Eingang

Ein vollständiges Gespräch ist referenziert.

## Ablauf

1. `.agents/roles/autor/AGENTS.md` vollständig lesen und das Gespräch an den Autor übergeben.
2. Den entstandenen Entwurf über `.agents/roles/editor/AGENTS.md` an den Editor übergeben.
3. Verlangt der Editor eine Überarbeitung, den Entwurf samt Feedback wieder über `.agents/roles/autor/AGENTS.md` übergeben.
4. Autor und Editor höchstens drei Autor-Iterationen durchlaufen lassen.
5. Bei `status: freigabe` oder `status: abgeschlossen` den Entwurf über `.agents/roles/herausgeber/AGENTS.md` übergeben.
6. Bei `status: blockiert` den Herausgeber nicht aufrufen und den Grund melden.
7. Den eigenen Durchgang nach `../../conventions/evolution.md` auswerten und
   nur relevante neue Erfahrung gegenstandsbezogen unter `lernen/` festhalten.
8. Nach einer Veröffentlichung eine Creator-Rückgabe mit Artikelpfad,
   referenziertem Gespräch und den konkreten Beobachtungen von Autor und Editor
   erstellen. Abgeleitete Formulierungen nicht als neue unabhängige Quelle
   darstellen.
9. Die Creator-Rückgabe dem aufrufenden Holon als Teil des Ergebnisses
   übergeben. Der Blog-Koordinator verändert d15r oder die Soul nicht selbst.
10. Mit veröffentlichtem Artikel, Commit und Push, Creator-Rückgabe oder dem
    konkreten Blocker abschließen.

## Grenze

Wie eine Rolle ihren Schritt ausführt, bestimmt ausschließlich ihre eigene `AGENTS.md` und der dort verlinkte Prozess.
