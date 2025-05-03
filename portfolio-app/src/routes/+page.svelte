<script>
    import Nav from '$lib/Nav.svelte';
    import Footer from '$lib/Footer.svelte';
    import Project from '$lib/Project.svelte';
    import Cont from '$lib/Cont.svelte';
</script>

<Nav></Nav>

<div class="greet">

  <p>Greetings! I am Alex and I design, research and code websites & games.</p>

</div>

<div class="projects">

  <a href="Projects">Projects</a>

</div>

<Footer></Footer>

<Project></Project>

<Cont></Cont>

<style>

.greet, .projects {
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

  
</style>    