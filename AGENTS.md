# Blog

Blog ist ein eigenständiges Holon und entwickelt aus Gesprächen eigenständige Artikel.

## Arbeitsmodell

- Sichtbare Dateien und Verzeichnisse enthalten die Artikel und Entwürfe, an denen gearbeitet wird.
- `.agents/` enthält Rollen, Prozesse, Lernprotokolle und Formatkonventionen.
- `AGENTS.md` ist der Einstiegspunkt und verweist auf die zuständige Rolle.

## Routing

| Signal oder Auftrag | Zuständige Rolle |
| --- | --- |
| Ein Gespräch soll vollständig als Blogartikel verarbeitet werden | `.agents/roles/coordinator/AGENTS.md` |
| Ein konkreter Entwurf soll veröffentlicht werden | `.agents/roles/coordinator/AGENTS.md` |
| Ein ausdrücklicher Einzelauftrag an Autor, Editor oder Herausgeber | `.agents/roles/coordinator/AGENTS.md` |

Vor der Arbeit die verlinkte `AGENTS.md` vollständig lesen. Der Koordinator wählt den passenden eigenen Prozess und verweist auf die einzelnen Rollen.

## Grenzen

- Keine vorhandenen veröffentlichten Artikel überschreiben.
- Neue, ungeprüfte Artikel unter `drafts/` speichern.
- Keine Änderungen an Knowledge, X oder d15r.
- Keine X-Beiträge erstellen.
- Bestehende, nicht zur Aufgabe gehörende Änderungen bleiben unangetastet.
