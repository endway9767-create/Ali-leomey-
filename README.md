<!DOCTYPE html>
<html>
<head>
<title>My First Website</title>

<style>
body {
  background: #f2f2f2;
  text-align: center;
  font-family: Arial;
  padding: 50px;
}

h1 {
  color: black;
}

button {
  padding: 10px 20px;
  font-size: 18px;
}
</style>

</head>

<body>

<h1>Hello, I made my first website!</h1>

<p>My name is leomey.</p>

<button>Click Me</button>

</body>
</html><button onclick="showMessage()">Click Me</button>

<p id="message"></p><!DOCTYPE html>
<html>
<head>
<title>My Portfolio</title>

<style>
body {
  margin: 0;
  font-family: Arial, sans-serif;
  background: #f4f6f9;
}

/* NAVBAR */
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: #1e2a38;
  padding: 15px 30px;
  color: white;
}

.navbar a {
  color: white;
  text-decoration: none;
  margin: 0 10px;
}

.navbar a:hover {
  color: #00c2ff;
}

/* HERO SECTION */
.hero {
  text-align: center;
  padding: 80px 20px;
  background: linear-gradient(135deg, #00c2ff, #0077ff);
  color: white;
}

.hero h1 {
  font-size: 40px;
  margin-bottom: 10px;
}

/* CARDS */
.container {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  padding: 40px;
  gap: 20px;
}

.card {
  background: white;
  width: 250px;
  padding: 20px;
  border-radius: 12px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
  text-align: center;
  transition: 0.3s;
}

.card:hover {
  transform: translateY(-5px);
}

/* BUTTON */
button {
  padding: 10px 15px;
  border: none;
  background: #0077ff;
  color: white;
  border-radius: 6px;
  cursor: pointer;
}

button:hover {
  background: #005ccc;
}
</style>

</head>

<body>

<!-- NAVBAR -->
<div class="navbar">
  <div><b>My Website</b></div>
  <div>
    <a href="#">Home</a>
    <a href="#">About</a>
    <a href="#">Projects</a>
    <a href="#">Contact</a>
  </div>
</div>

<!-- HERO -->
<div class="hero">
  <h1>Hi, I'm a Web Developer</h1>
  <p>I build modern websites using HTML, CSS & JavaScript</p>
  <button onclick="showMessage()">Hire Me</button>
  <p id="message"></p>
</div>

<!-- CARDS -->
<div class="container">

  <div class="card">
    <h3>Project 1</h3>
    <p>Simple website design</p>
  </div>

  <div class="card">
    <h3>Project 2</h3>
    <p>Responsive landing page</p>
  </div>

  <div class="card">
    <h3>Project 3</h3>
    <p>JavaScript mini app</p>
  </div>

</div>

<script>
function showMessage() {
  document.getElementById("message").innerHTML =
    "🚀 Thanks for visiting my portfolio!";
}
</script>

</body>
</html><!DOCTYPE html>
<html>
<head>
<title>My Portfolio</title>

<meta name="viewport" content="width=device-width, initial-scale=1.0">

<style>
:root {
  --bg: #f4f6f9;
  --text: #111;
  --card: #fff;
  --nav: #1e2a38;
  --accent: #0077ff;
}

body.dark {
  --bg: #0f172a;
  --text: #fff;
  --card: #1e293b;
  --nav: #0b1220;
  --accent: #38bdf8;
}

body {
  margin: 0;
  font-family: Arial;
  background: var(--bg);
  color: var(--text);
  transition: 0.3s;
}

/* NAV */
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: var(--nav);
  padding: 15px 20px;
  color: white;
  position: sticky;
  top: 0;
}

.navbar a {
  color: white;
  text-decoration: none;
  margin: 0 8px;
}

.navbar a:hover {
  color: var(--accent);
}

/* HERO */
.hero {
  text-align: center;
  padding: 70px 20px;
  background: linear-gradient(135deg, var(--accent), #4f46e5);
  color: white;
  animation: fadeIn 1s ease-in;
}

.hero h1 {
  font-size: 36px;
}

/* BUTTON */
button {
  padding: 10px 15px;
  border: none;
  background: white;
  color: black;
  border-radius: 6px;
  cursor: pointer;
  margin-top: 10px;
}

button:hover {
  opacity: 0.8;
}

/* CARDS */
.container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 15px;
  padding: 30px;
}

.card {
  background: var(--card);
  width: 250px;
  padding: 20px;
  border-radius: 12px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
  transition: transform 0.3s;
}

.card:hover {
  transform: translateY(-8px);
}

/* CONTACT */
.contact {
  text-align: center;
  padding: 40px;
}

input, textarea {
  width: 80%;
  max-width: 400px;
  padding: 10px;
  margin: 8px;
  border-radius: 6px;
  border: 1px solid #ccc;
}

/* ANIMATION */
@keyframes fadeIn {
  from {opacity: 0; transform: translateY(-20px);}
  to {opacity: 1; transform: translateY(0);}
}
</style>

</head>

<body>

<div class="navbar">
  <div><b>My Portfolio</b></div>
  <div>
    <a href="#">Home</a>
    <a href="#projects">Projects</a>
    <a href="#contact">Contact</a>
    <a href="#" onclick="toggleDark()">🌙</a>
  </div>
</div>

<div class="hero">
  <h1>Hi, I'm a Web Developer</h1>
  <p>I build modern websites</p>
  <button onclick="showMessage()">Hire Me</button>
  <p id="msg"></p>
</div>

<div id="projects" class="container">

  <div class="card">
    <h3>Project 1</h3>
    <p>Modern website design</p>
  </div>

  <div class="card">
    <h3>Project 2</h3>
    <p>Landing page UI</p>
  </div>

  <div class="card">
    <h3>Project 3</h3>
    <p>JavaScript app</p>
  </div>

</div>

<div id="contact" class="contact">
  <h2>Contact Me</h2>
  <input placeholder="Your Name"><br>
  <input placeholder="Your Email"><br>
  <textarea placeholder="Message"></textarea><br>
  <button>Send</button>
</div>

<script>
function showMessage() {
  document.getElementById("msg").innerHTML =
    "🚀 Thanks! I will contact you soon.";
}

function toggleDark() {
  document.body.classList.toggle("dark");
}
</script>

</body>
</html>

