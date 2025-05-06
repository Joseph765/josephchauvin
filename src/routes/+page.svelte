<script>
    import Music from "./Music.svelte";
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
    <Nav />
    <Hero />
</div>
<div class="divider"></div>
<Music />
<div class="divider"></div>
<About />
<div class="divider"></div>
<Contact />

<style>
    .layout {
        display: flex;
        align-items: center;
        flex-direction: column;
        color: var(--gray-12);
        height: 100vh;
        width: 100vw;
    }

    .divider {
        border-top: 1px solid var(--gray-6);
    }
</style>