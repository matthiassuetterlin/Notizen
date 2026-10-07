# Notizen

Notizen als Bubbles, im Look der Website (weiße Bubbles mit Haarlinie, die
wie Tropfen ineinanderfließen).

- **Doppelklick** auf die freie Fläche: neue Haupt-Bubble. Doppelklick auf eine Bubble (oder einfach lostippen, wenn sie ausgewählt ist): hineinschreiben. Enter oder Esc beendet, Shift+Enter macht eine neue Zeile.
- **Klick** wählt eine Bubble aus. Dann: **Entf** löscht sie (ihr Inhalt rutscht eine Ebene nach oben), **Tab** legt eine Unterbubble an, die Farbpunkte färben sie ein. Bubbles ohne eigene Farbe übernehmen die Farbe der Bubble, in der sie liegen; verschiedene Farben fließen als Verlauf ineinander.
- **Ziehen** in eine andere Bubble: Die Bubble gehört jetzt dorthin (mit allem, was in ihr liegt). Auf die freie Fläche ziehen macht sie wieder zur Haupt-Bubble. Mit Schwung losgelassen gleitet sie ein Stück weiter.
- **Shift beim Loslassen** (oder „Auch zuordnen“ in der Leiste, z. B. auf dem Tablet): Die Bubble gehört zusätzlich zur Ziel-Bubble. Die beiden Bubbles rücken zusammen und verschmelzen an der Stelle, an der die gemeinsame Bubble sitzt.
- **Mittlere Maustaste** oder Ziehen auf der freien Fläche verschiebt die Ansicht, Mausrad oder zwei Finger zoomen. „Übersicht“ zeigt alles.
- **Menü oben rechts**: Anziehung, Abstoßung, Gleiten, Verschmelzen, Tropfenform, Farbverlauf, Kontur, Größen und Schrift einstellen.
- Strg/Cmd+Z macht rückgängig.

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
