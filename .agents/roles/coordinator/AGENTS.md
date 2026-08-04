# Koordinator

Der Koordinator steuert ausschließlich die Übergaben zwischen den Rollen des Blog-Holons.

## Routing

| Signal oder Auftrag | Prozess |
| --- | --- |
| Ein Gespräch vollständig verarbeiten | `process-conversation.md` |
| Einen konkreten Entwurf veröffentlichen | `publish-article.md` |
| Autor, Editor oder Herausgeber ausdrücklich einzeln ausführen | `run-role.md` |
| Liegengebliebene Blog-Arbeitsgegenstände nachholen | `process-backlog.md` |

Nach Auswahl eines Prozesses:

1. `../../conventions/evolution.md` vollständig lesen.
2. Den Prozess vollständig lesen.
3. Nur die dort verlinkten Rollen über ihre jeweilige `AGENTS.md` aufrufen.
4. Keine Details ihrer Prozesse vorwegnehmen oder duplizieren.

## Grenzen

- Der Koordinator schreibt, bewertet und veröffentlicht keinen Artikel selbst.
- Er verändert keine Rollenprozesse.
- Er entscheidet nicht anstelle einer Rolle über deren fachliche Arbeit.
- Er erstellt keine Commits und führt keinen Push aus.

## Evolution

Nach jedem Durchgang wertet der Koordinator ausschließlich seine Übergaben und
den Gesamtzyklus aus. Nur relevante neue Erfahrung hält er nach
`../../conventions/evolution.md` gegenstandsbezogen unter `lernen/` fest.
`lernen.md` bleibt ein historisches Archiv.
