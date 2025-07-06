# 🟢 **HTML Tag Examples (Part 3: Hyperlinks, Media, Tables)**

---

## 🔗 **Hyperlinks**

✅ `<a>` – *Anchor / Link*
```html
<a href="https://www.example.com" target="_blank">Visit Example</a>
```
- `href` sets the URL.
- `target="_blank"` opens in a new tab.

---

## 📷 **Images and Media**

✅ `<img>` – *Image*
```html
<img src="cat.jpg" alt="A cute cat" width="300">
```
- `alt` is required for accessibility.

---

✅ `<figure>` + `<figcaption>`
```html
<figure>
  <img src="sunset.jpg" alt="Sunset over the ocean">
  <figcaption>Beautiful sunset at the beach.</figcaption>
</figure>
```

---

✅ `<picture>` – *Responsive Images*
```html
<picture>
  <source srcset="large.jpg" media="(min-width: 800px)">
  <source srcset="small.jpg">
  <img src="fallback.jpg" alt="Responsive image example">
</picture>
```

---

✅ `<map>` + `<area>` – *Image Map*
```html
<img src="planets.jpg" usemap="#planetmap" alt="Planets">

<map name="planetmap">
  <area shape="rect" coords="0,0,100,100" href="mercury.html" alt="Mercury">
  <area shape="circle" coords="200,200,50" href="venus.html" alt="Venus">
</map>
```
- `shape`: rect, circle, poly
- `coords`: pixel coordinates

---

✅ `<canvas>` – *Drawing Area (via JavaScript)*
```html
<canvas id="myCanvas" width="200" height="100" style="border:1px solid #000;"></canvas>

<script>
  var c = document.getElementById("myCanvas");
  var ctx = c.getContext("2d");
  ctx.fillStyle = "blue";
  ctx.fillRect(10,10,150,75);
</script>
```

---

✅ `<svg>` – *Scalable Vector Graphics*
```html
<svg width="100" height="100">
  <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow" />
</svg>
```

---

✅ `<video>` – *Embedded Video*
```html
<video width="320" controls>
  <source src="movie.mp4" type="video/mp4">
  Your browser does not support video.
</video>
```

---

✅ `<audio>` – *Embedded Audio*
```html
<audio controls>
  <source src="audio.mp3" type="audio/mpeg">
  Your browser does not support audio.
</audio>
```

---

✅ `<source>` – *Media Source*
Used inside `<video>`, `<audio>`, or `<picture>` to define files:
```html
<video controls>
  <source src="video.mp4" type="video/mp4">
  <source src="video.webm" type="video/webm">
</video>
```

---

✅ `<track>` – *Captions / Subtitles*
```html
<video controls>
  <source src="movie.mp4" type="video/mp4">
  <track src="subtitles.vtt" kind="subtitles" srclang="en" label="English">
</video>
```

---

## 🧮 **Tables**

✅ `<table>` – *Table container*
```html
<table border="1">
  <tr>
    <th>Item</th>
    <th>Price</th>
  </tr>
  <tr>
    <td>Apple</td>
    <td>$1</td>
  </tr>
</table>
```

---

✅ `<caption>` – *Table caption*
```html
<table border="1">
  <caption>Monthly Sales</caption>
  <tr><th>Month</th><th>Sales</th></tr>
  <tr><td>January</td><td>$1000</td></tr>
</table>
```

---

✅ `<thead>`, `<tbody>`, `<tfoot>`
```html
<table border="1">
  <thead>
    <tr><th>Product</th><th>Price</th></tr>
  </thead>
  <tbody>
    <tr><td>Pen</td><td>$2</td></tr>
    <tr><td>Notebook</td><td>$5</td></tr>
  </tbody>
  <tfoot>
    <tr><td>Total</td><td>$7</td></tr>
  </tfoot>
</table>
```

---

✅ `<colgroup>` + `<col>`
```html
<table border="1">
  <colgroup>
    <col span="1" style="background-color:lightgray;">
    <col span="1" style="background-color:lightyellow;">
  </colgroup>
  <tr><th>Name</th><th>Age</th></tr>
  <tr><td>Alice</td><td>30</td></tr>
</table>
```

---

