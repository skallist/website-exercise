## Step 5 - legge til funksjonalitet

I dette steget skal vi legge litt JavaScript som gjør siden vår mer interaktiv

### Dark mode av/på

1. Åpne index.html og lim inn følgende i `<script>`-elementet:

```javascript
function toggleTheme() {
  const body = document.body;

  if (body.classList.contains("dark-mode")) {
    body.classList.remove("dark-mode");
  } else {
    body.classList.add("dark-mode");
  }
}
```

2. Oppdater CSS-en i `<style>`-elementet som følger:

```css
body {
  background-color: #fff;
  font-family: "Arial";
  margin: 2em;
  color: #1f5373;
  transition: background-color 0.5s, color 0.5s;
}

.dark-mode {
  background-color: #333;
  color: #fff;
}
.dark-mode p {
  background-color: #607b8c;
}
.dark-mode a {
  color: #a7d5f2;
}
```

3. Legg til en knapp i HTML-koden for å skru dark mode av og på

```html
<button onclick="toggleTheme()">Dark mode av/på</button>
```

4. Lagre endringene og refresh nettleseren

[Videre til Steg 6 - Do it yourself](../step-6-diy/README.md)
