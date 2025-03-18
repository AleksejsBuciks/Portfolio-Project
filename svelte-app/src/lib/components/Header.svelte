<script>
    import { Navigation } from "$lib"
</script>    

<header>
    <div class="logo">
        <img src="/logo.png" alt="Website Logo">
        <h1>My Svelte App</h1>
    </div>
    <Navigation />
</header>

<style>
    header {
        display: flex;
        align-items: center;
        justify-content: space-between;
        background-color: var(--primary-color);
        color: white;
        padding: 1rem;
    }

    .logo {
        display: flex;
        align-items: center;
    }

    .logo {
        width: 50px;
        margin-right: 0.625rem;
    }
</style>