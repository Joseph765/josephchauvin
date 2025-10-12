<script>
    import { Container, Flex, Text } from "$lib/components";
	import Divider from "$lib/components/Divider.svelte";
</script>

<section>
    <Container>
        <Flex direction="column" gap="l" align="center">
            <img alt="Joseph Chauvin in his home studio" src="/me-in-the-studio.jpg" />
            <br />
            <Text>Hi! I'm Joseph Chauvin, a music composer for 2D action video games based in Asheville, North Carolina.</Text>
            <Text>I have a deep passion for crafting atmospheric, evocative music for metroidvania games that immerses players in captivating and challenging worlds.</Text>
            <Text>When I'm not writing music or playing video games, I enjoy spending time whitewater kayaking with my friends in the Appalachian mountains.</Text>
        </Flex>
    </Container>
</section>
<!-- <Divider /> -->

<style>
    section {
        display: flex;
        align-items: center;
        flex-direction: column;
        padding-block: 4rem;
        color: var(--color-text);
    }

    img {
        max-width: 100%;
        margin: auto;
        border-radius: 2px;
        max-height: 600px;
    }
</style>