# Blog

Blog ist ein eigenständiges Holon und entwickelt aus Gesprächen eigenständige Artikel.

Die kanonische Identität des medienübergreifenden Creators lebt unter
`../d15r/.agents/roles/creator/soul/AGENTS.md`. Blogrollen lesen sie als
gemeinsamen Identitätskontext, entwickeln daraus aber ihre eigenen
medienspezifischen Prozesse.

## Arbeitsmodell

- Sichtbare Dateien und Verzeichnisse enthalten die Artikel und Entwürfe, an denen gearbeitet wird.
- `.agents/` enthält Rollen, Prozesse, gegenstandsbezogene Lerndateien und
  Formatkonventionen.
- `AGENTS.md` ist der Einstiegspunkt und verweist auf die zuständige Rolle.

Jeder Agent gestaltet seinen eigenen Arbeitsbereich und entwickelt ihn nach jedem Zyklus weiter. Dafür gilt `.agents/conventions/evolution.md`.

## Routing

| Signal oder Auftrag | Zuständige Rolle |
| --- | --- |
| Ein Gespräch soll vollständig als Blogartikel verarbeitet werden | `.agents/roles/coordinator/AGENTS.md` |
| Ein konkreter Entwurf soll veröffentlicht werden | `.agents/roles/coordinator/AGENTS.md` |
| Ein ausdrücklicher Einzelauftrag an Autor, Editor oder Herausgeber | `.agents/roles/coordinator/AGENTS.md` |
| Liegengebliebene oder noch nicht abgeschlossene Blog-Arbeitsgegenstände sollen nachgeholt werden | `.agents/roles/coordinator/AGENTS.md` |

Vor der Arbeit die verlinkte `AGENTS.md` vollständig lesen. Der Koordinator wählt den passenden eigenen Prozess und verweist auf die einzelnen Rollen.

## Grenzen

- Keine vorhandenen veröffentlichten Artikel überschreiben.
- Neue, ungeprüfte Artikel unter `drafts/` speichern.
- Keine direkten Änderungen an Knowledge, X oder d15r.
- Beobachtungen über den Creator nur an dessen zuständige Rolle zurückgeben;
  die Soul nicht selbst verändern.
- Keine X-Beiträge erstellen.
- Bestehende, nicht zur Aufgabe gehörende Änderungen bleiben unangetastet.
