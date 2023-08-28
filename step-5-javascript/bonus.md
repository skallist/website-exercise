## Bonus

Under følger noen flere funksjoner det går an å prøve ut

### Vis mer/mindre feature

JavaScript

```javascript
function toggleContent(id) {
  const content = document.getElementById(id);
  if (content.classList.contains("show-more")) {
    content.classList.remove("show-more");
  } else {
    content.classList.add("show-more");
  }
}
```

CSS

```css
.content {
  overflow: hidden;
  height: 50px;
}

.show-more {
  height: auto;
}
```

Eksempel innhold og knapp
HTML

```html
<div class="content" id="description1">Lang beskrivelse...</div>
<button onclick="toggleContent('description1')">Show More/Less</button>
```

### Smooth scroll til seksjon

JavaScript

```javascript
function smoothScroll(targetId) {
  const target = document.getElementById(targetId);
  target.scrollIntoView({ behavior: "smooth" });
}
```

HTML

```html
<a href="javascript:void(0)" onclick="smoothScroll('section2')"
  >Go to Section 2</a
>
...
<div id="section2">Content of section 2</div>
```

### Skills bar

JavaScript

```javascript
window.addEventListener("scroll", () => {
  const skillBar = document.getElementById("skillBar1");
  const position = skillBar.getBoundingClientRect();
  if (position.top < window.innerHeight && position.bottom >= 0) {
    skillBar.style.width = skillBar.getAttribute("data-skill-level");
  }
});
```

CSS

```css
.skill-bar {
  height: 20px;
  width: 0;
  background-color: #3498db;
  transition: width 1s;
}
```

HTML

```html
<div class="skill-container">
  <div class="skill-bar" id="skillBar1" data-skill-level="80%"></div>
</div>
```
