<section id="music">
    <div class="container is-size-l">
        <h3>Demos</h3>
        <div class="songs">
            <div class="song">
                <h4>Retro</h4>
                <audio controls>
                    <source src="/src/lib/assets/songs/Rush.wav" type="audio/wav">
                    Your browser does not support the audio element.
                </audio>
            </div>
            <div class="song">
                <h4>Boss Battle</h4>
                <audio controls>
                    <source src="/src/lib/assets/songs/Boss Battle.wav" type="audio/wav">
                    Your browser does not support the audio element.
                </audio>
            </div>
            <div class="song">
                <h4>Uplifting</h4>
                <audio controls>
                    <source src="/src/lib/assets/songs/Home World.wav" type="audio/wav">
                    Your browser does not support the audio element.
                </audio>
            </div>
        </div>
        <!-- <div class="container is-size-xs">
            <iframe title="Kinect EP" style="border-radius: 12px;" src="https://open.spotify.com/embed/album/2KXETLWscghzck2sIuHrMT?utm_source=generator" width="100%" height="420" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
        </div> -->
    </div>
</section>

<style>
    section {
        padding-block: 6rem;
        background-color: var(--gray-1);
    }

    h3 {
        font-family: "Roboto Slab", sans-serif;
        font-size: 2rem;
        font-weight: 350;
        color: #d5d6d8;
        letter-spacing: 1px;
        text-transform: uppercase; 
        text-align: center;
        padding-bottom: 2rem;
    }

    .container {
        max-inline-size: 900px;
        margin: auto;
        padding-inline: 2rem;
    }

    .container.is-size-l {
        max-inline-size: 1200px;
    }

    /* .container.is-size-xs {
        max-inline-size: 450px;
    } */

    .songs {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
        gap: 1rem;
    }

    .song {
        /* width: calc(33% - 1rem); */
        border: 1px solid var(--gray-6);
        display: flex;
        flex-direction: column;
        /* justify-content: space-between; */
        /* gap: 2rem; */
        background: var(--gray-3);
        padding: 1rem;
        border-radius: 3px;
        /* aspect-ratio: 1/1; */
    }

    h4 {
        color: var(--gray-12);
        font-family: "Roboto Slab", sans-serif;
        font-size: 1.25rem;
        font-weight: 350;
        color: #d5d6d8;
        letter-spacing: 1px;
        text-transform: uppercase; 
        text-align: center;
        padding-bottom: 1rem;
    }

    audio {
        width: 100%;

    }
</style>