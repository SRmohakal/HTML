# 🟢 **Lesson 7: Multimedia – Audio & Video**

---

## 📝 **1️⃣ Embedding Video**

Use the `<video>` tag.

**Example:**

```html
<video width="400" controls>
  <source src="sample-video.mp4" type="video/mp4">
  <source src="sample-video.webm" type="video/webm">
  Your browser does not support the video tag.
</video>
```

🔹 **Explanation:**

* `width` sets the video width in pixels.
* `controls` shows Play, Pause, Volume, etc.
* `<source>` allows you to provide multiple formats.
* The text inside `<video>` is fallback content if the browser doesn’t support video.

---

✅ **Tip:**
If you don’t have a local video, you can use an online link:

```html
<video width="400" controls>
  <source src="https://www.w3schools.com/html/mov_bbb.mp4" type="video/mp4">
  Your browser does not support HTML video.
</video>
```

---

## 📝 **2️⃣ Embedding Audio**

Use the `<audio>` tag.

**Example:**

```html
<audio controls>
  <source src="sample-audio.mp3" type="audio/mpeg">
  <source src="sample-audio.ogg" type="audio/ogg">
  Your browser does not support the audio tag.
</audio>
```

🔹 **Explanation:**

* `controls` shows Play/Pause buttons.
* Multiple `<source>` tags improve compatibility.

---

## 📝 **3️⃣ Adding Captions**

**Captions require a separate file** (WebVTT).
Here’s an example with captions (optional for now):

```html
<video width="400" controls>
  <source src="sample-video.mp4" type="video/mp4">
  <track src="captions.vtt" kind="subtitles" srclang="en" label="English">
  Your browser does not support video.
</video>
```

*(You’d need to prepare `captions.vtt` for subtitles.)*

---

## 💻 **7️⃣ Exercise**

**Replace your `<body>` with this markup:**

```html
<body>
  <h1>My Multimedia Page</h1>

  <h2>Sample Video</h2>
  <video width="400" controls>
    <source src="https://www.w3schools.com/html/mov_bbb.mp4" type="video/mp4">
    Your browser does not support the video tag.
  </video>

  <h2>Sample Audio</h2>
  <audio controls>
    <source src="https://www.w3schools.com/html/horse.mp3" type="audio/mpeg">
    Your browser does not support the audio tag.
  </audio>
</body>
```

✅ **Open in your browser—you should see:**

* A video player (click Play)
* An audio player (click Play)

---
