<!-- <img alt="Elektron Digitone" src="/src/lib/assets/Digitone-Red.JPG" /> -->
<!-- <img alt="Elektron Digitone" src="/src/lib/assets/Digitone-Digitakt.JPG" /> -->
<img alt="Elektron Digitone" src="/unsplash-studio.jpg" />
<div class="overlay"></div>
<div class="title">
    <h1>Music Composer For 2D Action Games</h1>
    <!-- <h2>Video Game Composer</h2> -->
    <!-- <button>Click Here</button> -->
</div>
<!-- <div class="arrow-down">
    <button aria-label="scroll down" onclick={() => scrollTo("music")}>
        <svg xmlns="http://www.w3.org/2000/svg" width="36" height="36" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-move-down-icon lucide-move-down"><path d="M8 18L12 22L16 18"/><path d="M12 2V22"/></svg>
    </button>
</div> -->

<style>
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
        top: calc(50% - 102px);
        text-align: center;
        display: flex;
        align-items: center;
        flex-direction: column;
        gap: 16px;
    }

    /* .arrow-down {
        position: absolute;
        bottom: 5%;
    } */

    h1 {
        font-family: "Roboto Slab", sans-serif;
        font-size: clamp(2.5rem, 4.5vw + 1.5rem, 5rem);
        font-weight: 315;
        margin: 0;
        letter-spacing: -3.5px;
        color: var(--gray-12);
        max-inline-size: 720px;
        line-height: 1.2;
    }
/* 
    h2 {
        font-family: "Roboto Slab", sans-serif;
        font-size: 1rem;
        font-weight: 450;
        color: #d5d6d8;
        letter-spacing: 2px;
        text-transform: uppercase;
    }

    button {
        appearance: none;
        background: none;
        border: none;
        color: var(--gray-12);
        cursor: pointer;
    } */
</style>