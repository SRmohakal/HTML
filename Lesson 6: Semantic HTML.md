# 🟢 **Lesson 6: Semantic HTML**

---
**Semantic elements** clearly describe their purpose.

Compare:

❌ *Non-semantic:*

```html
<div id="header"></div>
```

✅ *Semantic:*

```html
<header></header>
```

Semantic tags are *self-descriptive*—you instantly know what they are for.

---

## 📝 **2️⃣ Common Semantic Tags**

| Tag            | Purpose                             |
| -------------- | ----------------------------------- |
| `<header>`     | Top of the page or section          |
| `<nav>`        | Navigation links                    |
| `<main>`       | Main content (one per page)         |
| `<section>`    | Thematic grouping of content        |
| `<article>`    | Independent piece of content        |
| `<aside>`      | Side content (ads, sidebars)        |
| `<footer>`     | Bottom of page or section           |
| `<figure>`     | Self-contained content with caption |
| `<figcaption>` | Caption for a `<figure>`            |
| `<mark>`       | Highlight text                      |
| `<time>`       | Date/time value                     |

---

## 📝 **3️⃣ Example Semantic Layout**

```html
<body>
  <header>
    <h1>My Website</h1>
    <nav>
      <a href="#">Home</a> |
      <a href="#">About</a> |
      <a href="#">Contact</a>
    </nav>
  </header>

  <main>
    <article>
      <h2>Welcome to My Site</h2>
      <p>This is a sample article showcasing semantic HTML.</p>
    </article>

    <section>
      <h2>Latest News</h2>
      <p>Our website just launched!</p>
    </section>
  </main>

  <aside>
    <h3>Sidebar</h3>
    <p>Related links and ads can go here.</p>
  </aside>

  <footer>
    <p>&copy; 2025 My Website</p>
  </footer>
</body>
```

---

## 💡 **Why Use Semantic HTML?**

✅ Easier to read and maintain
✅ Improves SEO ranking
✅ Helps screen readers for accessibility
✅ Future-proofs your code

---

## 💻 **6️⃣ Exercise**

**Replace your `<body>` with this markup and view in the browser:**

```html
<body>
  <header>
    <h1>My Personal Blog</h1>
    <nav>
      <a href="#">Home</a> |
      <a href="#">Posts</a> |
      <a href="#">About Me</a>
    </nav>
  </header>

  <main>
    <article>
      <h2>First Blog Post</h2>
      <p>Today I learned about semantic HTML and why it's important.</p>
    </article>

    <section>
      <h2>Upcoming Topics</h2>
      <ul>
        <li>HTML5 APIs</li>
        <li>Accessibility</li>
        <li>SEO Best Practices</li>
      </ul>
    </section>
  </main>

  <aside>
    <h3>About the Author</h3>
    <p>I am learning to become a professional web developer.</p>
  </aside>

  <footer>
    <p>&copy; 2025 My Personal Blog</p>
  </footer>
</body>
```

✅ **What you should see:**

* A page with a header, navigation links, main content, sidebar, and footer.

---

