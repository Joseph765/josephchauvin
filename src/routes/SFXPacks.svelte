<script>
    import { Section, Heading, Button, Container, Flex, Text } from "$lib/components";
</script>

<section id="sfxpacks">
    <Container size="xl">
        <Flex direction="column" justify="center" style="padding-bottom: 2rem;">
            <Heading>SFX Packs</Heading>
            <Text style="max-inline-size: 100%;" align="center">A collection of ready-to-use sound effects for your game.</Text>
        </Flex>
        <div class="grid">
            <Flex direction="column" gap="m" align="center">
                <a href="https://josephchauvin.itch.io/retro-action-music-pack">
                    <img alt="Sci-Fi UI Sound Pack" src="/Mockup.jpg" />
                </a>
                <Flex direction="column" gap="xs" align="center">
                    <Text align="center">Sci-Fi UI</Text>
                    <Text align="center">$12.99 USD</Text>
                </Flex>
            </Flex>
            <div class="coming-soon">Coming Soon</div>
            <div class="coming-soon">Coming Soon</div>
            <div class="coming-soon">Coming Soon</div>
        </div>
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

    .grid {
        display: grid;
        grid-template-columns: repeat(auto-fit, 281px);
        gap: var(--space-xl);
        width: 100%;
        justify-content: center;
    }

    img,
    .coming-soon {
        height: 281px;
        min-width: 281px;
        border-radius: var(--v-radius-rounded);
    }

    img {
        max-height: 332px;
        height: 281px;
    }

    .coming-soon {
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: var(--v-font-size-l);
        font-family: var(--v-font);
        letter-spacing: var(--v-letter-spacing-l);
        line-height: var(--v-line-height-l);
        background-color: var(--v-color-surface);
        -webkit-user-select: none; /* Safari */
        -ms-user-select: none; /* IE 10 and Edge */
        user-select: none; /* Standard syntax */
    }

    @media (pointer: fine) { 
        a:hover {
            border-radius: var(--v-radius-rounded);
            box-shadow: 0 0 6px 4px var(--v-color-text);
        }
    }

    @media only screen and (max-width: 700px) { 
        section {
            padding-block: 2rem;
        }
    }
</style>