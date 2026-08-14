<script>
    import { Section, Heading, Button, Container, Flex, Text } from "$lib/components";
</script>

<section id="sfxpacks">
    <Flex direction="column" style="padding-bottom: 2rem;">
        <Heading>SFX Packs</Heading>
        <Text>A collection of ready-to-use sound effects for your game.</Text>
    </Flex>
    <Container size="xl">
        <Flex wraps gap="xl" justify="center">
            <Flex direction="column" gap="m" align="center">
                <a href="https://josephchauvin.itch.io/retro-action-music-pack">
                    <img alt="Retro Action Music Pack" src="/retroactionmusicpack.png" />
                </a>
                <Flex direction="column" gap="xs" align="center">
                    <Text size="xl">Retro Action Music Pack</Text>
                    <Text size="xl">$9.99 USD</Text>
                </Flex>
            </Flex>
            <Flex direction="column" gap="m" align="center">
                <a href="https://josephchauvin.itch.io/retro-action-music-pack">
                    <img alt="Retro Action Music Pack" src="/retroactionmusicpack.png" />
                </a>
                <Flex direction="column" gap="xs" align="center">
                    <Text size="xl">Retro Action Music Pack</Text>
                    <Text size="xl">$9.99 USD</Text>
                </Flex>
            </Flex>
            <Flex direction="column" gap="m" align="center">
                <a href="https://josephchauvin.itch.io/retro-action-music-pack">
                    <img alt="Retro Action Music Pack" src="/retroactionmusicpack.png" />
                </a>
                <Flex direction="column" gap="xs" align="center">
                    <Text size="xl">Retro Action Music Pack</Text>
                    <Text size="xl">$9.99 USD</Text>
                </Flex>
            </Flex>
            <Flex direction="column" gap="m" align="center">
                <a href="https://josephchauvin.itch.io/retro-action-music-pack">
                    <img alt="Retro Action Music Pack" src="/retroactionmusicpack.png" />
                </a>
                <Flex direction="column" gap="xs" align="center">
                    <Text size="xl">Retro Action Music Pack</Text>
                    <Text size="xl">$9.99 USD</Text>
                </Flex>
            </Flex>
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
        max-height: 332px;
    }

    @media (pointer: fine) { 
        a:hover {
            box-shadow: 0 0 6px 4px var(--v-color-text);
        }
    }
</style>