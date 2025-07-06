# 🟢 **Lesson 4: Lists and Tables**

---

## 📝 **1️⃣ Unordered Lists**

An **unordered list** uses bullets:

```html
<ul>
  <li>HTML</li>
  <li>CSS</li>
  <li>JavaScript</li>
</ul>
```

🔹 **Explanation:**

* `<ul>` = Unordered List
* `<li>` = List Item

---

## 📝 **2️⃣ Ordered Lists**

An **ordered list** uses numbers:

```html
<ol>
  <li>Step One</li>
  <li>Step Two</li>
  <li>Step Three</li>
</ol>
```

🔹 **Tip:** You can change numbering style with CSS later.

---

## 📝 **3️⃣ Nesting Lists**

Lists can be nested inside each other:

```html
<ul>
  <li>Frontend
    <ul>
      <li>HTML</li>
      <li>CSS</li>
    </ul>
  </li>
  <li>Backend</li>
</ul>
```

---

## 📝 **4️⃣ Tables**

Tables organize data in rows and columns.

**Basic Table Example:**

```html
<table border="1">
  <tr>
    <th>Language</th>
    <th>Level</th>
  </tr>
  <tr>
    <td>HTML</td>
    <td>Beginner</td>
  </tr>
  <tr>
    <td>CSS</td>
    <td>Intermediate</td>
  </tr>
</table>
```

🔹 **Explanation:**

* `<table>` – Starts the table.
* `<tr>` – Table row.
* `<th>` – Table header (bold and centered by default).
* `<td>` – Table data cell.

---

**Adding a caption:**

```html
<table border="1">
  <caption>My Skills Table</caption>
  <tr>
    <th>Skill</th>
    <th>Level</th>
  </tr>
  <tr>
    <td>HTML</td>
    <td>Pro</td>
  </tr>
</table>
```

---

## 💻 **4️⃣ Exercise**

**Replace your `<body>` with this:**

```html
<body>
    <h1>My Learning Progress</h1>

    <h2>Topics Covered</h2>
    <ul>
        <li>HTML Basics</li>
        <li>Text Formatting</li>
        <li>Links and Images</li>
        <li>Lists and Tables</li>
    </ul>

    <h2>Steps to Learn</h2>
    <ol>
        <li>Practice daily</li>
        <li>Build projects</li>
        <li>Review and improve</li>
    </ol>

    <h2>My Skills Table</h2>
    <table border="1">
        <caption>Learning Progress</caption>
        <tr>
            <th>Topic</th>
            <th>Status</th>
        </tr>
        <tr>
            <td>HTML</td>
            <td>Learning</td>
        </tr>
        <tr>
            <td>CSS</td>
            <td>Upcoming</td>
        </tr>
    </table>
</body>
```

