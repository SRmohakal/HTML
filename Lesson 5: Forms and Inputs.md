# 🟢 **Lesson 5: Forms and Inputs**

---

## 📝 **1️⃣ The `<form>` Tag**

**Basic structure:**

```html
<form action="submit-page.html" method="post">
    <!-- Form fields go here -->
</form>
```

🔹 **Explanation:**

* `action` = Where to send the form data (we’ll often leave this blank in practice or use `#`).
* `method` = GET or POST (POST is used for sending secure data).

For learning, you can omit `action` and `method`.

---

## 📝 **2️⃣ Input Fields**

**Text input:**

```html
<label for="username">Username:</label>
<input type="text" id="username" name="username">
```

* `label` improves accessibility and usability.
* `for` links the label to the input’s `id`.

---

**Password input:**

```html
<label for="password">Password:</label>
<input type="password" id="password" name="password">
```

---

**Checkbox:**

```html
<label><input type="checkbox" name="subscribe"> Subscribe to newsletter</label>
```

---

**Radio buttons:**

```html
<p>Choose your role:</p>
<label><input type="radio" name="role" value="student"> Student</label>
<label><input type="radio" name="role" value="teacher"> Teacher</label>
```

*Note: All radio buttons in the same group must share the same `name`.*

---

**Select dropdown:**

```html
<label for="country">Country:</label>
<select id="country" name="country">
  <option value="bd">Bangladesh</option>
  <option value="us">USA</option>
  <option value="uk">UK</option>
</select>
```

---

**Textarea:**

```html
<label for="comments">Comments:</label>
<textarea id="comments" name="comments" rows="4" cols="50"></textarea>
```

---

## 📝 **3️⃣ Buttons**

**Submit button:**

```html
<button type="submit">Submit</button>
```

**Reset button:**

```html
<button type="reset">Reset</button>
```

---

## 💻 **5️⃣ Exercise**

**Replace your `<body>` with this example:**

```html
<body>
    <h1>Contact Form</h1>
    <form>
        <label for="name">Name:</label><br>
        <input type="text" id="name" name="name"><br><br>

        <label for="email">Email:</label><br>
        <input type="email" id="email" name="email"><br><br>

        <label for="message">Message:</label><br>
        <textarea id="message" name="message" rows="4" cols="50"></textarea><br><br>

        <label><input type="checkbox" name="subscribe"> Subscribe to newsletter</label><br><br>

        <p>Preferred Contact Method:</p>
        <label><input type="radio" name="contact" value="email"> Email</label>
        <label><input type="radio" name="contact" value="phone"> Phone</label><br><br>

        <label for="country">Country:</label>
        <select id="country" name="country">
            <option value="bd">Bangladesh</option>
            <option value="us">USA</option>
            <option value="uk">UK</option>
        </select><br><br>

        <button type="submit">Submit</button>
        <button type="reset">Reset</button>
    </form>
</body>
```

✅ **Open in browser—you should see:**

* A form with text fields
* A textarea
* Checkbox
* Radio buttons
* Dropdown
* Submit & Reset buttons

---
