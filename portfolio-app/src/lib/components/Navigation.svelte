<script>
    
</script>

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

<style>
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
   .off-screen-menu:active{
    right: 0;
   }

   nav {
    padding: 1rem;
    display: flex;
    background-color: aquamarine;
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
    background-color: violet;
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
</style>