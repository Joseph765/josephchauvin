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
    <meta charset="UTF-8">
    <meta name="description" content="Music Composer For 2D Action Games">
    <meta name="keywords" content="Video Game Music Composer">
    <meta name="author" content="Joseph Chauvin">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <meta property="og:image" content="http://josephchauvin.com/me-in-the-studio.jpg">
    <meta property="og:image:type" content="image/png">
    <meta property="og:image:width" content="1024">
    <meta property="og:image:height" content="1024">
</svelte:head>

<div class="layout">
    <section>
        <Nav />
        <Hero />
    </section>
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
    
    section {
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