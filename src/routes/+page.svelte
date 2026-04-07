<script>
    import Nav from "./Nav.svelte";
    import Hero from "./Hero.svelte";
    import DemoReel from "./DemoReel.svelte";
    import About from "./About.svelte";
    import Footer from "./Footer.svelte";
    import Contact from "./Contact.svelte";
	import { Divider } from "$lib/components";
</script>

<svelte:head>
	<title>Joseph Chauvin | Video Game Sound Designer</title>
    <meta charset="UTF-8">
    <meta name="description" content="Sound Designer For Video Games">
    <meta name="keywords" content="Video Game Sound Designer">
    <meta name="author" content="Joseph Chauvin">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</svelte:head>

<div class="layout">
    <Nav />
    <Hero />
    <Divider />
    <DemoReel />
    <Divider />
    <Footer />
</div>

<style>
    .layout {
        color: var(--v-color-text);
        overflow: hidden;
        padding-block-start: var(--header-height);
    }
</style>