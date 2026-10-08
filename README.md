# Verantwortungsplaner

Zuständigkeiten einer Firma als lebendige Bubble-Karte: **Bereiche**, **Rollen** und **Menschen**,
gezeigt in drei Linsen, die weich ineinander übergehen. Gedanken und Recherche dazu stehen in
[`KONZEPT.md`](KONZEPT.md).

- **Bereiche**: Rollen in ihren Bereichen, Menschen als Punkte. Rolle in einen anderen Bereich ziehen verschiebt sie, einen Personen-Punkt auf eine andere Rolle ziehen überträgt die Aufgabe (Shift: teilen, auf die freie Fläche: abgeben).
- **Menschen**: jede Person eine Bubble, ihre Rollen docken an und verschmelzen mit ihr. Rolle auf eine Person ziehen überträgt sie, mit Shift wird sie geteilt.
- **Netz**: wer liefert an wen, wer arbeitet mit wem, wer unterstützt wen.
- **Verbinden** (in jeder Linse): Fährt man über eine Rolle, poppen am Rand vier Andockpunkte auf. Aus einem zieht man live ein Kabel zu einer anderen Rolle; beim Loslassen entsteht die Verbindung und ein kleines Menü fragt nach der Art (liefert an, arbeitet mit, unterstützt), Richtung umkehren oder löschen. Ein Klick auf eine Linie öffnet dasselbe Menü.
- **„Wer ist zuständig für …?“** oben sucht in Rollen, Aufgaben und Namen und zeigt Bereich › Rolle › Person.
- **Frei anordnen**: In „Bereiche“ zieht man einen ganzen Bereich an seiner Fläche oder am Titel, Beim ersten Aufbau wird nichts überlappend angeordnet; legt man einen Bereich bewusst an oder in einen anderen, dockt er an und verschmilzt, Wegziehen löst ihn wieder. Im „Netz“ einen Bereich an seinem Hof oder Titel. Die Anordnung bleibt gespeichert; „Anordnung dieser Ansicht zurücksetzen“ im Menü ordnet neu. Die Titel der Bereiche stehen gerade über der Form.
- **Fähnchen** halten offene Punkte fest, die noch geklärt werden müssen: Rolle, Person oder Bereich anklicken, im Panel „Fähnchen setzen“ und Notiz tippen. Das Fähnchen steckt dann am Rand der Bubble (Maus drüber zeigt den Text), der Kreis davor hakt es als geklärt ab. Der Knopf „Fähnchen“ oben listet alle offenen und geklärten.
- **Lücken** zeigt Rollen ohne Person, doppelt verantwortete Aufgaben und Menschen mit vielen Rollen.
- **Doppelklick** legt an, **Klick** öffnet rechts die Karte zum Bearbeiten, **Entf** löscht, **Strg/Cmd+Z** macht rückgängig, **1 2 3** wechselt die Linse, **/** sucht.
- **Mausrad** zoomt überall, auch über den Bubbles; Ziehen auf der freien Fläche oder die **mittlere Maustaste** verschiebt die Ansicht. Unten links: Rückgängig, Wiederholen und Zoom (Klick auf die Prozentzahl zeigt alles).
- **Gespeichert** (ganz oben im Menü ☰): „+ Aktuelle Einstellungen speichern“ legt einen neuen Eintrag an, benannt nach Datum und Uhrzeit (z. B. „07.10.2026 | 21.59“). Jeder Eintrag behält seinen Namen, auch beim Verschieben oder Löschen anderer. Ein Klick lädt den Eintrag, ein zweiter Klick darauf (oder Doppelklick, oder Stift ✎) benennt ihn um; Enter übernimmt, Esc bricht ab. Einträge lassen sich an der Zeile (oder am Griff ⋮⋮) nach oben und unten ziehen. Der Haken markiert den Default, der Knopf „Default“ lädt ihn. Neue Besucher bekommen acht eingebaute Einträge: Dark & Fruity (Default, damit startet die Seite), Glowing Dark, Fruity Heaven, CI Contours, Fruity 3D Heaven, Buttons, Minesweeper, Night Golfing. „↗ Alle exportieren“ kopiert alle Einträge als JSON in die Zwischenablage.
- **Bearbeiten-Fenster** rechts: an der linken Kante breiter ziehbar, − / + oder Strg/Cmd+Mausrad zoomen den Inhalt; ist das Menü ☰ offen, steht es links daneben.
- **Menü ☰ oben rechts** (bleibt offen, bis man es mit × oder ☰ schließt; an der linken Kante breiter ziehbar; − / + oben oder Strg/Cmd+Mausrad zoomen den Inhalt): hell, dunkel oder wie System; Farbset (Frisch, Pastell, Abend, Mono), Farbverlauf, Farbstärke, Deckkraft, Verschmelzen, Abstand der Rollen, Plastisch, Kontur mit Konturfarbe (Automatisch: hell schwarz, dunkel weiß, oder eine der VAVE-CI-Farben), Konturstärke und Konturschärfe, Schrift, „Schrift in der Bubble halten“ (verkleinert und bricht lange Namen um, Rollen mit langem Namen wachsen etwas mit; 0 % schaltet das ab), Punkte im Hintergrund. Dazu Datei sichern und laden.

Alles wird automatisch im Browser gespeichert (localStorage, pro Gerät und Browser).

## Frühere Versionen

- [`bubbles.html`](bubbles.html): die freien Bubble-Notizen (Andocken, Verschmelzen, Verbinden).
- [`hierarchie.html`](hierarchie.html): die Version mit Mehrfach-Zuordnung.

### Bedienung von bubbles.html

- **Doppelklick** auf die freie Fläche: neue Haupt-Bubble. Doppelklick auf eine Bubble (oder einfach lostippen, wenn sie ausgewählt ist): hineinschreiben. Enter beginnt einen neuen Absatz; Esc, Strg/Cmd+Enter oder ein Klick daneben beendet.
- **Klick** wählt eine Bubble aus, **Shift-Klick** nimmt weitere dazu oder wieder heraus (dann wirken Farbe, Löschen und Ziehen auf alle). Dann: **Entf** löscht sie (ihr Inhalt rutscht eine Ebene nach oben), **Tab** legt eine Unterbubble an, die Farbpunkte färben sie ein. Bubbles ohne eigene Farbe übernehmen die Farbe der Bubble, in der sie liegen; verschiedene Farben fließen als Verlauf ineinander.
- **Ziehen** verschiebt. Berührt die Bubble beim Loslassen eine andere, docken beide an und bleiben verschmolzen; zieht man eine angedockte Bubble weg und lässt sie frei los, löst sie sich. „Gruppe“ in der Leiste wählt alles, was an der gewählten Bubble hängt, um es gemeinsam zu verschieben.
- **In eine Bubble hineinziehen** legt die Bubble dort hinein (auch eine Unterbubble in eine andere Bubble) und dockt sie an, was sie dort berührt. **Herausziehen** holt sie heraus: in die umgebende Bubble oder als eigene Haupt-Bubble aufs Brett. Ein Hinweis unten sagt vor dem Loslassen, was passiert. Eine Bubble liegt immer in höchstens einer anderen. Hatte sie keine eigene Farbe, behält sie beim Umziehen die Farbe der Bubble, aus der sie kommt.
- **Verbinden**: zwei Bubbles mit Shift-Klick wählen und „Verbinden“ drücken. Das geht auch, wenn sie in verschiedenen Bubbles liegen: Beide bleiben, wo sie sind, und behalten ihre Farbe, ein Hals mit Farbverlauf verbindet sie. Dieselbe Taste heißt dann „Trennen“. Breite und Zug zueinander stehen im Menü unter **Verbindungen**.
- **Mittlere Maustaste** oder Ziehen auf der freien Fläche verschiebt die Ansicht, Mausrad oder zwei Finger zoomen. „Übersicht“ zeigt alles.
- **„Struktur“ oben links** zeigt, was worin liegt, und listet die angedockten Gruppen. Klick wählt aus und holt die Bubble ins Bild, Doppelklick schreibt. Einträge lassen sich dort **ziehen**: auf einen anderen Eintrag legt sie dort hinein, mit gedrückter Shift-Taste dockt sie neben ihm an; auf das gestrichelte Feld macht sie zur eigenen Haupt-Bubble. Die Bubbles auf der Fläche folgen sofort.
- **Sonne/Mond oben rechts** schaltet zwischen heller und dunkler Ansicht; im Menü gibt es zusätzlich „Wie System“.
- **Menü oben rechts**: Ansicht (hell, dunkel, wie System) und **Gespeichert**: „+ Einstellungen speichern“ legt die aktuellen Einstellungen als 1, 2, 3 … ab, der Stern lädt sie beim Öffnen. Darunter: **Farben** (Farbset Pastell, Küste, Mono, CI (die CI-Farben; wählbar, Standard bleibt Pastell); Reichweite des Farbverlaufs, wie weit die Farbe einer Bubble in die angrenzenden hineinläuft; Farbstärke; Deckkraft der Füllung; Schriftfarbe als Farbregler, „Automatisch“ passt sie an hell/dunkel an), **Schrift** (Manrope, Playfair, Space Grotesk; Stärke; Schriftgröße; größer, je mehr darin liegt), **Form** (Runde Bubbles an/aus; Rundung der freien Form; Verschmelzen; Kontur an/aus; Konturstärke; Konturfarbe; Plastisch; Größe leerer Bubbles; Rand innen) und **Bewegung** (Abstand zwischen Bubbles; Anziehung zur Mitte; Abstoßung; Gleiten) **Verbindungen** (ohne Auswahl keine Linien; ein Klick auf eine Rolle zeigt ihre, auf eine Person die aller ihrer Rollen, auf einen Bereich die aller Rollen darin; der Schalter „Alle Verbindungen“ oben (standardmäßig an) blendet alle ein; Als Flugrouten über allem an/aus: Bögen von Bubble zu Bubble über Farbe und Schrift, mit weichem Schatten; Regler Flughöhe) und **Hintergrund** (Punkte an/aus).
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

## Daten mit Passwort freigeben

Die Daten (Bereiche, Rollen, Menschen, Verbindungen) liegen im Browser. Damit andere sie sehen, ohne dass sie offen im Netz stehen: ☰ → „Für alle verschlüsseln …“, Passwort zweimal eingeben (mindestens 12 Zeichen, am besten ein Satz aus 4+ Wörtern), den erzeugten Text an Claude schicken. Er wird als `VAULT` in `index.html` eingebaut (PBKDF2-SHA-256 mit 600 000 Runden, AES-GCM 256). Besucher sehen beim Öffnen ein Passwortfeld; das richtige Passwort lädt die Daten, „Abbrechen“ zeigt die Beispieldaten. Vorhandene eigene Daten im Browser werden vorher unter `notizen.backup` gesichert. Über ☰ → „Freigegebene Daten laden (Passwort) …“ lässt sich die Abfrage jederzeit wieder öffnen.
