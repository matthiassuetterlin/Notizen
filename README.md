# Notizen

Notizen als Bubbles, im Look der Website (weiße Bubbles mit Haarlinie, die
wie Tropfen ineinanderfließen).

- **Doppelklick** auf die freie Fläche: neue Haupt-Bubble. Doppelklick auf eine Bubble (oder einfach lostippen, wenn sie ausgewählt ist): hineinschreiben. Enter oder Esc beendet, Shift+Enter macht eine neue Zeile.
- **Klick** wählt eine Bubble aus, **Shift-Klick** nimmt weitere dazu oder wieder heraus (dann wirken Farbe, Löschen und Ziehen auf alle). Dann: **Entf** löscht sie (ihr Inhalt rutscht eine Ebene nach oben), **Tab** legt eine Unterbubble an, die Farbpunkte färben sie ein. Bubbles ohne eigene Farbe übernehmen die Farbe der Bubble, in der sie liegen; verschiedene Farben fließen als Verlauf ineinander.
- **Ziehen** verschiebt nur. Mit Schwung losgelassen gleitet eine Bubble ein Stück weiter.
- **Shift beim Loslassen** über einer Bubble: einordnen. Gehört die gezogene Bubble schon woanders hin, gehört sie jetzt zusätzlich dazu; die beiden Bubbles rücken zusammen und verschmelzen an der Stelle, an der die gemeinsame Bubble sitzt.
- **Strg beim Loslassen** (auf dem Mac auch Cmd oder Alt): herauslösen. Die Bubble verlässt jede Bubble, aus der sie herausgezogen wurde. Wer aus der letzten herausgezogen und in der umgebenden Bubble losgelassen wird, landet dort, sonst wird sie eine eigene Haupt-Bubble.
- Auf dem Tablet ersetzen „Einordnen“ und „Herauslösen“ in der Leiste die Tasten.
- **Mittlere Maustaste** oder Ziehen auf der freien Fläche verschiebt die Ansicht, Mausrad oder zwei Finger zoomen. „Übersicht“ zeigt alles.
- **„Struktur“ oben links** zeigt die Hierarchie als Baum und listet alle Verbindungen. Klick wählt aus und holt die Bubble ins Bild, Doppelklick schreibt. Einträge lassen sich dort **ziehen**: auf einen anderen Eintrag legt sie dort hinein; mit gedrückter Shift-Taste bleibt sie, wo sie ist, und steht zusätzlich unter dem neuen Punkt (dieselbe Bubble, beide Oberpunkte verbinden sich), auf das gestrichelte Feld macht sie zur eigenen Haupt-Bubble. Die Bubbles auf der Fläche folgen sofort.
- **Sonne/Mond oben rechts** schaltet zwischen heller und dunkler Ansicht; im Menü gibt es zusätzlich „Wie System“.
- **Menü oben rechts**: oben die **Stile**. 1 Bunt (farbig, flach, klare Linie), 2 Monochrom (Grautöne, Haarlinie, Serifenschrift) und 3 Plastisch (weiche Farben, Licht und Schatten, ohne Linie) sind fest eingebaut; „+ Aktuellen Stil speichern“ legt eigene darunter an, durchnummeriert nach Position (wird einer gelöscht, rücken die folgenden nach). Der Stern macht einen Stil zum Standard beim Öffnen. Darunter aufklappbar: Farben (Farbset Pastell, Rosé, Küste, Mono; Schriftfarbe; Farbverlauf), Text (Schrift Manrope, Playfair, DM Mono; Stärke; Größe; wie stark Bubbles mit viel Inhalt größer beschriftet werden; Abstand zur Kontur), Form (u. a. Plastisch/3D), Kontur und Bewegung.
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
