# Hands-on øvelse - bygge en webside

## Innhold
[Steg 1](./step-1/README.md)

## VS Code

Ikke strengt nødvendig, men det hjelper en del

Gå til https://code.visualstudio.com/download og last ned

Følg instruksjonene for å installere

## Mappestruktur

1. Lag en ny mappe (hvor som helst)
2. Kall den noe fint (f.eks webside)
3. Åpne mappen fra VS Code
4. Legg til en ny fil, kall den index.html

## Index.html

Kopier og lim inn følgende HTML i index.html

```html
<html>
  <head>
    <title>Webside</title>

    <style>
      /* styles go here */
    </style>

    <script type="text/javascript">
      // code goes here
    </script>
  </head>

  <body>
    <h1>Webside</h1>
  </body>
</html>
```

Lagre (ctrl + s eller cmd + s)
Gå tilbake til mappen og dobbeltklikk på index.html for å åpne den i nettleseren

## Gjør en endring

1. Endre teksten i title `<title>{din tekst her}</title>`
2. Lagre, gå til nettleseren og trykk refresh (ctrl eller cmd + r)
3. Gjør det sammen med teksten i `<h1>`-elementet i `<body>`

## Nyttige elementer:

De fleste elementer følger samme oppbygning:

`<navn-på-element>innhold</navn-på-element>`

Vi kaller disse åpne-og-lukke tags

`<>  </>`

```html
Headings
<h1>{tekst her}</h1>
- bytt ut ett-tallet med større tall for underoverskrifter
```

Tekst

```html
<p>{tekst her}</p>
Avsnitt <span>{tekst her}</span> Tekst som ikke brytes <b>{tekst her}</b> fet
tekst
```

Bilder
Img-elementet er ett av elementene som ikke har åpne-lukke tag par,

```html
<img src="sti-til-bilde.jpg" alt="alternativ-tekst" />
```

Link

```html
<a href="link-til-sted.html">{Tekst her}</a>
```

Container for andre elementer

```html
<div>{elementer her}</div>
```

Knapp

```html
<button>Trykk her</button>
```

Lister

```html
<ul>
  - betyr unordered list
  <li></li>
  - li står for list item
</ul>

<ol>
  - betyr ordered list (nummerert)
  <li></li>
  - li står for list item
</ol>
```

Se disse sidene for inspirasjon

- https://www.w3schools.com/html/html_examples.asp
- https://htmlcheatsheet.com/
