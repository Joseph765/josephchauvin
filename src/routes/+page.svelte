<script>
    import Demos from "./Demos.svelte";
    import Contact from "./Contact.svelte";
    import Nav from "./Nav.svelte";
    import Hero from "./Hero.svelte";
    import About from "./About.svelte";
    import Footer from "./Footer.svelte";
</script>

<svelte:head>
	<title>Joseph Chauvin | Video Game Composer</title>
	<!-- <meta name="robots" content="noindex nofollow" /> -->
</svelte:head>

<div class="layout">
    <header>
        <Nav />
        <Hero />
    </header>
    <Demos />
    <About />
    <Contact />
    <Footer />
</div>

<style>
    .layout {
        color: var(--color-text);
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