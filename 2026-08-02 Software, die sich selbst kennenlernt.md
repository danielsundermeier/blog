---
beschreibung: "Wie kleine Entwicklungszyklen nicht nur Software verändern, sondern das Verständnis ihrer Aufgaben, Grenzen und Beziehungen wachsen lassen."
was_ist_gut:
  - "Der Einstieg mit dem Wunsch, ein Feature in GitHub zu strukturieren, macht die abstrakte Idee unmittelbar greifbar."
  - "Die Trennung zwischen fachlichem Anliegen und technischer Umsetzung führt schlüssig zum rekursiven Lernprozess."
  - "Das Bild des Organismus verbindet Issues, Module und Architektur, ohne die konkrete Softwareentwicklung aus dem Blick zu verlieren."
  - "Der Schluss kehrt zur ursprünglichen Issue-Struktur zurück und zeigt sie im Licht der gewonnenen Erkenntnis neu."
was_kann_ueberarbeitet_werden: []
ton:
  ziel: "Ruhig, klar, warm und entdeckend; persönlich in den Beobachtungen, ohne aus dem beschriebenen Prozess eine allgemeingültige Lehre zu machen."
  bewertung: "Der Text bleibt nah an der persönlichen Entdeckung und lädt zur gemeinsamen Erkundung ein. Möglichkeiten und Vermutungen werden als solche kenntlich gemacht; der Ton wirkt inspirierend, ohne zu drängen."
dramaturgie:
  ziel: "Von einer konkreten GitHub-Idee über die Grenzen starrer Planung zur Software als lernendem Organismus führen und am Ende die Issue-Struktur als Gedächtnis dieses Lernens neu betrachten."
  bewertung: "Die Gedankenfolge entwickelt sich nachvollziehbar von Issue und Sub-Issue über Rückkopplung und Holons bis zum lernenden Gesamtsystem. Die anfängliche GitHub-Beobachtung erhält im Schluss eine erweiterte Bedeutung."
status: veroeffentlicht
iteration: 1
---

# Software, die sich selbst kennenlernt

Vor ein paar Tagen habe ich begonnen, eine rudimentäre Struktur für ein ICM von Cardmonitor anzulegen. Kurz darauf sah ich eine zweite Einsatzmöglichkeit: Vielleicht ließe sich dieselbe Struktur auch auf unsere Arbeit in GitHub übertragen.

Ein Feature Request wäre zunächst ein fachliches Issue. Wir würden das Anliegen verstehen und grob in Schritte gliedern, ohne schon jeden Schritt technisch auszuarbeiten. Erst der Teil, den wir als Nächstes wirklich bearbeiten, würde zu einem eigenen Sub-Issue. Dort könnten wir die konkrete Umsetzung planen, einen Branch anlegen, die Änderung implementieren, testen und dokumentieren.

Selbst wenn ein Feature nur einen technischen Schritt benötigt, hätte diese Trennung einen Wert. Das übergeordnete Issue bliebe beim fachlichen Anliegen: Was soll sich für einen Menschen verbessern? Das Sub-Issue beschriebe die technische Veränderung: Was müssen wir im System tun, damit diese Verbesserung möglich wird?

Zunächst wirkte das auf mich wie eine gute Möglichkeit, Arbeit übersichtlich zu organisieren. Doch je länger ich darüber nachdachte, desto weniger ging es um Übersicht.

Es ging um Lernen.

## Der Plan ist nur der Anfang

Die naheliegende Idee wäre, ein großes Anliegen am Anfang vollständig zu zerlegen. Wir würden alle Sub-Issues anlegen und anschließend eines nach dem anderen abarbeiten.

Aber genau hier widerspricht die tatsächliche Entwicklung oft dem Plan.

Wenn wir den ersten Schritt umsetzen, lernen wir Dinge, die wir vorher noch nicht wissen konnten. Eine Abhängigkeit zeigt sich erst im Code. Eine angenommene Grenze existiert gar nicht. Zwei Module, die getrennt erschienen, erfüllen in Wirklichkeit gemeinsam eine Aufgabe. Oder wir entdecken eine einfachere Lösung, weil wir das Problem inzwischen genauer verstanden haben.

Ein vollständiger Plan würde dann schnell zu einer Beschreibung unserer früheren Annahmen.

Vielleicht genügt deshalb zunächst eine grobe Gliederung. Wir halten die Richtung fest, arbeiten aber immer nur den nächsten Schritt vollständig aus. Nach seiner Umsetzung betrachten wir das System erneut und entscheiden mit dem neu gewonnenen Wissen, was nun sinnvoll ist.

Der Plan ist damit kein Vertrag mit der Zukunft. Er ist ein vorläufiges Modell der Wirklichkeit.

Diese Haltung erinnert mich an einen Satz, der mir während des Gesprächs in den Sinn kam:

> Make the change easy. Then make the easy change.

Manchmal besteht der nächste sinnvolle Schritt noch nicht darin, das gewünschte Feature zu bauen. Zuerst müssen wir die Bedingungen schaffen, unter denen diese Änderung klar, klein und eigenständig möglich wird.

Auch dieser vorbereitende Schritt kann neue Informationen liefern. Vielleicht erkennen wir dabei, dass das ursprüngliche Problem an einer ganz anderen Stelle liegt. Die Umsetzung korrigiert unser Modell, bevor wir uns zu weit an dieses Modell gebunden haben.

## Was nach einer Änderung zurückbleibt

Ein abgeschlossener Schritt hinterlässt dann mehr als veränderten Code.

Wir haben etwas über die bearbeiteten Module gelernt:

