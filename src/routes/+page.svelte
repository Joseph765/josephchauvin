<script>
    function scrollTo(id) {
        document.getElementById(id).scrollIntoView();
    }
</script>

<div class="layout">
    <!-- <img alt="Elektron Digitone" src="/src/lib/assets/Digitone-Red.JPG" /> -->
    <!-- <img alt="Elektron Digitone" src="/src/lib/assets/Digitone-Digitakt.JPG" /> -->
    <img alt="Elektron Digitone" src="/unsplash-studio.jpg" />
    <div class="overlay"></div>
    <div class="title">
        <h1>Joseph Chauvin</h1>
        <h2>Video Game Composer</h2>
    </div>
    <div class="arrow-down">
        <button aria-label="scroll down" onclick={() => scrollTo("music")}>
            <svg xmlns="http://www.w3.org/2000/svg" width="36" height="36" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-move-down-icon lucide-move-down"><path d="M8 18L12 22L16 18"/><path d="M12 2V22"/></svg>
        </button>
    </div>
</div>
<div class="divider"></div>
<section id="music">
    <div class="container">
        <h3>Music</h3>
        <div class="container is-size-xs">
            <iframe title="Kinect EP" style="border-radius: 12px;" src="https://open.spotify.com/embed/album/2KXETLWscghzck2sIuHrMT?utm_source=generator" width="100%" height="420" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
        </div>
    </div>
</section>
<!-- <div class="divider"></div>
<section id="about">
    <div class="container">
        <h3>About</h3>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
    </div>
</section> -->
<div class="divider"></div>
<section id="contact">
    <div class="container">
        <h3>Contact</h3>
        <p>Joseph.chauvin102@gmail.com</p>
    </div>
</section>

<style>
    .layout {
        display: flex;
        align-items: center;
        flex-direction: column;
        color: var(--gray-12);
        height: 100dvh;
        width: 100dvw;
    }

    img {
        object-fit: cover;
        width: 100%;
        height: 100%;
        position: absolute;
        top: 0;
        left: 0;
    }

    .overlay {
        width: 100%;
        height: 100%;
        position: absolute;
        top: 0;
        left: 0;
        background: var(--indigo-1);
        opacity: 0.8;
    }

    .title {
        position: absolute;
        top: calc(50% - 97px);
        text-align: center;
        display: flex;
        align-items: center;
        flex-direction: column;
        gap: 16px;
    }

    .arrow-down {
        position: absolute;
        bottom: 5%;
    }

    h1 {
        font-family: "Roboto Slab", sans-serif;
        font-size: clamp(2.5rem, 8vw + 1.5rem, 5rem);
        font-weight: 315;
        margin: 0;
        letter-spacing: -3.5px;
        color: var(--gray-12);
    }

    h2 {
        font-family: "Roboto Slab", sans-serif;
        font-size: 1rem;
        font-weight: 450;
        color: #d5d6d8;
        letter-spacing: 2px;
        text-transform: uppercase;
    }

    h3 {
        font-family: "Roboto Slab", sans-serif;
        font-size: 2rem;
        font-weight: 350;
        color: #d5d6d8;
        letter-spacing: 1px;
        text-transform: uppercase; 
        text-align: center;
        padding-bottom: 1rem;
    }

    p {
        font-family: "Roboto Slab", sans-serif;
        font-size: 1rem;
        font-weight: 350;
        color: #d5d6d8;
        letter-spacing: 1px;
        text-align: center;
        padding-bottom: 1rem;
    }

    section {
        padding-block: 6rem;
        background-color: var(--gray-1);
    }

    .container {
        max-inline-size: 900px;
        margin: auto;
        padding-inline: 2rem;
    }

    .container.is-size-xs {
        max-inline-size: 450px;
    }

    .divider {
        border-top: 1px solid var(--gray-6);
    }

    button {
        appearance: none;
        background: none;
        border: none;
        color: var(--gray-12);
        cursor: pointer;
    }
</style>