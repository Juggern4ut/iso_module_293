---
theme: gaia
_class: lead
paginate: true
backgroundColor: #fff
backgroundImage: url('./images/hero-background.svg')
---

![bg left:40% 80%](./images/web-icon.png)

# Modul 293

## Webauftritt erstellen und veröffentlichen

---

# Inhalte dieses Modules

- Einführung in HTML - Tags/Attribute
- Einführung in CSS
- CSS Box-Modell, Inline/Block Elemente
- HTML Best practices
- Listen, Navigation
- CSS Positionierung
- CSS Flexbox
- Repetition
- Prüfung I
- Tabellen
- Formulare
- Grid I 
- CSS Animationen
- Responsive Webseiten
- Prüfung II

---

# Lernziele dieser Lektion

- Verstehen, was HTML ist und welche Rolle es in der Webentwicklung spielt.
- Kennenlernen der grundlegenden Struktur eines HTML-Dokuments.
- Verstehen von Tags und Attributen

---

# Was ist HTML?

![bg left:40% 80%](./images/html-structure.png)
- Die Hypertext Markup Language definiert das **Skelett** einer Webseite.
- HTML besteht aus vielen verschachtelten **Tags**.
- Bietet **keine** Funktionalität oder Styles.

---

# Struktur eines Tags

Tags bestehen aus den Folgenden 3 Teilen:
- Tagname
- Attribute
- Inhalte

```html
<tagname>Inhalt</tagname>
<tagname attribut="wert">Inhalt</tagname>
```

---

# Beispiel
```html
<h1>Ich bin ein Titel</h1>
<p>Das ist ein Paragraf</p>
<a href="https://google.com">Click me!</a>
```

![right:30% 80%](./images/html-result.png)

---

# HTML Struktur

Eine Webseite sollte immer mindestens die folgenden Tags beinhalten.
```html
<!DOCTYPE html> <!-- Definiert den Dokumententyp -->
<html> <!-- Äusserster Tag beinhaltet alles -->
    <head> <!-- Unsichtbar, beinhaltet Meta-Information -->
        ...
    </head>
    <body> <!-- Beinhaltet alle sichtbaren Elemente der Webseite -->
        ...
    </body>
</html>
```

---

# Meistgenutze Tags

- `h1`,`h2`,`h3`... Titel in unterschiedlichen Grössen.
- `p` Einfacher Paragraf, um Textinhalte darzustellen.
- `a` Link (Anchor), um zu anderen Seiten oder Inhalten zu verlinken.
- `img` Bild, um visuelle Inhalte einzufügen.
- `ol`, `ul` (Nummerierte) Listen, um Inhalte zu strukturieren.
- `li` Listenelement in (nummerierten) Listen.
- `div` Allgemeiner Container um Inhalte zu gruppieren.
- `main`, `section`, `article`, `aside` Bestimmte Container

---

# Verschachtelung

Der Inhalt eines Tags kann ein weiterer Tag sein. Die Tiefe der Verschachtelung ist unbegrenzt.

```html
<section>Inhalt</section>
```

```html
<section>
    <ul>
        <li>
            <a href="https://google.com">Google</a>
        </li>
    </ul>
</section>
```
