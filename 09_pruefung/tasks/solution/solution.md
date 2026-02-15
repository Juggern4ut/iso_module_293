# Musterlösung Aufgabenblatt 08 (Repetition)

## Teil 1: Grundlagen-Check
- `<!DOCTYPE html>` sagt dem Browser, dass die Seite als HTML5 interpretiert werden soll.
- `id` ist eindeutig pro Seite, `class` kann mehrfach verwendet werden.
- Im `head` stehen Metadaten, Titel, Verknüpfungen zu CSS/JS und technische Informationen.

## Teil 2: HTML-Struktur verbessern
Semantisch bessere Version:

```html
<header>
  <h1>Meine Seite</h1>
</header>
<nav>
  <a href="#">Home</a>
  <a href="#">Kontakt</a>
</nav>
<main>
  <p>Inhalt der Seite</p>
</main>
<footer>
  <p>Footer</p>
</footer>
```

## Teil 3: CSS und Box Model
- Box Model: content, padding, border, margin.
- Padding und Border vergrössern den insgesamt sichtbaren Platzbedarf der Box.
- Beispielklasse:

```css
.panel {
  width: 240px;
  padding: 12px;
  border: 2px solid #333;
  margin: 16px;
}
```

## Teil 4: Listen, Navigation und Links
- Navigation soll als `ul` mit `li` und `a` aufgebaut sein.
- Externer Link kann mit `target="_blank"` geöffnet werden.
- Beschreibende Texte: z. B. "Kontakt", "Kursübersicht", "Dokumentation".

## Teil 5: Positionierung
- `relative`: bleibt im Layoutfluss, kann visuell verschoben werden.
- `absolute`: aus dem Layoutfluss entfernt, positioniert relativ zum nächsten positionierten Elternteil.
- `fixed`: aus dem Layoutfluss entfernt, fix zum Browserfenster.

## Teil 6: Flexbox anwenden
- Container mit `display: flex;`.
- Abstand mit `gap`.
- Ausrichtung z. B. mit `justify-content: center; align-items: center;`.

## Teil 7: Gesamtaufgabe
- Beispielumsetzung siehe `index.html` und `styles.css` im selben Ordner.
- Enthalten: Header, Navigation, Hauptbereich mit Boxen, Footer.
- Eingesetzte Themen: semantisches HTML, Box Model, relative Positionierung, Flexbox.

## Teil 8: Reflexion (Beispiel)
- Sicheres Thema: Grundstruktur von HTML und einfache CSS-Selektoren.
- Mehr Übung nötig: Positionierung mit `absolute`.
- Nächste Lernziele:
  1. Flexbox-Achsen ohne Hilfe korrekt anwenden.
  2. Eine komplette Seite semantisch und sauber strukturiert umsetzen.
