# Musterlösung Aufgabenblatt 11 (HTML-Formulare I)

## Teil 1: Grundbegriffe verstehen
- `form` fasst alle Eingabefelder und Buttons eines Formulars zusammen.
- `action` gibt grob an, wohin die Formulardaten gesendet werden.
- `method` legt grob fest, wie die Daten gesendet werden, zum Beispiel mit `get` oder `post`.
- Ein Button mit `type="submit"` sendet das Formular ab.

## Teil 2: Formular-Grundstruktur schreiben

```html
<form action="/anfrage" method="post">
  <button type="submit">Senden</button>
</form>
```

## Teil 3: Eingabefelder ergänzen

```html
<form action="/anfrage" method="post">
  <input type="text" name="vorname" />
  <input type="text" name="nachname" />
  <input type="number" name="alter" />
  <button type="submit">Senden</button>
</form>
```

## Teil 4: Code lesen
- Der Benutzer kann eine Stadt und eine Postleitzahl eingeben.
- Beim Klick auf den Button wird das Formular abgesendet.
- `action="/send"` bestimmt das Ziel, `method="get"` die grobe Art der Übertragung.

## Teil 5: Fehler korrigieren

```html
<form action="/registrieren" method="post">
  <input type="text" name="vorname" />
  <input type="number" name="alter" />
  <button type="submit">Absenden</button>
</form>
```

Gefundene Fehler:
1. Beim ersten `input` fehlte das schliessende `>`.
2. `input` ist ein leeres Element und braucht kein schliessendes `</input>`.
3. Der Button war nicht korrekt geschlossen.

## Teil 6: Praxisaufgabe
- Umsetzung siehe `index.html` und `styles.css`.
- Enthalten sind ein Formular mit `action`, `method`, zwei Textfeldern, einem Zahlenfeld und Submit-Button.

## Teil 7: Reflexion (Beispielantwort)
- Das Formular ist der Rahmen, die Eingabefelder sind die einzelnen Eingabeelemente darin.
- Der Submit-Button startet das Absenden der Daten.
- Noch unklar könnte sein, wann man `get` und wann man `post` verwendet.
