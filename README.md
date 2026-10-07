# Notizen

Notizen als Bubbles, im Look der Website (weiße Bubbles mit Haarlinie, die
wie Tropfen ineinanderfließen).

- **Doppelklick** auf die freie Fläche: neue Haupt-Bubble. Doppelklick in eine Bubble: neue Unterbubble darin.
- **Klick** auf eine Bubble: hineinschreiben. Enter oder Esc beendet, Shift+Enter macht eine neue Zeile.
- **Ziehen** in eine andere Bubble: Die Bubble gehört jetzt dorthin (mit allem, was in ihr liegt). Auf die freie Fläche ziehen macht sie wieder zur Haupt-Bubble.
- **Shift beim Loslassen** (oder „Auch zuordnen“ in der Leiste, z. B. auf dem Tablet): Die Bubble gehört zusätzlich zur Ziel-Bubble. Die beiden Bubbles rücken zusammen und verschmelzen an der Stelle, an der die gemeinsame Bubble sitzt.
- Ziehen auf die freie Fläche verschiebt die Ansicht, Mausrad oder zwei Finger zoomen. „Übersicht“ zeigt alles.
- Entf löscht die ausgewählte Bubble (ihr Inhalt rutscht eine Ebene nach oben), Strg/Cmd+Z macht rückgängig.

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
