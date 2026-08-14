<script>
    import { Section, Heading, Button, Container, Flex, Text, Divider } from "$lib/components";

    let showStudioPhoto = true;
</script>

<section id="about">
    <Heading style="padding-bottom: 2rem;">About</Heading>
    <Container>
        <Flex direction="column" gap="l" align="center">
            <img alt="Joseph Chauvin in his home studio" src="/me-in-the-studio-2.jpg" />
            <Text align="center">
                I'm Joseph Chauvin, a video game sound designer based in Houston, Texas. I've always been drawn to video games and the worlds they create. The sounds of those worlds have always been a huge part of what made them feel real and memorable to me.
            </Text>
            <Text align="center">
                That's what I love about sound design. Games can transport us somewhere completely new, and every detail, from a character's footsteps to the sound of an entire environment, helps tell that story. Being able to contribute to that experience through sound is something I find incredibly meaningful.
            </Text>
            <Text align="center">
                When I'm not designing sounds or playing video games, I enjoy spending time with my family.
            </Text>
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
        /* max-height: 600px; */
    }

    @media only screen and (max-width: 700px) { 
        section {
            padding-block: 2rem;
        }
    }
</style>