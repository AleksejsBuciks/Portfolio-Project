<script>
    import { onMount } from 'svelte';
    
    onMount(() => {
      console.log("Home Page Loaded");  
    })

    const hamMenu = document.querySelector(".ham-menu");

    const offScreenMenu = document.querySelector(".off-screen-menu");
    
    hamMenu?.addEventListener("click", () => {
      hamMenu.classList.toggle("active");
      offScreenMenu?.classList.toggle("active");
    });

</script>

<div class="Heading">
    
<h1>Portfolio</h1>

<div class="off-screen-menu">
  
  <ul>
          <li>Home</li>
      <li>About Me</li>
      <li>Projects</li>
      <li>Contact</li>
  </ul>
</div>

<nav>
  <div class="ham-menu">
      <span></span>
      <span></span>
      <span></span>
  </div>
</nav>

</div>



<style>
      
  .Heading {
    text-align: center;
  }

  .off-screen-menu{
    background-color: black;
    height: 100vh;
    width: 100%;
    max-width: 450px;
    position: fixed;
    top: 0;
    right: -450px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    font-size: 3rem;
    transition: .3s ease;
   }
   .off-screen-menu.active{
    right: 0;
   }

   nav {
    padding: 1rem;
    display: flex;
    background-color: #141d26;
   }

   .ham-menu{
    height: 50px;
    width: 50px;
    margin-left: auto;
    position: relative;
   }

   .ham-menu span{
    height: 5px;
    width: 100%;
    background-color: #7d0edf;
    border-radius: 25px;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    transition: .3s ease;
   }

   .ham-menu span:nth-child(1){
    top: 25%;
   } 

   .ham-menu span:nth-child(3){
    top: 75%;
   }

   .ham-menu.active span:nth-child(1){
    top: 50%;
    transform: translate(-50%, -50%) rotate(45deg);
   }

   .ham-menu.active span:nth-child(2){
    opacity: 0;
   }

   .ham-menu.active span:nth-child(3){
    top: 50%;
    transform: translate(-50%, -50%) rotate(-45deg);
   }
</style>    