# Musterlösung Aufgabenblatt 10 (HTML-Tabellen)

## Teil 1: Grundelemente verstehen
- `table` definiert den gesamten Tabellenbereich.
- `th` ist eine Kopfzelle (meist Titel/Bezeichnung), `td` ist eine normale Datenzelle.
- `tr` steht für eine Tabellenzeile und enthält `th`/`td`.

## Teil 2: Tabelle aufbauen
- Beispielstruktur:

```html
<table>
  <tr>
    <th>Name</th>
    <th>Fach</th>
    <th>Note</th>
  </tr>
  <tr>
    <td>Lea</td>
    <td>HTML</td>
    <td>5.0</td>
  </tr>
</table>
```

## Teil 3: Struktur verbessern
- `caption` beschreibt den Inhalt der Tabelle.
- `thead` enthält Kopfzeilen.
- `tbody` enthält die eigentlichen Datensätze.
- Vorteil: klarere Struktur, besser lesbar, einfacher wartbar.

## Teil 4: Zellen zusammenfassen
- `colspan="3"` verbindet drei Spalten in einer Zeile.
- `rowspan="2"` verbindet zwei Zeilen in einer Spalte.
- Dadurch können zusätzliche Infos oder Gruppierungen übersichtlich dargestellt werden.

## Teil 5: Fehler finden und korrigieren
Korrigierte Version:

```html
<table>
  <thead>
    <tr>
      <th>Produkt</th>
      <th>Preis</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Tastatur</td>
      <td>49.-</td>
    </tr>
  </tbody>
</table>
```

Gefundene Fehler:
1. In `thead` fehlte die Zeile `tr`.
2. `td` bei `Tastatur` war nicht geschlossen.
3. Struktur in `thead`/`tbody` war dadurch nicht valide.

## Teil 6: Praxisaufgabe
- Umsetzung siehe `index.html` und `styles.css` im gleichen Ordner.
- Enthalten sind:
  - `caption`, `thead`, `tbody`
  - mindestens fünf Datenzeilen
  - eine zusammengefasste Zelle mit `colspan`

## Teil 7: Reflexion (Beispielantwort)
- Einfach war die Grundstruktur aus `table`, `tr`, `th`, `td`.
- Unsicherheit gab es bei `colspan` und `rowspan`.
- Eine Tabelle ist korrekt strukturiert, wenn Zeilen sauber aufgebaut sind und Kopf-/Datenbereich sinnvoll getrennt sind.
