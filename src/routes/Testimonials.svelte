<script>
    import { Section, Heading, Button, Container, Flex, Text } from "$lib/components";
</script>

<section id="testimonials">
    <Flex direction="column" gap="s" style="padding-bottom: 2rem;">
        <Heading>Testimonials</Heading>
        <!-- <Text>Need sounds made specifically for your game? I create custom SFX tailored to your game's style and needs.</Text> -->
    </Flex>
    <Container size="xl">
        <Flex wraps gap="l" justify="center">
            <div class="card">
                <Flex direction="column" gap="m" align="center">
                    <Text size="s">"Joseph was great to work with. He understood exactly what we were looking for and brought the sounds to life." </Text>
                    <Text align="end">— Developer Name, Game Name</Text>
                </Flex>
            </div>
            <div class="card">
                <Flex direction="column" gap="m" align="center">
                    <Text>"Joseph was great to work with. He understood exactly what we were looking for and brought the sounds to life." </Text>
                    <Text align="end">— Developer Name, Game Name</Text>
                </Flex>
            </div>
            <div class="card">
                <Flex direction="column" gap="m" align="center">
                    <Text>"Joseph was great to work with. He understood exactly what we were looking for and brought the sounds to life." </Text>
                    <Text align="end">— Developer Name, Game Name</Text>
                </Flex>
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
        scroll-margin-top: var(--header-height);
    }

    .card {
        box-shadow: 1px 1px 0 1px var(--v-gray-2);
        border: 1px solid var(--v-gray-8);
        border-radius: var(--v-radius-rounded);
        padding: var(--v-space-xl);
        max-width: 585px;
    }

    @media only screen and (max-width: 700px) { 
        section {
            padding-block: 2rem;
        }
    }
</style>