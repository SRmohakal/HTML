# 🟢 **HTML Tag Examples (Part 4: Lists, Forms, Interactive Elements)**

---

## 📝 **Lists**

✅ **Unordered List** (`<ul>`, `<li>`)
```html
<ul>
  <li>Apple</li>
  <li>Banana</li>
  <li>Cherry</li>
</ul>
```
*Creates a bulleted list.*

---

✅ **Ordered List** (`<ol>`, `<li>`)
```html
<ol>
  <li>First step</li>
  <li>Second step</li>
  <li>Third step</li>
</ol>
```
*Creates a numbered list.*

---

✅ **Definition List** (`<dl>`, `<dt>`, `<dd>`)
```html
<dl>
  <dt>HTML</dt>
  <dd>HyperText Markup Language</dd>
  <dt>CSS</dt>
  <dd>Cascading Style Sheets</dd>
</dl>
```
*For term-definition pairs.*

---

## 📋 **Forms**

✅ `<form>` – *Form container*
```html
<form action="/submit" method="post">
  <label for="username">Username:</label>
  <input type="text" id="username" name="username"><br><br>

  <label for="password">Password:</label>
  <input type="password" id="password" name="password"><br><br>

  <button type="submit">Login</button>
</form>
```

---

✅ `<input>` – *Input field types*
```html
<input type="text" placeholder="Text input">
<input type="email" placeholder="Email">
<input type="number" placeholder="Number">
<input type="date">
<input type="checkbox"> I agree
<input type="radio" name="choice" value="A"> A
<input type="radio" name="choice" value="B"> B
<input type="file">
<input type="submit" value="Send">
```

---

✅ `<textarea>` – *Multi-line text input*
```html
<textarea rows="4" cols="40">Default text here.</textarea>
```

---

✅ `<select>` + `<option>` – *Drop-down list*
```html
<select name="fruit">
  <option value="apple">Apple</option>
  <option value="banana">Banana</option>
  <option value="cherry">Cherry</option>
</select>
```

---

✅ `<optgroup>` – *Grouped options*
```html
<select>
  <optgroup label="Citrus">
    <option>Lemon</option>
    <option>Orange</option>
  </optgroup>
  <optgroup label="Berries">
    <option>Strawberry</option>
    <option>Blueberry</option>
  </optgroup>
</select>
```

---

✅ `<label>` – *Label for inputs*
```html
<label for="email">Email:</label>
<input type="email" id="email">
```

---

✅ `<fieldset>` + `<legend>` – *Grouping inputs*
```html
<fieldset>
  <legend>Personal Info</legend>
  <label for="fname">First name:</label>
  <input type="text" id="fname"><br><br>

  <label for="lname">Last name:</label>
  <input type="text" id="lname">
</fieldset>
```

---

✅ `<datalist>` – *Autocomplete options*
```html
<input list="browsers" name="browser">
<datalist id="browsers">
  <option value="Chrome">
  <option value="Firefox">
  <option value="Safari">
</datalist>
```

---

✅ `<output>` – *Calculation result*
```html
<form oninput="result.value=parseInt(a.value)+parseInt(b.value)">
  <input type="range" id="a" value="50">
  + <input type="number" id="b" value="25">
  = <output name="result">75</output>
</form>
```

---

✅ `<progress>` – *Progress bar*
```html
<progress value="70" max="100"></progress>
```

---

✅ `<meter>` – *Scalar measurement*
```html
<meter value="0.6">60%</meter>
```

---

## ⚙️ **Interactive Elements**

✅ `<details>` + `<summary>` – *Toggle content*
```html
<details>
  <summary>More Information</summary>
  <p>This content can be expanded or collapsed.</p>
</details>
```

---

✅ `<dialog>` – *Popup dialog*
```html
<dialog id="myDialog">
  <p>This is a dialog box.</p>
  <button onclick="document.getElementById('myDialog').close()">Close</button>
</dialog>

<button onclick="document.getElementById('myDialog').showModal()">Open Dialog</button>
```

---

✅ `<menu>` – *Commands or context menus*
```html
<menu>
  <li><button onclick="alert('Save!')">Save</button></li>
  <li><button onclick="alert('Load!')">Load</button></li>
</menu>
```

---
