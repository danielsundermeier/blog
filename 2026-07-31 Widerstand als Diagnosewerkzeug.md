---
beschreibung: "Wie der Widerstand gegen eine technische Lösung sichtbar machte, dass nicht die Hindernisse, sondern unsere Grundannahme das eigentliche Problem war."
was_ist_gut:
  - "Der Einstieg macht die abstrakte Idee des Widerstands an einer konkreten, nachvollziehbaren API-Situation sichtbar. Produktzahl, sequentielle Abfragen, Rate Limit und fehlende Berechtigung zeigen gemeinsam, warum nicht nur ein einzelnes Hindernis vorlag."
  - "Die Erkenntnis entsteht schrittweise aus den immer komplizierteren Workarounds und der erst spät geprüften Grundannahme. Der Text verkündet die Heuristik nicht vorab, sondern lässt sie aus dem Unterschied zwischen den beiden Lösungswegen hervorgehen."
  - "Die Unterscheidung zwischen lokaler Schwierigkeit und systemischem Widerstand verhindert eine pauschale Gleichsetzung von Anstrengung und falschem Weg. Der steile Berg, die möglichen fehlenden Informationen und der unvermeidbar schwierige Abschnitt halten die Aussage offen und glaubwürdig."
  - "Die Fragen an die eigene Vorstellung übertragen das technische Beispiel behutsam auf andere Vorhaben, ohne eine endgültige Entscheidungsregel zu behaupten. Der Ton bleibt dadurch persönlich, suchend und einladend."
  - "Der Schluss kehrt zur Preisabfrage und zum Puzzleteil zurück. Dass das neue Teil vermutlich besser, aber nicht endgültig richtig ist, schließt den dramaturgischen Kreis und bewahrt zugleich die Unsicherheit des Gesprächs."
was_kann_ueberarbeitet_werden: []
ton:
  ziel: "Ruhig, persönlich und suchend; der Text soll dazu einladen, Widerstand als Rückmeldung zu lesen, ohne Anstrengung pauschal zum Zeichen eines falschen Weges zu erklären."
  bewertung: "Das Ziel wird erreicht. Der Text bleibt ruhig, klar und persönlich und lädt mit Fragen wie „Welchen Teil meiner Vorstellung verteidige ich gerade?“ zur eigenen Prüfung ein. Einschränkungen wie „vielleicht“, „nicht unbedingt“ und die ausdrückliche Anerkennung unvermeidbarer Schwierigkeiten verhindern, dass die Beobachtung belehrend oder zur allgemeingültigen Wahrheit wird."
dramaturgie:
  ziel: "Von dem Versuch, Preise über hunderttausende einzelne API-Abfragen zu ermitteln, über immer absurdere Umgehungslösungen zur Überprüfung der Grundannahme führen und am Ende zum Bild des nicht passenden Puzzleteils zurückkehren."
  bewertung: "Die Dramaturgie folgt lückenlos der beabsichtigten Bewegung: konkrete API-Grenzen, abstruser werdende Workarounds, Prüfung der Grundannahme, Vergleich der beiden Wege und vorsichtige Verallgemeinerung zur diagnostischen Heuristik. Der Übergang vom technischen Beispiel zum persönlichen Sumpfgefühl ist vorbereitet, und der Schluss betrachtet die anfängliche Preisabfrage durch das Bild des passenden Puzzleteils neu."
status: veroeffentlicht
iteration: 1
---

# Widerstand als Diagnosewerkzeug

Wir wollten die Preise unserer Produkte ermitteln, indem wir sämtliche Angebote eines Marktplatzes abrufen.

Die Idee klang zunächst naheliegend. Wenn wir alle Angebote kennen, kennen wir schließlich auch den Marktpreis. Also begannen wir, die dafür nötige Technik zu planen.

Dann antwortete die Realität.

Der Marktplatz stellte die Angebote nur für einzelne Produkte bereit. Davon gab es mehr als 350.000. Wir konnten immer nur eine Abfrage zur selben Zeit ausführen. Selbst ein vollständiger Tag hätte nicht gereicht, um jedes Produkt einmal abzurufen. Dazu kamen ein Rate Limit und ein API-Zugang, mit dem diese Art der Nutzung gar nicht erlaubt war.

Fast alles sprach gegen unseren Weg.

Doch statt den Weg zu überprüfen, versuchten wir, die Hindernisse zu überwinden.

Für jede Grenze suchten wir einen neuen Workaround. Wie könnten wir mehr Abfragen unterbringen? Wie könnten wir den Prozess anders verteilen? Wie ließe sich die fehlende Zeit doch noch ausgleichen? Jede Antwort machte unsere Lösung komplizierter, ohne das eigentliche Problem zu beseitigen.

Unsere Ideen wurden immer abstruser.

Das hätte uns etwas sagen können. Wir lasen den Widerstand jedoch zunächst nur als technische Aufgabe. Wir glaubten, wir müssten cleverer, ausdauernder oder kreativer werden. Die Grundannahme blieb unangetastet:

