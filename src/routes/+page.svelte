<script>
    import Demos from "./Demos.svelte";
    import Contact from "./Contact.svelte";
    import Nav from "./Nav.svelte";
    import Hero from "./Hero.svelte";
    import About from "./About.svelte";
</script>

<svelte:head>
	<title>Joseph Chauvin</title>
	<!-- <meta name="robots" content="noindex nofollow" /> -->
</svelte:head>

<div class="layout">
    <header>
        <Nav />
        <Hero />
    </header>
    <div class="divider"></div>
    <Demos />
    <!-- <div class="divider"></div>
    <About /> -->
    <div class="divider"></div>
    <Contact />
</div>

<style>
    .layout {
        color: var(--gray-12);
        overflow: hidden;
    }
    
    header {
        display: flex;
        align-items: center;
        flex-direction: column;
        height: 100vh;
        /* max-height: 100vh; */
        /* width: 100%; */
    }

    .divider {
        border-top: 1px solid var(--gray-6);
    }

    @media (pointer: coarse) {
        header {
            height: 100svh !important;
        }
    }
</style>