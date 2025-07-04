# 🟢 **Lesson 3: Links and Images**

---

## 📝 **1️⃣ Hyperlinks**

Use the `<a>` tag to make a link.

**Basic example:**

```html
<a href="https://www.google.com">Visit Google</a>
```

🔹 **Explanation:**

* `<a>` means “anchor”.
* `href` specifies the URL.
* The text between `<a>` and `</a>` is clickable.

**Open link in a new tab:**

```html
<a href="https://www.google.com" target="_blank">Open Google in New Tab</a>
```

* `target="_blank"` tells the browser to open a new tab.

---

## 📝 **2️⃣ Images**

Use the `<img>` tag to display an image.

**Example:**

```html
<img src="https://via.placeholder.com/150" alt="Placeholder Image">
```

🔹 **Explanation:**

* `src` is the image URL.
* `alt` is the alternative text if the image doesn’t load (and for screen readers).

---

## 📝 **3️⃣ Combining Links and Images**

Make an image clickable:

```html
<a href="https://www.wikipedia.org">
    <img src="https://via.placeholder.com/150" alt="Wikipedia">
</a>
```

When you click the image, you go to Wikipedia.

---

## 💻 **3️⃣ Exercise**

**Replace your `<body>` with this:**

```html
<body>
    <h1>Welcome to My Webpage</h1>
    <p>Here are some useful links:</p>
    <ul>
        <li><a href="https://www.google.com" target="_blank">Google</a></li>
        <li><a href="https://www.wikipedia.org" target="_blank">Wikipedia</a></li>
    </ul>
    
    <h2>My Favorite Image</h2>
    <img src="https://via.placeholder.com/300" alt="Sample Image">
    
    <p>Click the image to visit Wikipedia:</p>
    <a href="https://www.wikipedia.org" target="_blank">
        <img src="https://via.placeholder.com/150" alt="Clickable Image">
    </a>
</body>
```

---

✅ **What you should see:**

* Two clickable links that open in new tabs
* A large image
* A smaller clickable image

---
