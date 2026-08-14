<script>
    import { Section, Heading, Button, Container, Flex, Text } from "$lib/components";
</script>

<section id="sfxpacks">
    <Container size="xl">
        <Flex direction="column" justify="center" style="padding-bottom: 2rem;">
            <Heading>SFX Packs</Heading>
            <Text style="max-inline-size: 100%;" align="center">A collection of ready-to-use sound effects for your game.</Text>
        </Flex>
        <Flex wraps gap="xl" justify="center">
            <Flex direction="column" gap="m" align="center">
                <a href="https://josephchauvin.itch.io/retro-action-music-pack">
                    <img alt="Retro Action Music Pack" src="/retroactionmusicpack.png" />
                </a>
                <Flex direction="column" gap="xs" align="center">
                    <Text align="center">Retro Action Music Pack</Text>
                    <Text align="center">$9.99 USD</Text>
                </Flex>
            </Flex>
            <Flex direction="column" gap="m" align="center">
                <a href="https://josephchauvin.itch.io/retro-action-music-pack">
                    <img alt="Retro Action Music Pack" src="/retroactionmusicpack.png" />
                </a>
                <Flex direction="column" gap="xs" align="center">
                    <Text align="center">Retro Action Music Pack</Text>
                    <Text align="center">$9.99 USD</Text>
                </Flex>
            </Flex>
            <Flex direction="column" gap="m" align="center">
                <a href="https://josephchauvin.itch.io/retro-action-music-pack">
                    <img alt="Retro Action Music Pack" src="/retroactionmusicpack.png" />
                </a>
                <Flex direction="column" gap="xs" align="center">
                    <Text align="center">Retro Action Music Pack</Text>
                    <Text align="center">$9.99 USD</Text>
                </Flex>
            </Flex>
            <Flex direction="column" gap="m" align="center">
                <a href="https://josephchauvin.itch.io/retro-action-music-pack">
                    <img alt="Retro Action Music Pack" src="/retroactionmusicpack.png" />
                </a>
                <Flex direction="column" gap="xs" align="center">
                    <Text align="center">Retro Action Music Pack</Text>
                    <Text align="center">$9.99 USD</Text>
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
        scroll-margin-top: var(--header-height);
    }

    img {
        max-width: 100%;
        margin: auto;
        border-radius: 2px;
        max-height: 332px;
        border-radius: var(--v-radius-rounded);
    }

    @media (pointer: fine) { 
        a:hover {
            border-radius: var(--v-radius-rounded);
            box-shadow: 0 0 6px 4px var(--v-color-text);
        }
    }
</style>