# 🟢 **HTML Tag Examples (Part 5: Scripting, Embedded Content, Language Tags)**

---

## 🧩 **Scripting and Templates**

✅ `<script>` – *JavaScript code*

```html
<script>
  console.log("Hello from JavaScript!");
</script>
```

✅ `<noscript>` – *Fallback if JavaScript is disabled*

```html
<noscript>
  <p>Please enable JavaScript to use this site.</p>
</noscript>
```

✅ `<template>` – *Reusable template content*

```html
<template id="cardTemplate">
  <div class="card">
    <h2></h2>
    <p></p>
  </div>
</template>

<script>
  const template = document.getElementById("cardTemplate");
  const clone = template.content.cloneNode(true);
  clone.querySelector("h2").textContent = "Dynamic Title";
  clone.querySelector("p").textContent = "Dynamic content here.";
  document.body.appendChild(clone);
</script>
```

✅ `<slot>` – *Web Components content placeholder*

```html
<template id="myComponent">
  <style>
    div { border: 1px solid #ccc; padding: 10px; }
  </style>
  <div>
    <slot></slot>
  </div>
</template>
```

*(Requires JavaScript to define a custom element.)*

---

## 🌍 **Embedded Content**

✅ `<iframe>` – *Embed another HTML page*

```html
<iframe src="https://example.com" width="400" height="300"></iframe>
```

✅ `<embed>` – *Embed external resources*

```html
<embed src="file.pdf" width="500" height="375">
```

✅ `<object>` – *Generic embedded content*

```html
<object data="file.pdf" type="application/pdf" width="500" height="375">
  <p>PDF cannot be displayed.</p>
</object>
```

✅ `<param>` – *Parameters for `<object>`*

```html
<object data="movie.swf">
  <param name="autoplay" value="true">
</object>
```

---

## 🏷️ **Language & Ruby Annotations**

✅ `<ruby>`, `<rt>`, `<rp>` – *Ruby annotations (pronunciation guides)*

```html
<ruby>
  漢 <rt>Kan</rt>
  字 <rt>ji</rt>
</ruby>
```

With fallback parentheses:

```html
<ruby>
  漢 <rp>(</rp><rt>Kan</rt><rp>)</rp>
  字 <rp>(</rp><rt>ji</rt><rp>)</rp>
</ruby>
```

---

✅ `<bdi>` – *Bidirectional isolation*

```html
<p>User: <bdi>مرحبا</bdi></p>
```

*Prevents text direction issues.*

---

✅ `<bdo>` – *Override text direction*

```html
<bdo dir="rtl">This text is right-to-left.</bdo>
```

---

✅ `<wbr>` – *Word break opportunity*

```html
<p>Thisisaverylong<wbr>wordthatmightbreak.</p>
```

---
