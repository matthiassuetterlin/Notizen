# Notizen

Notizen als Bubbles auf einem freien Brett, im Look der Website: Bubbles, die man
aneinanderschiebt, verschmelzen wie Tropfen und bleiben so angedockt; jede behält ihre Farbe.

Die frühere Version mit Mehrfach-Zuordnung (eine Bubble in mehreren Bubbles) liegt als
`hierarchie.html` im Repository und lässt sich dort weiter öffnen.

- **Doppelklick** auf die freie Fläche: neue Haupt-Bubble. Doppelklick auf eine Bubble (oder einfach lostippen, wenn sie ausgewählt ist): hineinschreiben. Enter beginnt einen neuen Absatz; Esc, Strg/Cmd+Enter oder ein Klick daneben beendet.
- **Klick** wählt eine Bubble aus, **Shift-Klick** nimmt weitere dazu oder wieder heraus (dann wirken Farbe, Löschen und Ziehen auf alle). Dann: **Entf** löscht sie (ihr Inhalt rutscht eine Ebene nach oben), **Tab** legt eine Unterbubble an, die Farbpunkte färben sie ein. Bubbles ohne eigene Farbe übernehmen die Farbe der Bubble, in der sie liegen; verschiedene Farben fließen als Verlauf ineinander.
- **Ziehen** verschiebt. Berührt die Bubble beim Loslassen eine andere, docken beide an und bleiben verschmolzen; zieht man eine angedockte Bubble weg und lässt sie frei los, löst sie sich. „Gruppe“ in der Leiste wählt alles, was an der gewählten Bubble hängt, um es gemeinsam zu verschieben.
- **In eine Bubble hineinziehen** legt die Bubble dort hinein (auch eine Unterbubble in eine andere Bubble) und dockt sie an, was sie dort berührt. **Herausziehen** holt sie heraus: in die umgebende Bubble oder als eigene Haupt-Bubble aufs Brett. Ein Hinweis unten sagt vor dem Loslassen, was passiert. Eine Bubble liegt immer in höchstens einer anderen. Hatte sie keine eigene Farbe, behält sie beim Umziehen die Farbe der Bubble, aus der sie kommt.
- **Mittlere Maustaste** oder Ziehen auf der freien Fläche verschiebt die Ansicht, Mausrad oder zwei Finger zoomen. „Übersicht“ zeigt alles.
- **„Struktur“ oben links** zeigt, was worin liegt, und listet die angedockten Gruppen. Klick wählt aus und holt die Bubble ins Bild, Doppelklick schreibt. Einträge lassen sich dort **ziehen**: auf einen anderen Eintrag legt sie dort hinein, mit gedrückter Shift-Taste dockt sie neben ihm an; auf das gestrichelte Feld macht sie zur eigenen Haupt-Bubble. Die Bubbles auf der Fläche folgen sofort.
- **Sonne/Mond oben rechts** schaltet zwischen heller und dunkler Ansicht; im Menü gibt es zusätzlich „Wie System“.
- **Menü oben rechts**: Ansicht (hell, dunkel, wie System) und **Gespeichert**: „+ Einstellungen speichern“ legt die aktuellen Einstellungen als 1, 2, 3 … ab, der Stern lädt sie beim Öffnen. Darunter: **Farben** (Farbset Pastell, Küste, Mono; Farbverlauf, wie weit die Farbe einer Bubble in die angrenzenden hineinläuft; Farbstärke; Deckkraft; Schriftfarbe als Farbregler, „Automatisch“ passt sie an hell/dunkel an), **Schrift** (Manrope, Playfair, DM Mono; Stärke; Schriftgröße; größer, je mehr darin liegt), **Form** (Runde Bubbles an/aus; Rundung der freien Form; Verschmelzen; Kontur an/aus; Konturstärke; Konturfarbe; Plastisch; Größe leerer Bubbles; Rand innen) und **Bewegung** (Abstand zwischen Bubbles; Anziehung zur Mitte; Abstoßung; Gleiten) und **Hintergrund** (Punkte an/aus).
- **Runde Bubbles aus**: Bubbles mit Inhalt bleiben nicht rund, sondern legen sich als freie Form um ihre Unterbubbles, die Beschriftung sitzt oben. „Rundung der freien Form“ regelt stufenlos zwischen eng anliegend und fast rund. Leere Bubbles bleiben rund.
- Strg/Cmd+A wählt alle Bubbles aus.
- Strg/Cmd+Z macht rückgängig, Strg/Cmd+Shift+Z oder Strg+Y wiederholt (auch als Buttons in der Leiste).

Alles wird automatisch im Browser gespeichert (localStorage, pro Gerät und Browser).
„Export“ lädt eine JSON-Datei herunter, „Import“ liest sie wieder ein.

## Öffnen

`index.html` im Browser öffnen, oder:

```bash
python3 -m http.server 8000
```

## Veröffentlichung

Jeder Push auf `main` veröffentlicht die Seite über GitHub Pages
(Workflow `.github/workflows/pages.yml`, Quelle in den Pages-Einstellungen: „GitHub Actions“).
