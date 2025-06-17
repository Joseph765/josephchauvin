<script>
    import { Divider, Section, Text, Heading, Container, Flex } from "$lib/components";
</script>

<Divider />
<Section id="music">
    <Container>
        <Heading style="padding-bottom: 2rem;">Music</Heading>
        <Flex direction="column">
            <!-- Iconoclasts Recomposed YouTube Video -->
            <iframe style="display: block; max-width: 900px; width: calc(100vw - 5rem); height: auto; aspect-ratio: 16/9; padding-inline: 0rem;" src="https://www.youtube.com/embed/kRZNdofcpoI?si=oreRsJjt2ofW0xY4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
            <!-- ReelCrafter reel: Demo Reel -->
            <iframe
                title="Demo Reel"
                width="100%"
                height="400"
                scrolling="no"
                frameborder="no"
                src="https://play.reelcrafter.com/embed/411f2358-fac7-499a-980e-3c9e85fadd2f">
            </iframe>
        </Flex>
        <!-- <div class="container is-size-xs">
            <iframe title="Kinect EP" style="border-radius: 12px;" src="https://open.spotify.com/embed/album/2KXETLWscghzck2sIuHrMT?utm_source=generator" width="100%" height="420" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
        </div> -->
    </Container>
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

    .container.is-size-s {
        max-inline-size: 700px;
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