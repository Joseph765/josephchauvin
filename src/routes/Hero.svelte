<script>
    import { Button, Container, Flex, Text } from "$lib/components";
	import Divider from "$lib/components/Divider.svelte";
</script>

<section id="hero">
    <Container size="xl">
        <Flex direction="column" gap="l" align="center">
            <iframe style="display: block; max-width: 1000px; width: calc(100vw - 5rem); height: auto; aspect-ratio: 16/9; padding-inline: 0rem;" src="https://www.youtube.com/embed/KvZztfj-aA4?si=mCjWf5R-va-2KVx-" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
            <Text align="center">Hello! I'm Joseph, a video game sound designer. I create immersive and satisfying sound effects that bring games to life.</Text>
            <!-- <div class="buttons">
                <Button variant="secondary" href="mailto:joseph.chauvin102@gmail.com" size="l" expanded>
                    <svg slot="start" xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-package-icon lucide-package"><path d="M11 21.73a2 2 0 0 0 2 0l7-4A2 2 0 0 0 21 16V8a2 2 0 0 0-1-1.73l-7-4a2 2 0 0 0-2 0l-7 4A2 2 0 0 0 3 8v8a2 2 0 0 0 1 1.73z"/><path d="M12 22V12"/><polyline points="3.29 7 12 12 20.71 7"/><path d="m7.5 4.27 9 5.15"/></svg>
                    SFX Packs
                </Button>
                <Button href="mailto:joseph.chauvin102@gmail.com" size="l" expanded>
                    <svg slot="start" xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-wand-icon lucide-wand"><path d="M15 4V2"/><path d="M15 16v-2"/><path d="M8 9h2"/><path d="M20 9h2"/><path d="M17.8 11.8 19 13"/><path d="M15 9h.01"/><path d="M17.8 6.2 19 5"/><path d="m3 21 9-9"/><path d="M12.2 6.2 11 5"/></svg>
                    Custom SFX
                </Button>
            </div> -->
        </Flex>
    </Container>
</section>

<style>
    section {
        display: flex;
        align-items: center;
        flex-direction: column;
        padding-block: 4rem;
        color: var(--v-color-text);
        background-color: var(--v-color-background);
        /* min-height: 100vh; */
    }

    img {
        max-width: 100%;
        margin: auto;
        border-radius: 2px;
        max-height: 600px;
    }

    .buttons {
        display: flex;
        width: 100%;
        gap: var(--v-space-m);
    }

    @media only screen and (max-width: 700px) { 
        section {
            padding-block: 4rem 2rem;
        }
    }
</style>