<script>
    import { Button, Container, Flex, Text } from "$lib/components";
	import Divider from "$lib/components/Divider.svelte";
</script>

<section id="hero">
    <Container size="xl">
        <Flex direction="column" gap="l" align="center">
            <iframe style="display: block; max-width: 1000px; width: calc(100vw - 2rem); height: auto; aspect-ratio: 16/9; padding-inline: 0rem;" src="https://www.youtube.com/embed/KvZztfj-aA4?si=mCjWf5R-va-2KVx-" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
            <Text align="center">Hello! I'm Joseph, a video game sound designer. I create immersive and satisfying sound effects that bring games to life.</Text>
        </Flex>
    </Container>
</section>

<style>
    section {
        display: flex;
        align-items: center;
        flex-direction: column;
        padding-block: 6rem 4rem;
        color: var(--v-color-text);
        background-color: var(--v-color-background);
    }

    iframe {
        border-radius: var(--v-radius-rounded);
    }

    @media only screen and (max-width: 700px) { 
        section {
            padding-block: 6rem 2rem;
        }
    }
</style>