- welche Aufgabe sie tatsächlich erfüllen,
- welche Konventionen in ihnen gelten,
- mit welchen anderen Teilen sie verbunden sind,
- wo ihre Grenzen hilfreich sind,
- und wo ihre gegenwärtige Form nicht mehr zu ihrer Aufgabe passt.

Dieses Wissen kann dazu führen, dass wir ein Modul weiter aufteilen, mit einem anderen zusammenführen oder seine Verantwortung präzisieren. Vielleicht bleibt der Code der konkreten Änderung klein, während sich unser Verständnis seiner Umgebung deutlich verändert.

Genau darin liegt für mich inzwischen der eigentliche Wert des ICM. Es dokumentiert nicht nur, wie das System gerade aufgebaut ist. Es hält fest, was wir bei seiner Bearbeitung über seine Teile und ihre Beziehungen gelernt haben.

Der nächste Zyklus beginnt dadurch nicht wieder bei null.

## Module als Holons

Ich denke bei diesen Teilen gern an Holons. Ein Holon ist ein eigenständiges Ganzes und zugleich Teil eines größeren Ganzen. Ein Modul besitzt eine eigene Aufgabe, dient aber gleichzeitig der Anwendung. Die Anwendung ist wiederum ein Ganzes für sich und Teil eines Unternehmens, einer Arbeitsweise oder eines Lebensbereichs.

Dasselbe Muster wiederholt sich auf verschiedenen Ebenen.

Wenn wir ein Modul isoliert optimieren, kann es seine eigene Aufgabe vielleicht besser erfüllen und dem Gesamtsystem trotzdem schaden. Eine besonders elegante technische Lösung kann das fachliche Anliegen unnötig kompliziert machen. Eine lokal bequeme Schnittstelle kann die Arbeit mehrerer anderer Teile erschweren.

Die Passung eines Holons zeigt sich deshalb nicht nur daran, wie gut es für sich funktioniert. Seine Form muss auch das übergeordnete Ganze unterstützen.

Ob das gelungen ist, lässt sich nicht immer im Voraus beweisen. Manchmal merken wir erst nach einer Änderung, dass das Ganze nicht mehr so gut funktioniert. Auch das ist kein wertloses Scheitern. Es ist ein Signal aus der Wirklichkeit. Wir können es aufnehmen, unser Verständnis korrigieren und es im nächsten Zyklus besser versuchen.

So entsteht Architektur nicht einmal am Anfang eines Projekts. Sie entwickelt sich durch wiederholte Begegnungen mit dem wirklichen System.

## Ein Organismus aus Beziehungen

Aus dieser Perspektive erscheint Software weniger wie eine Maschine, die nach einem fertigen Bauplan zusammengesetzt wird. Sie ähnelt eher einem Organismus, dessen Teile sich spezialisieren und gegenseitig Bedingungen schaffen.

Die Aufgabe des Ganzen besteht dann auch darin, seinen Teilen eine passende Umgebung zu geben: klare Verantwortlichkeiten, verständliche Schnittstellen, verlässliche Konventionen und genügend Freiheit, ihre eigene Aufgabe gut zu erfüllen.

Davon profitiert wiederum das Ganze.

Ein gut abgegrenztes Modul ist leichter zu verstehen und zu verändern. Eine verständliche Anwendung liefert klarere Signale aus ihrer Nutzung. Ein guter Entwicklungsprozess sorgt dafür, dass diese Signale nicht verloren gehen. Und ein wachsendes gemeinsames Gedächtnis hilft uns, aus ihnen bessere nächste Schritte abzuleiten.

Das Ganze stärkt die Teile. Die Teile stärken das Ganze.

Das bedeutet nicht, dass jede Veränderung automatisch eine Verbesserung ist. Evolution kennt keine Garantie für den richtigen nächsten Versuch. Entscheidend ist vielmehr, dass das System Rückmeldungen wahrnehmen, Erfahrungen bewahren und seine Struktur daraufhin anpassen kann.

Vielleicht bauen wir deshalb nicht nur Software.

Wir bauen einen Organismus, der lernen kann.

## GitHub als sichtbares Gedächtnis

Damit kehre ich zu der ursprünglichen Idee zurück.

Das fachliche Issue hält fest, welches Ergebnis wir erreichen möchten. Das aktuelle Sub-Issue beschreibt den nächsten in sich geschlossenen Eingriff. Der Branch und seine Commits zeigen die tatsächliche Veränderung. Tests geben Rückmeldung über ihre Wirkung. Eine fachliche Zusammenfassung übersetzt das Ergebnis zurück in die Sprache des ursprünglichen Anliegens.

Nach dem Abschluss ergänzen wir, was wir über die betroffenen Holons gelernt haben. Erst mit diesem Wissen bestimmen wir den nächsten Schritt.

GitHub wäre in diesem Modell nicht bloß eine Aufgabenliste. Es würde zu einem sichtbaren Teil des Gedächtnisses: Was wollten wir erreichen? Was haben wir angenommen? Was haben wir verändert? Was hat uns die Wirklichkeit darauf geantwortet? Und was verstehen wir jetzt besser als zuvor?

Der Code zeigt, wie die Software heute beschaffen ist.

Die verbundenen Issues, Entscheidungen und Erkenntnisse zeigen, wie sie gelernt hat, diese Form anzunehmen.

Vielleicht ist das der entscheidende Unterschied zwischen Software, die nur wächst, und Software, die reift: Mit jedem Zyklus erhält sie nicht einfach mehr Funktionen. Sie lernt ihre eigene Aufgabe, ihre Teile und deren Beziehungen ein wenig besser kennen.
