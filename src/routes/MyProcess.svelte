<script>
    import { Section, Heading, Button, Container, Flex, Text } from "$lib/components";
</script>

<section id="myprocess">
    <Container size="xl">
        <Flex direction="column" gap="s" style="padding-bottom: 2rem;">
            <Heading>My Process</Heading>
            <Text align="center" style="max-inline-size: 100%;">See how I create sounds for games, from recording and experimentation to the final result.</Text>
        </Flex>
        <div class="grid">
            <iframe width="100%" height="275" src="https://www.youtube.com/embed/65kUga8yTrc?si=eq-Opnam0WBNIM89" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
            <iframe width="100%" height="275" src="https://www.youtube.com/embed/_bCMnWh7UA8?si=hWIJDgtzTmqchCCO" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
            <iframe width="100%" height="275" src="https://www.youtube.com/embed/9T1SoDzWuLA?si=FkbmoEU3CWMFGIsX" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
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
        grid-template-columns: repeat(auto-fit, minmax(min(464px, 100%), 1fr));
        justify-content: center;
        gap: var(--space-xl);
        width: 100%;
    }

    iframe {
        border-radius: var(--v-radius-rounded);
    }

    @media only screen and (max-width: 700px) { 
        section {
            padding-block: 2rem;
        }
    }
</style>