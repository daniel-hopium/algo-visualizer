# Algorithmen-Visualizer – Algorithmen zum Anfassen

Sortieren, Suchen, Datenstrukturen, Graphen und Rekursion – Schritt für Schritt animiert. Jeder Schritt zeigt die aktive Codezeile, Zähler für Vergleiche und Schreibzugriffe und eine Erklärung. Dazu echte Laufzeitmessungen, ein Sortier-Rennen und Datenstrukturen zum Selberbefüllen.

28 Einträge in 7 Kapiteln, auf Deutsch und Englisch.

Online: https://daniel-hopium.github.io/algo-visualizer/

## Starten

`index.html` im Browser öffnen, per Doppelklick. Kein Build, kein Server, keine
Abhängigkeiten. Internet braucht es nur für die Google-Schriften.

## Inhalt

| Kapitel | Einträge |
|---|---|
| Grundlagen | Die O-Notation, Theorie trifft Messung |
| Sortieren | Das Rennen, Stabil oder nicht?, Bubble Sort, Selection Sort, Insertion Sort, Shell Sort, Merge Sort, Quicksort, Heap Sort, Counting Sort |
| Suchen | Lineare Suche, Binäre Suche, Zwei Zeiger, Gleitendes Fenster |
| Datenstrukturen | Stack & Queue, Hashtabelle, Binärer Suchbaum, Binärer Heap |
| Graphen | Wegsuche im Gitter, Topologische Sortierung |
| Rekursion & DP | Der Aufrufbaum, Türme von Hanoi, Editierdistanz, Gierig oder optimal? |
| In JavaScript | sort() und seine Fallen, Was Methoden kosten |

Jeder Eintrag hat eine eigene Adresse (`#kapitel/eintrag`), die meisten eine Stolperfalle
oder einen Merksatz und Links zu MDN oder der passenden Doku. Der Überblick hat eine
durchsuchbare Tabelle aller Einträge.

## So funktioniert es

- **Rekorder:** Jeder Algorithmus läuft einmal komplett durch und speichert jeden Schritt als Bild. Darum kann man frei vor- und zurückspringen.
- **Datenformen:** Zufällig, sortiert, umgekehrt, fast sortiert, wenige Werte – damit werden beste und schlechteste Fälle sichtbar.
- **Zum Anfassen:** Hashtabelle, Suchbaum, Heap, Stack und Queue selbst befüllen; Wände und Schlamm ins Gitter zeichnen und fünf Wegsuche-Verfahren vergleichen.
- **Echt gemessen:** Sortier-Rennen mit gezählten Vergleichen und echte Kosten typischer JavaScript-Muster.

## Bedienung

- **Sprache:** Der Link oben rechts („English“ / „Deutsch“) wechselt die Sprache. Sie steht
  als `?lang=en` in der Adresse (teilbar), wird im `localStorage` gemerkt und folgt sonst der
  Browsersprache.
- `Strg+K` (Mac: `Cmd+K`) springt in die Suche der Seitenleiste.
- Hell und dunkel folgen der Systemeinstellung; der Sonne/Mond-Knopf überschreibt sie.
- Ab 1280px Breite schaltet der Breite-Knopf die breite Ansicht ein; dort lässt sich die
  Lektion am Griff rechts schmaler oder breiter ziehen.

## Aufbau

Alles steckt in einer Datei, `index.html`:

- **Hülle:** Kopfleiste, Seitenleiste mit Suche, Router, Sprache, Theme und Breite – dieselbe
  wie in den Schwester-Apps.
- **`CATS` und `ENTRIES`:** die Kapitel und ein Objekt pro Eintrag mit Text (`desc`, `tip`,
  `rule`, `links`) und einer Demo-Art (`kind`): `run` (echter Code mit Konsole), `trace`
  (Schritt-für-Schritt-Zustände), `sim` (Regler → Ergebnis) oder `custom` (eigene Demo mit
  `html()` und `init()`, die eine Aufräumfunktion zurückgibt).
- **Zweisprachig:** `tx('Deutsch','English')` steht direkt neben jedem Text.
- **Icons:** `tools/make_icons.py` erzeugt `favicon.svg`, `favicon.ico` und
  `apple-touch-icon.png` aus einer Geometrie (braucht Pillow).

## Schwester-Apps

[UI-Atlas](https://daniel-hopium.github.io/ui-atlas/), [CSS-Atlas](https://daniel-hopium.github.io/css-atlas/), [HTML-Atlas](https://daniel-hopium.github.io/html-atlas/), [ARIA-Kompass](https://daniel-hopium.github.io/aria-compass/), [Angular-Patterns](https://daniel-hopium.github.io/angular-patterns/), [Rechte-Kompass](https://daniel-hopium.github.io/access-compass/), [JS-Laufzeit](https://daniel-hopium.github.io/js-runtime/), [HTTP-Atlas](https://daniel-hopium.github.io/http-atlas/), [Sicherheits-Labor](https://daniel-hopium.github.io/security-lab/), [Performance-Atlas](https://daniel-hopium.github.io/perf-atlas/), [Regex-Werkstatt](https://daniel-hopium.github.io/regex-lab/).
