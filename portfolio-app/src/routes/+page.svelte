<script>
    import { onMount } from 'svelte';
  let menuOpen = false;

  onMount(() => {
    console.log("Home Page Loaded");  
  });

  function toggleMenu() {
    menuOpen = !menuOpen;
  } 

</script>

<nav class="navbar">

  <button class="menu-button" on:click={toggleMenu} aria-label="Toggle menu">
    &#9776; Menu
  </button>
  <div class="brand">Portfolio</div>
  <div class="contact">Socials</div>

</nav>

<div class="side-menu {menuOpen ? 'open' : ''}">

  <a href="/">Home</a>
  <a href="Projects">Projects</a>
  <a href="About">About</a>
  <a href="d">Contact</a>

</div>

<div class="greet">

  <p>Greetings! I am Alex and I design, research and code websites & games.</p>

</div>

<div class="projects">

  <p>Projects</p>

</div>

<div class="text-row">

  <div class="box">
    <div class="logo html">HTML<br>5</div>
    <p>I've worked extensively with HTML to create structured, responsive web pages and ensure cross-browser compatibility.</p>
  </div>

  <div class="box">
    <div class="logo js">JS</div>
    <p>I have hands-on experience with JavaScript, building dynamic and interactive web applications.</p>
  </div>

  <div class="box">
    <div class="logo css">C++</div>
    <p>I have experience using C++ to develop efficient, high-performance applications, utilizing object-oriented principles and managing memory effectively.</p>
  </div>

</div>


<style>

.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: #141d26;
  color: white;
  padding: 10px 20px;
  font-size: 18px;
  position: fixed;
  width: 100%;
  top: 0;
  z-index: 1000;
}

.menu-button {
  background: none;
  border: none;
  color: #7d0edf;
  font-size: 18px;
  cursor: pointer;
}
.menu-button:focus {
  outline: 2px solid #7d0edf;
}

.brand {
  color: #7d0edf;
  font-size: 24px;
}

.contact {
  color: white;
}

.side-menu {
  position: fixed;
  top: 0;
  left: -220px;
  width: 220px;
  height: 100vh;
  background-color: #1e2a38;
  padding: 60px 20px;
  box-shadow: 2px 0 5px rgba(0, 0, 0, 0.5);
  display: flex;
  flex-direction: column;
  gap: 20px;
  transition: left 0.3s ease;
  z-index: 999;
}

.side-menu.open {
  left: 0;
}

.side-menu a {
  color: white;
  text-decoration: none;
  font-size: 18px;
}

.side-menu a:hover {
  color: #7d0edf;
}

.greet, .projects, .text-row {
  margin-top: 100px;
}

  .greet {
    text-align: center;    
    font-size: 40px;
    margin-top: 175px;
    width: 40%;
    margin-left: 450px;
  }
  
  .projects {
    text-align: center;
    margin-top: 150px;
    font-size: 30px;
    color: aliceblue;
    background-color: #7d0edf;
    height: 50px;
    width: 175px;
    margin-left: 675px;
    border-radius: 100px;
  }

  .text-row {
  display: flex;
  justify-content: center;
  align-items: flex-start;
  margin-top: 250px;
  gap: 30px;
  flex-wrap: wrap;
}

.box {
  background-color: #7d0edf;
  padding: 20px;
  border-radius: 10px;
  width: 280px;
  text-align: center;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.3);
  color: white;
}

.logo {
  width: 60px;
  height: 60px;
  border-radius: 50%;
  margin: 0 auto 10px auto;
  display: flex;
  justify-content: center;
  align-items: center;
  font-weight: bold;
  font-size: 16px;
  color: white;
}

.logo.html {
  background-color: #e44d26;
}

.logo.js {
  background-color: #f7df1e;
  color: black;
}

.logo.css {
  background-color: #4dabf7;
}
</style>    