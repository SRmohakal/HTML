# 🟢 **Lesson 9: Accessibility Basics**

---

## 📝 **1️⃣ Why Accessibility Matters**

* Over **1 billion people** worldwide have disabilities.
* Search engines also benefit from accessible HTML.
* Many countries have laws (e.g., ADA, WCAG).

✅ **Professional websites are always accessible.**

---

## 📝 **2️⃣ Alt Text for Images**

The `alt` attribute **describes images** for screen readers and shows fallback text.

✅ Example:

```html
<img src="cat.jpg" alt="A black cat sitting on a windowsill.">
```

❌ Bad example:

```html
<img src="cat.jpg" alt="">
```

*(Only use empty alt when the image is decorative.)*

---

## 📝 **3️⃣ Label Elements Clearly**

Always link labels to inputs using `for` and `id`:

```html
<label for="email">Email Address:</label>
<input type="email" id="email" name="email">
```

This helps screen readers announce the label when the input is focused.

---

## 📝 **4️⃣ Use Landmarks**

Semantic HTML makes it easier to navigate:

✅ Good:

```html
<main>
  <section>
    <h2>Blog Posts</h2>
    <article>
      <h3>Post Title</h3>
      <p>Post content...</p>
    </article>
  </section>
</main>
```

❌ Bad:

```html
<div>
  <div>
    <h2>Blog Posts</h2>
    ...
  </div>
</div>
```

**Landmarks like `<main>`, `<nav>`, `<header>`, `<footer>` help screen readers.**

---

## 📝 **5️⃣ ARIA Basics**

**ARIA (Accessible Rich Internet Applications)** attributes give extra information:

* `aria-label` adds a text label:

```html
<button aria-label="Close">X</button>
```

* `role` defines purpose:

```html
<div role="alert">Form submission failed.</div>
```

**Use ARIA only when semantic HTML doesn’t cover your needs.**

---

## 📝 **6️⃣ Keyboard Navigation**

✅ Make sure:

* All links and buttons can be tabbed to.
* Use `<button>` elements instead of `<div>` for clickable actions.

---

## 💻 **9️⃣ Exercise**

**Replace your `<body>` with this example and test tabbing through the page:**

```html
<body>
  <header>
    <h1>Accessible Page Example</h1>
    <nav>
      <a href="#main">Skip to Main Content</a> |
      <a href="#">Home</a> |
      <a href="#">About</a>
    </nav>
  </header>

  <main id="main">
    <section>
      <h2>About This Page</h2>
      <p>This page demonstrates basic accessibility techniques.</p>
    </section>

    <section>
      <h2>Image Example</h2>
      <img src="https://via.placeholder.com/150" alt="Placeholder image example">
    </section>

    <section>
      <h2>Contact Form</h2>
      <form>
        <label for="email">Email:</label><br>
        <input type="email" id="email" name="email"><br><br>

        <label for="message">Message:</label><br>
        <textarea id="message" name="message"></textarea><br><br>

        <button type="submit">Submit</button>
      </form>
    </section>
  </main>

  <footer>
    <p>&copy; 2025 Accessible Site</p>
  </footer>
</body>
```

