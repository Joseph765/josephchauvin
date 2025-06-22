<script>
    import Nav from "./Nav.svelte";
    import Hero from "./Hero.svelte";
    import Music from "./Music.svelte";
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
    <!-- <meta property="og:image" content="http://josephchauvin.com/me-in-the-studio.jpg"> -->
    <meta property="og:image:type" content="image/png">
    <meta property="og:image:width" content="1024">
    <meta property="og:image:height" content="1024">
</svelte:head>

<div class="layout">
    <Nav />
    <Hero />
    <Music />
    <About />
    <Footer />
</div>

<style>
    .layout {
        color: var(--color-text);
        overflow: hidden;
        padding-block-start: 81px;
    }
</style>