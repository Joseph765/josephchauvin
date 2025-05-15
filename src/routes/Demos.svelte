<script>
    import { Divider, Section, Text, Heading } from "$lib/components";
</script>

<Divider />
<Section id="music">
    <div class="container is-size-l">
        <Heading style="padding-bottom: 2rem;">Music</Heading>
        <!-- <div class="songs">
            <div class="song">
                <Heading size="s" style="padding-bottom: 1rem;">Retro</Heading>
                <audio controls>
                    <source src="/songs/Rush.wav" type="audio/wav">
                    Your browser does not support the audio element.
                </audio>
            </div>
            <div class="song">
                <Heading size="s" style="padding-bottom: 1rem;">Boss Battle</Heading>
                <audio controls>
                    <source src="/songs/Boss Battle.wav" type="audio/wav">
                    Your browser does not support the audio element.
                </audio>
            </div>
            <div class="song">
                <Heading size="s" style="padding-bottom: 1rem;">Adventure</Heading>
                <audio controls>
                    <source src="/songs/Blockrock.wav" type="audio/wav">
                    Your browser does not support the audio element.
                </audio>
            </div>
        </div> -->
        <!-- ReelCrafter reel: Demo Reel -->
        <iframe
            title="Demo Reel"
            width="100%"
            height="400"
            scrolling="no"
            frameborder="no"
            src="https://play.reelcrafter.com/embed/411f2358-fac7-499a-980e-3c9e85fadd2f">
        </iframe>
        <!-- <div class="container is-size-xs">
            <iframe title="Kinect EP" style="border-radius: 12px;" src="https://open.spotify.com/embed/album/2KXETLWscghzck2sIuHrMT?utm_source=generator" width="100%" height="420" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
        </div> -->
    </div>
</Section>

<style>
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

    audio {
        width: 100%;

    }
</style>