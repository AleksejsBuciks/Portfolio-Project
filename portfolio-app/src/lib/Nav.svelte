<script>
    import { onMount } from 'svelte';
  let menuOpen = false;
  
  function toggleMenu() {
    menuOpen = !menuOpen;   
  } 

  import { base } from '$app/paths';

</script>

<nav class="navbar">

    <button class="menu-button" on:click={toggleMenu} aria-label="Toggle menu">
      &#9776; Menu
    </button>
    <div class="brand">Portfolio</div>
      
  </nav>
  
  <div class="side-menu {menuOpen ? 'open' : ''}">
  
    <a href="{base}/">Home</a>
    <a href="{base}/Projects">Projects</a>
    <a href="{base}/About">About</a>
    <a href="{base}/Contact">Contact</a>
  
  </div>

<style>

 .navbar {
    display: flex;
    justify-content: center;
    align-items: center;
    background-color: #141d26;
    color: white;
    padding: 10px 20px;
    font-size: 18px;
    position: fixed;
    width: 100%;
    top: 0;
    z-index: 1000;
    position: relative;
}

.menu-button {
    position: absolute;
    left: 20px;
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

</style>