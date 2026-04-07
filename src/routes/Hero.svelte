<script>
    import { Button, Container, Flex, Text } from "$lib/components";
	import Divider from "$lib/components/Divider.svelte";
</script>

<section>
    <Container>
        <Flex direction="column" gap="l" align="center">
            <img alt="Joseph Chauvin in his home studio" src="/me-in-the-studio-2.jpg" />
            <Text>Hello! I'm Joseph Chauvin, a sound designer for video games based in Houston, Texas.</Text>
            <Text>I'm passionate about creating immersive audio for games. I especially love working with synthesizers and designing sci-fi sounds, futuristic ambiences, and powerful effects.</Text>
            <Text>When I'm not designing sounds or playing video games, I love spending time with my family.</Text>
            <div class="mobile-button">
                <Button href="mailto:joseph.chauvin102@gmail.com" size="l" expanded>
                    <svg slot="start" xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-mail-icon lucide-mail"><path d="m22 7-8.991 5.727a2 2 0 0 1-2.009 0L2 7"/><rect x="2" y="4" width="20" height="16" rx="2"/></svg>
                    Contact
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
    }

    img {
        max-width: 100%;
        margin: auto;
        border-radius: 2px;
        max-height: 600px;
    }

    .mobile-button {
        display: none;
        width: 100%;
    }

    @media only screen and (max-width: 700px) {
        .mobile-button {
            display: block;
        }
    }
</style>