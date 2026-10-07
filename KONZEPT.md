# Notizen: Zuständigkeiten als lebendige Karte

## Was ich mir angeschaut habe

- **GlassFrog und Holaspirit** (Holakratie): Kreise in Kreisen, darin Rollen mit Zweck,
  Verantwortlichkeiten und Hoheitsbereichen. Stark: Rollen statt Stellen. Schwach: die
  Kreiskarte zeigt nur die Struktur, nicht, wer wie viel trägt oder wer mit wem arbeitet.
- **Peerdom und Nestr**: dieselbe Kreislogik, dazu eine Sicht pro Person. Man sieht, in
  welchen Kreisen jemand Rollen hat, aber jede Sicht ist eine eigene Seite.
- **Kumu**: freie Netzwerkkarten mit verschiedenen „Perspektiven“ auf dieselben Daten.
  Stark für Beziehungen, kennt aber keine Organisation.
- **Team Topologies**: wenige, klare Arten, wie Teams zusammenarbeiten (Zusammenarbeit,
  Lieferung als Dienst, Befähigung). Daraus kommen die drei Beziehungsarten.
- **RACI-Matrizen**: beantworten „wer ist zuständig“, sind aber Tabellen, die niemand gern liest.

Das Muster dahinter: Alle guten Werkzeuge trennen **das Modell** (wer, was, wo) von **der
Ansicht**. Keines lässt dieselben Elemente sichtbar von einer Sicht in die andere wandern.

## Die Kernidee

**Ein Modell, drei Linsen, eine Frage.**

1. **Drei Dinge statt einer Sorte Bubble**: *Bereiche* (Teams, Abteilungen), *Rollen*
   (ein Bündel von Verantwortung mit Zweck) und *Menschen*. Eine Rolle liegt in genau einem
   Bereich, kann aber von mehreren Menschen getragen werden, und ein Mensch trägt Rollen in
   beliebig vielen Bereichen. Damit löst sich das Problem „eine Unterbubble gehört zwei
   Überbubbles“ von selbst: Es ist ein Mensch, der zwei Bereiche verbindet, oder eine Rolle,
   die zwei Menschen teilen.
2. **Drei Linsen auf dieselben Bubbles**, die beim Umschalten weich ineinander übergehen:
   - **Bereiche**: die Struktur, Rollen gepackt in ihren Bereichen, Menschen als Punkte.
   - **Menschen**: jeder Mensch eine Bubble, seine Rollen docken als farbige Tropfen an
     und verschmelzen mit ihm. Geteilte Rollen hängen zwischen zwei Menschen und verbinden
     sie. Man sieht sofort, wer viel trägt und wo eine Person zwei Bereiche verbindet.
   - **Netz**: wer liefert an wen, wer arbeitet mit wem, wer unterstützt wen. Bereiche
     sind hier keine Kreise mehr, sondern weiche Höfe um ihre Rollen.
3. **Eine Frage oben in der Mitte**: „Wer ist zuständig für …?“ Man tippt „Rechnungen“
   und bekommt die Antwort als Pfad Bereich › Rolle › Mensch, der Rest der Karte tritt zurück.
   Findet sich nichts, ist das eine Lücke.
4. **Lücken-Radar**: Rollen ohne Mensch, Aufgaben, die zwei Rollen verantworten (wer
   entscheidet?), Menschen mit vielen Rollen (Ausfallrisiko) und Menschen ohne Rolle.

## Bedienung im Prototyp

- Ziehen ordnet zu, Shift beim Loslassen teilt statt verschiebt. Ein Hinweis unten sagt
  vor dem Loslassen, was passiert.
- Doppelklick legt an: auf einen Bereich eine Rolle, auf eine Person eine Rolle für sie,
  auf die freie Fläche einen Bereich oder eine Person.
- Klick öffnet rechts die Karte des Elements: Zweck, Verantwortlichkeiten, wer sie trägt,
  Beziehungen. Alles dort ist direkt bearbeitbar.

## Was als Nächstes spannend wäre

- **Zeitachse**: Stände speichern und zwischen „vorher“ und „nachher“ einer
  Umstrukturierung hin und her blenden.
- **Vertretungen**: pro Rolle eine Vertretung, im Lücken-Radar sichtbar.
- **Hoheit** (Domains): was eine Rolle allein entscheiden darf, getrennt von dem, was sie tut.
- **Gemeinsam bearbeiten**: mehrere Leute pflegen dieselbe Karte.
- **Aus Text bauen**: eine Stellenbeschreibung oder ein Meeting-Protokoll einfügen,
  daraus Rollen und Aufgaben vorschlagen lassen.
