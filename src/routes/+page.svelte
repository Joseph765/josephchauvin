<script>
    import Nav from "./Nav.svelte";
    import Hero from "./Hero.svelte";
    import Music from "./Music.svelte";
    import About from "./About.svelte";
    import Footer from "./Footer.svelte";
    import Contact from "./Contact.svelte";
	import { Divider } from "$lib/components";
</script>

<svelte:head>
	<title>Joseph Chauvin | Video Game Composer</title>
    <meta charset="UTF-8">
    <meta name="description" content="Music Composer For 2D Action Games">
    <meta name="keywords" content="Video Game Music Composer">
    <meta name="author" content="Joseph Chauvin">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</svelte:head>

<div class="layout">
    <Nav />
    <Hero />
    <Divider />
    <Music />
    <!-- <About /> -->
    <Divider />
    <Contact />
    <Divider />
    <Footer />
</div>

<style>
    .layout {
        color: var(--color-text);
        overflow: hidden;
        padding-block-start: var(--header-height);
    }
</style>