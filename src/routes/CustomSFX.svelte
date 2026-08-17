<script>
    import { Section, Heading, Button, Container, Flex, Text } from "$lib/components";
</script>

<section id="customsfx">
    <Container>
        <Flex direction="column" gap="" style="padding-bottom: 2rem;">
            <Heading>Custom SFX</Heading>
            <Text>Need sounds made specifically for your game? I create custom SFX tailored to your game's style and needs.</Text>
            <div class="banner">
                $20 Per SFX
                <!-- <Text align="center" style="max-inline-size: 100%;">$20 Per SFX</Text> -->
            </div>
        </Flex>
        <Flex gap="m" direction="column">
            <Heading size="s" align="start">How It Works</Heading>
            <ul>
                <li>
                    <Text align="start">Email me at <a href="mailto:joseph.chauvin102@gmail.com">joseph.chauvin102@gmail.com.</a></Text>
                </li>
                <li>
                    <Text align="start">Send me your game, references, and a description of the sounds you're looking for.</Text>
                </li>
                <li>
                    <Text>I'll create an initial draft and work with you through feedback and revisions.</Text>
                </li>
                <li>
                    <Text>Once everything sounds right, I'll deliver the final SFX ready for your game.</Text>
                </li>
            </ul>
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

    .banner {
        padding: var(--v-space-m);
        /* border: 1px solid var(--v-accent-1); */
        border-radius: var(--v-radius-rounded);
        background-color: var(--v-gray-2);
        text-align: center;
        font-family: var(--v-font);
        font-size: var(--v-font-size-xl);
        font-weight: var(--v-font-weight-regular);
        letter-spacing: var(--v-letter-spacing-xl);
    }

    ul {
        margin: 0;
    }

    a {
        font-family: var(--v-font);
        color: var(--v-color-text);
    }

    @media only screen and (max-width: 700px) { 
        section {
            padding-block: 2rem;
        }
    }
</style>