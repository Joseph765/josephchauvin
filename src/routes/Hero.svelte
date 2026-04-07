<script>
    import { Container, Flex, Text } from "$lib/components";
	import Divider from "$lib/components/Divider.svelte";
</script>

<section>
    <Container>
        <Flex direction="column" gap="l" align="center">
            <img alt="Joseph Chauvin in his home studio" src="/me-in-the-studio.jpg" />
            <br />
            <Text>Hello! I'm Joseph Chauvin, a sound designer for video games based in Houston, Texas.</Text>
            <Text>I'm passionate about creating immersive audio for games. I especially love working with synthesizers and designing sci-fi sounds, futuristic ambiences, and powerful effects.</Text>
            <Text>When I'm not designing sounds or playing video games, I love spending time with my family.</Text>
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
</style>