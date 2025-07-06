# 🟢 **Lesson 8: Meta Tags and SEO Basics**

---
Meta tags provide **metadata**—information about your web page that isn’t displayed to users but is read by:

* Browsers
* Search engines
* Social media platforms

They always go inside `<head>`.

---

## 📝 **2️⃣ Common Meta Tags**

✅ **Character encoding**
Sets how text characters are interpreted (use UTF-8):

```html
<meta charset="UTF-8">
```

✅ **Viewport settings**
Helps your page look good on mobile:

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

✅ **Description**
Appears in search engine results:

```html
<meta name="description" content="This is my personal website where I share HTML tutorials.">
```

✅ **Keywords** *(less important nowadays)*:

```html
<meta name="keywords" content="HTML, tutorials, web development">
```

✅ **Author**:

```html
<meta name="author" content="Your Name">
```

---

## 📝 **3️⃣ Example Complete `<head>`**

```html
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="A sample HTML page to learn meta tags and SEO basics.">
  <meta name="keywords" content="HTML, meta tags, SEO">
  <meta name="author" content="Your Name">
  <title>Meta Tags Example</title>
</head>
```

---

✅ **Pro Tip:**
Modern search engines mainly care about:

* `<title>`
* `<meta name="description">`
* Page content structure (headings, semantic tags)

---

## 📝 **4️⃣ Example Complete Page**

Here’s a **full HTML document** showing everything together:

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta name="description" content="A simple webpage demonstrating meta tags for SEO.">
  <meta name="keywords" content="HTML, SEO, meta tags">
  <meta name="author" content="Your Name">
  <title>My SEO-Friendly Page</title>
</head>
<body>
  <header>
    <h1>Welcome to My SEO-Friendly Page</h1>
  </header>
  <main>
    <article>
      <h2>Why Meta Tags Matter</h2>
      <p>Meta tags help improve how your site appears in search results and control the behavior of the browser.</p>
    </article>
  </main>
  <footer>
    <p>&copy; 2025 My Website</p>
  </footer>
</body>
</html>
```

---

