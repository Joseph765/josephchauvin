<script>
    import { Section, Heading, Flex } from "$lib/components";
	import Text from "$lib/components/Text.svelte";

    let showStudioPhoto = true;
</script>

<section id="contact">
    <div class="container">
        <Heading style="padding-bottom: 2rem; color: var(--gray-1);">Custom Music</Heading>
        <Flex direction="column" gap="l">
            <div>
                <Text style="color: var(--gray-1);">Interested in custom music for your project?</Text>
                <br />
                <Text style="color: var(--gray-1);">Contact me with details about:</Text>
                <Text style="color: var(--gray-1);">
                    <ul>
                        <li>Your game's musical influences</li>
                        <li>Project deadline</li>
                        <li>Specific track types (e.g., ambient, cinematic, battle)</li>
                        <li>Total minutes of music required</li>
                    </ul>
                </Text>
                <Text style="color: var(--gray-1);">Pricing is based on a per-minute rate for finished music.</Text>
            </div>
            <a href="mailto:joseph.chauvin102@gmail.com" onclick={() => showMenu = false}>Contact</a>
        </Flex>
    </div>
</section>


<style>
    section {
        display: flex;
        align-items: center;
        flex-direction: column;
        /* height: 100vh; */
        background: var(--gray-12);
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
        width: 100%;
        font-family: var(--font-family);
        color: var(--color-text);
        text-decoration: none;
    }

    @media (pointer: fine) {
        a:hover {
            background: var(--gray-1);
            color: var(--gray-12);
            text-decoration: underline;
        }
    }
</style>