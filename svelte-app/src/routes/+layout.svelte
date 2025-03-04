<script>
    //Import components
    import {Header, Footer} from "$lib";
</script>

<Header />

<main>
    <slot />
</main>

<Footer />

<style>
    main{
        padding: 2rem;
        text-align: center;
    }
</style>    