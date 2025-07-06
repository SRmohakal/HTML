# 🟢 **Lesson 10: HTML5 APIs and Advanced Techniques**

---

## 📝 **1️⃣ Geolocation API**

Get user location (with permission).

**Basic example (requires JavaScript):**

```html
<button onclick="getLocation()">Show My Location</button>
<p id="location"></p>

<script>
function getLocation() {
  if (navigator.geolocation) {
    navigator.geolocation.getCurrentPosition(showPosition);
  } else {
    document.getElementById("location").innerText = "Geolocation not supported.";
  }
}

function showPosition(position) {
  document.getElementById("location").innerText =
    "Latitude: " + position.coords.latitude + 
    ", Longitude: " + position.coords.longitude;
}
</script>
```

---

## 📝 **2️⃣ Drag and Drop API**

Make elements draggable and droppable.

**Basic example:**

```html
<div id="drag1" draggable="true" ondragstart="drag(event)" style="width:100px;height:100px;background-color:skyblue;">
  Drag me
</div>

<div id="dropzone" ondrop="drop(event)" ondragover="allowDrop(event)" style="width:150px;height:150px;border:2px dashed #ccc;margin-top:20px;">
  Drop here
</div>

<script>
function allowDrop(ev) {
  ev.preventDefault();
}

function drag(ev) {
  ev.dataTransfer.setData("text", ev.target.id);
}

function drop(ev) {
  ev.preventDefault();
  var data = ev.dataTransfer.getData("text");
  ev.target.appendChild(document.getElementById(data));
}
</script>
```

---

## 📝 **3️⃣ Local Storage**

Save data in browser storage that persists between sessions.

**Example:**

```html
<input type="text" id="nameInput" placeholder="Enter your name">
<button onclick="saveName()">Save</button>
<p id="greeting"></p>

<script>
function saveName() {
  var name = document.getElementById("nameInput").value;
  localStorage.setItem("username", name);
  showGreeting();
}

function showGreeting() {
  var name = localStorage.getItem("username");
  if (name) {
    document.getElementById("greeting").innerText = "Hello, " + name + "!";
  }
}

showGreeting();
</script>
```

---

## 📝 **4️⃣ Interaction with HTML**

While HTML defines the structure, these APIs use JavaScript to make pages interactive. You now know the **starting point** for integrating HTML with advanced browser features.

---