> Um Preise zu bekommen, müssen wir alle einzelnen Angebote abrufen.

Solange diese Annahme feststand, konnte jede neue Schwierigkeit nur ein Hindernis sein. Wir hatten den Weg bereits gewählt. Also musste die Realität sich irgendwie dazu bringen lassen, ihn freizugeben.

Irgendwann gingen wir einen Schritt zurück.

Nicht zur letzten technischen Entscheidung, sondern zur Frage davor: Müssen wir die Preise wirklich auf diese Weise ermitteln?

Als wir diese Annahme losließen, fanden wir einen anderen Weg. Plötzlich schien vieles einfacher zu werden. Grenzen, die uns vorher ständig beschäftigten, spielten keine Rolle mehr. Die einzelnen Teile begannen wieder zusammenzupassen.

Der Unterschied lag nicht darin, dass die zweite Lösung vollkommen mühelos war. Auch ein passender Weg verlangt Arbeit. Der Unterschied war, dass die Schwierigkeiten ihren Charakter verändert hatten.

Auf dem ersten Weg tauchte derselbe Widerspruch überall auf. Die Zahl der Produkte war zu groß, die verfügbare Zeit zu kurz, die Schnittstelle zu langsam und die Berechtigung unpassend. Kein einzelner Fehler blockierte uns. Das gesamte Umfeld widersprach der Art, wie wir das Problem lösen wollten.

Auf dem neuen Weg gab es weiterhin Aufgaben. Doch sie ließen sich nacheinander bearbeiten. Eine gelöste Frage machte die nächste klarer, statt zwei neue Umgehungskonstruktionen hervorzubringen.

Vielleicht ist das eine hilfreiche Unterscheidung.

Nicht jede Anstrengung bedeutet, dass wir falsch liegen. Etwas Neues zu lernen kann schwer sein. Ein anspruchsvolles Projekt kann Geduld verlangen. Ein steiler Abschnitt ist noch kein Grund, den Berg zu verlassen.

Wenn Schwierigkeiten jedoch an vielen unabhängigen Stellen dieselbe Grundidee infrage stellen, lohnt sich eine andere Reaktion. Dann sollten wir vielleicht nicht sofort fragen, wie wir den nächsten Widerstand brechen. Wir könnten fragen, worauf er zeigt.

Ein einzelnes Problem lädt dazu ein, es zu lösen.

Probleme überall laden dazu ein, das Modell zu überprüfen.

Damit wird Widerstand vom Gegner zum Diagnosewerkzeug. Er sagt nicht unbedingt, dass wir aufgeben sollen. Er macht sichtbar, welche Annahme gerade mit der Realität kollidiert.

Das ist schwer zu erkennen, wenn wir bereits viel in eine Lösung investiert haben. Je länger wir an ihr arbeiten, desto leichter halten wir Beharrlichkeit für die einzige vernünftige Antwort. Jeder Workaround beweist dann, wie entschlossen wir sind. Gleichzeitig bindet er uns noch stärker an den Weg, den er retten soll.

Vielleicht liegt die eigentliche Ausdauer manchmal darin, einen Schritt zurückzugehen.

Nicht beim ersten Hindernis. Nicht aus Bequemlichkeit. Sondern dann, wenn wir bemerken, dass unsere Arbeit fast nur noch daraus besteht, die Folgen einer ungeprüften Annahme zu verwalten.

Ich kenne dieses Gefühl auch außerhalb technischer Probleme. Ein Vorhaben wird zäh. Jeder Schritt scheint neue Reibung zu erzeugen. Ich arbeite mehr, doch komme der Wurzel nicht näher. Es fühlt sich an, als würde ich durch einen Sumpf waten.

Früher hätte ich darin vor allem eine Aufforderung gesehen, mich noch stärker anzustrengen. Heute versuche ich, das Gefühl zunächst als Frage zu lesen:

> Welchen Teil meiner Vorstellung verteidige ich gerade gegen die Rückmeldung der Realität?

Die Antwort muss nicht sein, alles zu verwerfen. Vielleicht fehlt nur eine Information. Vielleicht ist der Weg richtig und der schwierige Abschnitt unvermeidbar. Aber manchmal entdecken wir eine Annahme, die so selbstverständlich wirkte, dass wir sie nie geprüft haben.

Dann verändert ein Schritt zurück mehr als zehn Schritte nach vorn.

Bei unserer Preisabfrage hatten wir lange versucht, ein Puzzleteil an eine Stelle zu drücken, an die es nicht gehörte. Weil es fast passte, glaubten wir, wir müssten nur mehr Kraft aufwenden. Doch jeder zusätzliche Druck verformte das Bild.

Erst als wir aufhörten zu drücken, konnten wir wieder auf das ganze Puzzle schauen.

Nun haben wir vermutlich ein besseres Teil gefunden. Wir wissen noch nicht, ob es das endgültig richtige ist. Aber wir erkennen einen Unterschied: Es muss nicht von immer neuen Konstruktionen an seinem Platz gehalten werden.

Es fällt beinahe von selbst hinein.
