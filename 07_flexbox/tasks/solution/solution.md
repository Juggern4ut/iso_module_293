# Musterlösung Aufgabenblatt 06 (Positionierung)

## Teil 1: Grundlagen verstehen
- `position: static;` ist die Standard-Positionierung im normalen Dokumentfluss.
- Bei `static` haben `top`, `right`, `bottom` und `left` keine Wirkung.

## Teil 2: Relative Positionierung
- Das Element wird von seiner ursprünglichen Position aus verschoben.
- Ja, der ursprüngliche Platz im Layout bleibt reserviert.
- Beispiel:

```html
<div class="container">
  <div class="box-relative">Relative Box</div>
</div>
```

```css
.container {
  border: 1px solid #ccc;
}

.box-relative {
  position: relative;
  top: 12px;
  left: 20px;
}
```

## Teil 3: Absolute Positionierung
- `relative`: bleibt im Dokumentfluss, kann visuell verschoben werden.
- `absolute`: wird aus dem Dokumentfluss genommen und relativ zum nächsten positionierten Parent platziert.
- Mit `position: relative;` auf `.container` wird `.box` relativ zu `.container` positioniert.
- Ohne `position: relative;` auf `.container` orientiert sich `.box` am Viewport (oder einem anderen positionierten Parent).

## Teil 4: Fixe Positionierung
- `position: fixed;` fixiert ein Element relativ zum Browserfenster.
- Beim Scrollen bleibt das Element an der gleichen Bildschirmposition sichtbar.
- Typische Einsatzgebiete:
  1. Fixe Navigationsleiste
  2. Cookie-Hinweis/Info- oder Hilfe-Button

## Teil 5: Z-Index verstehen
- `.box2` liegt im Vordergrund, weil `z-index: 2` größer ist als `z-index: 1`.
- `z-index` wirkt nur bei positionierten Elementen (`relative`, `absolute`, `fixed`, `sticky`), weil nur dann ein Layering-Kontext relevant ist.

## Teil 6: Fehler finden und korrigieren
- Fehler: Das Element ist nicht positioniert, daher wirken `top` und `z-index` nicht wie erwartet.
- Korrektur:

```css
.box {
  position: relative;
  top: 20px;
  z-index: 10;
}
```

## Teil 7: Praxisaufgabe
- Umsetzung siehe `index.html` und `styles.css` in diesem Ordner.
- Enthalten:
  - relativer Container
  - zwei absolut positionierte Elemente
  - fixes Element
  - überlappende Elemente mit `z-index`
