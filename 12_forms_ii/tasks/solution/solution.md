# Musterlösung Aufgabenblatt 12 (HTML-Formulare II)

## Teil 1: Elemente zuordnen
- Genau eine Option aus mehreren: Radio-Buttons
- Mehrere unabhängige Optionen: Checkboxen
- Auswahl aus einer Liste: `select` mit `option`
- Längerer Freitext: `textarea`

## Teil 2: Dropdown bauen

```html
<select name="kurs">
  <option>HTML</option>
  <option>CSS</option>
  <option>Flexbox</option>
  <option>Formulare</option>
</select>
```

## Teil 3: Radios und Checkboxen
- Radio-Buttons eignen sich für genau eine Auswahl in einer Gruppe.
- Checkboxen eignen sich für mehrere gleichzeitige Auswahlen.

```html
<input type="radio" name="niveau" value="anfaenger" />
<input type="radio" name="niveau" value="mittel" />
<input type="radio" name="niveau" value="fortgeschritten" />

<input type="checkbox" name="extras" value="kaffee" />
<input type="checkbox" name="extras" value="handout" />
```

## Teil 4: Textarea ergänzen

```html
<textarea name="bemerkungen" rows="5"></textarea>
```

- `textarea` ist für längere mehrzeilige Texte gedacht.
- Ein normales Textfeld mit `type="text"` ist für kurze einzeilige Eingaben gedacht.

## Teil 5: Code lesen
- Möglich sind eine Auswahl im Dropdown, genau eine Tempo-Auswahl, eine Checkbox-Auswahl und ein Kommentar.
- Die Radio-Buttons haben denselben `name`, damit sie als Gruppe funktionieren.
- Checkboxen können mehrfach gewählt werden.

## Teil 6: Praxisaufgabe
- Umsetzung siehe `index.html` und `styles.css`.
- Enthalten sind Dropdown, Radio-Buttons, Checkboxen, `textarea` und Submit-Button.

## Teil 7: Reflexion (Beispielantwort)
- Ein Dropdown ist sinnvoll, wenn viele Optionen wenig Platz brauchen sollen.
- Checkboxen sind sinnvoll, wenn mehrere Optionen gleichzeitig gewählt werden dürfen.
- Unsicherheit kann es bei der Gruppierung von Radio-Buttons mit `name` geben.
