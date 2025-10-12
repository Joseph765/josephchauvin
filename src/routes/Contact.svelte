<script>
    import { Section, Heading, Flex, Container } from "$lib/components";
	import Text from "$lib/components/Text.svelte";

    let showStudioPhoto = true;
</script>

<section id="contact">
    <Container>
        <Heading style="padding-bottom: 2rem;">Custom Music</Heading>
        <Flex direction="column" gap="l">
            <div>
                <Text mobileCenter={false}>Interested in custom music for your project?</Text>
                <br />
                <Text mobileCenter={false}>Contact me with details about:</Text>
                <Text mobileCenter={false}>
                    <ul>
                        <li>Your game's musical influences</li>
                        <li>Project deadline</li>
                        <li>Specific track types (e.g., ambient, cinematic, battle)</li>
                        <li>Total minutes of music required</li>
                    </ul>
                </Text>
                <Text mobileCenter={false}>Pricing is based on a per-minute rate for finished music.</Text>
            </div>
            <a href="mailto:joseph.chauvin102@gmail.com" onclick={() => showMenu = false}>Contact</a>
        </Flex>
    </Container>
</section>


<style>
    section {
        display: flex;
        align-items: center;
        flex-direction: column;
        /* height: 100vh; */
        /* background: var(--gray-12); */
        padding-block: 4rem;
    }

    .container {
        max-inline-size: 900px;
        margin: auto;
        padding-inline: 2rem;
    }

    a {
        padding: 0.5rem 1rem;
        border-radius: 2px;
        background: var(--color-accent);
        border: none;
        display: flex;
        justify-content: center;
        align-items: center;
        cursor: pointer;
        font-size: 1rem;
        font-family: var(--font-family);
        color: var(--color-text-contrast);
        text-decoration: none;
    }

    @media (pointer: fine) {
        a:hover {
            background: var(--color-text);
            color: var(--color-text-contrast);
            text-decoration: underline;
        }
    }
</style>