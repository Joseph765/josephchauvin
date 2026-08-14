<script>
    import { Button, Container, Flex, Text } from "$lib/components";
	import Divider from "$lib/components/Divider.svelte";
</script>

<section id="hero">
    <Container size="xl">
        <Flex direction="column" gap="l" align="center">
            <!-- <img alt="Joseph Chauvin in his home studio" src="/me-in-the-studio-2.jpg" /> -->
            <iframe style="display: block; max-width: 1000px; width: calc(100vw - 5rem); height: auto; aspect-ratio: 16/9; padding-inline: 0rem;" src="https://www.youtube.com/embed/KvZztfj-aA4?si=mCjWf5R-va-2KVx-" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
            <Text>Hello! I'm Joseph, a video game sound designer. I create immersive and satisfying sound effects that bring games to life.</Text>
            <!-- <Text>I'm passionate about creating immersive audio for games. I especially love working with synthesizers and designing sci-fi sounds, futuristic ambiences, and powerful effects.</Text>
            <Text>When I'm not designing sounds or playing video games, I love spending time with my family.</Text> -->
            <div class="buttons">
                <Button variant="secondary" href="mailto:joseph.chauvin102@gmail.com" size="l" expanded>
                    <svg slot="start" xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-mail-icon lucide-mail"><path d="m22 7-8.991 5.727a2 2 0 0 1-2.009 0L2 7"/><rect x="2" y="4" width="20" height="16" rx="2"/></svg>
                    SFX Packs
                </Button>
                <Button href="mailto:joseph.chauvin102@gmail.com" size="l" expanded>
                    <svg slot="start" xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-mail-icon lucide-mail"><path d="m22 7-8.991 5.727a2 2 0 0 1-2.009 0L2 7"/><rect x="2" y="4" width="20" height="16" rx="2"/></svg>
                    Custom SFX
                </Button>
            </div>
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
</style>