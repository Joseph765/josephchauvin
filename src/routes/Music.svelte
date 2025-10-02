<script>
    import { Divider, Section, Text, Heading, Container, Flex, Link } from "$lib/components";
</script>

<section id="music">
    <Container>
        <Heading style="padding-bottom: 2rem; color: var(--gray-1);">Demo Reel</Heading>
        <Flex direction="column" gap="l">
            <!-- Retro Action Music Pack -->
            <!-- <iframe style="display: block; max-width: 900px; width: calc(100vw - 5rem); height: auto; aspect-ratio: 16/9; padding-inline: 0rem;" src="https://www.youtube.com/embed/cY4oApBxKyI?si=-2CQ9M4HUJBHUg1X" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
            <Flex direction="column" gap="m" align="center">
                <Text><a href="https://josephchauvin.itch.io/retro-action-music-pack" target="_blank">Retro Action Music Pack</a> is out now! Enjoy 10 action-packed track loops suitable for retro-styled games.</Text>
                <Text style="width: 100%;">Available on Itch & Game Dev Market.</Text>
            </Flex>
            <Divider space="none" /> -->
            <!-- Iconoclasts Recomposed YouTube Video -->
            <!-- <iframe style="display: block; max-width: 900px; width: calc(100vw - 5rem); height: auto; aspect-ratio: 16/9; padding-inline: 0rem;" src="https://www.youtube.com/embed/kRZNdofcpoI?si=oreRsJjt2ofW0xY4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
            <Flex direction="column" align="center">
                <Text>Enjoy a recomposition I did for the game Iconoclasts which perfectly encapsulates my style as a video game composer.</Text>
                </Flex> -->
            <iframe style="display: block; max-width: 900px; width: calc(100vw - 5rem); height: auto; aspect-ratio: 16/9; padding-inline: 0rem;" src="https://www.youtube.com/embed/aPZhcU34UEI?si=ch-Zv4n1LhlzYh5G" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
            <Text style="color: var(--gray-1);">Enjoy a handful of tracks I made inspired by the genre defining "Metroid" series.</Text>
            <!-- <Divider space="none" /> -->
            <!-- ReelCrafter reel: Demo Reel -->
            <!-- <iframe
                title="Demo Reel"
                width="100%"
                height="400"
                scrolling="no"
                frameborder="no"
                src="https://play.reelcrafter.com/embed/411f2358-fac7-499a-980e-3c9e85fadd2f">
            </iframe> -->
            <!-- Spotify Kinect EP -->
            <!-- <iframe title="Kinetic EP" style="border-radius:12px" src="https://open.spotify.com/embed/album/2KXETLWscghzck2sIuHrMT?utm_source=generator" width="100%" height="352" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe> -->
        </Flex>
    </Container>
</section>

<style>
    section {
        background: var(--gray-12);
        display: flex;
        align-items: center;
        flex-direction: column;
        padding-block: 4rem;
        color: var(--gray-1);
        min-height: 60dvh;
    }

    a {
        font-family: var(--font-family);
        font-weight: 350;
        color: var(--color-text-link);
        letter-spacing: 1px;
    }
</style>