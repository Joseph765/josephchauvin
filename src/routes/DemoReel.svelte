<script>
    import { Divider, Section, Text, Heading, Container, Flex, Link } from "$lib/components";
</script>

<section id="demoreel">
    <Container>
        <Heading style="padding-bottom: 2rem;">Demo Reel</Heading>
        <Flex direction="column" gap="l">
            <iframe style="display: block; max-width: 800px; width: calc(100vw - 5rem); height: auto; aspect-ratio: 16/9; padding-inline: 0rem;" src="https://www.youtube.com/embed/KvZztfj-aA4?si=mCjWf5R-va-2KVx-" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
            <Text>Enjoy a sound redesign I did for Metroid Prime 4!</Text>
        </Flex>
    </Container>
</section>

<style>
    section {
        display: flex;
        align-items: center;
        flex-direction: column;
        /* padding-block: 4rem; */
        color: var(--v-gray-1);
        min-height: 60dvh;
    }
</style>