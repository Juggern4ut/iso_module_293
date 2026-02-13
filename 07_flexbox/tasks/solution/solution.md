# Musterlösung Aufgabenblatt 07 (Flexbox)

## Teil 1: Grundlagen verstehen
- Unterschied Block/Flex: Beim Block-Layout stehen Elemente standardmässig untereinander. Bei Flexbox werden direkte Kinder flexibel in einer Zeile oder Spalte angeordnet.
- Flex-Items: Alle direkten Kind-Elemente des Flex-Containers.
- Aktivierung: `display: flex;`

## Teil 2: Achsen verstehen
- Bei `flex-direction: row;` verläuft die Hauptachse horizontal.
- Die Querachse verläuft vertikal.
- Bei `column` ist es umgekehrt: Hauptachse vertikal, Querachse horizontal.

## Teil 3: Ausrichtung im Container
- `justify-content: center;` zentriert die Items auf der Hauptachse.
- `justify-content: space-between;` verteilt die Items mit maximalem Abstand dazwischen.
- `align-items: center;` zentriert Items auf der Querachse.

## Teil 4: Umbruch und Abstände
- Mit `flex-wrap: wrap;` springen Items in die nächste Zeile, wenn kein Platz mehr vorhanden ist.
- Vorteil von `gap`: gleichmässige Abstände ohne Extra-Logik für erstes/letztes Element.

## Teil 5: Eigenschaften von Flex-Items
- Bei `1 : 2 : 1` erhält `item-b` am meisten Platz.
- Bei allen `flex: 1;` teilen sich alle Items den Platz gleichmässig.

## Teil 6: Fehler finden und korrigieren
- `justify-content` und `align-items` wirken nur auf Flex-Container, nicht auf normale Items.
- Korrektur:

```css
.container {
  display: flex;
  justify-content: center;
  align-items: center;
}
```

## Teil 7: Praxisaufgabe
- Umsetzung siehe `index.html` und `styles.css` in diesem Ordner.
- Enthalten: Navbar (Logo + 3 Links), Kartenbereich mit 4 Karten, Footer.
- Alle drei Bereiche nutzen Flexbox.

## Teil 8: Reflexion (Beispiel)
- Hilfreichste Eigenschaft: `justify-content`, weil damit Layouts schnell geordnet werden können.
- Schwierigkeit: Unterschied zwischen Hauptachse und Querachse bei wechselnder `flex-direction`.
- Realer Einsatz: Navigation, Kartenraster, Buttons in Toolbars, Dashboard-Layouts.
