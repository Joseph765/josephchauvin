<script>
    import { Container, Flex, Text } from "$lib/components";
</script>

<section>
    <Container>
        <Flex direction="column">
            <img alt="Joseph Chauvin in his home studio" src="/me-in-the-studio.jpg" />
            <br />
            <Text style="color: var(--gray-1);">Hi! I'm Joseph Chauvin, a music composer for 2D action games based in Asheville, North Carolina.</Text>
            <Text style="color: var(--gray-1);">I have a deep passion for crafting retro-styled action music that inspires players to overcome challenges.</Text>
        </Flex>
    </Container>
</section>
<!-- <img alt="My Studio" src="/my-studio.jpg" />
<div class="overlay"></div>
<div class="title">
    <h1>Music Composer For 2D Action Games</h1>
    <a class="button" href="mailto:joseph.chauvin102@gmail.com">Contact</a>
</div>
<div class="arrow-down">
    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-chevron-down-icon lucide-chevron-down"><path d="m6 9 6 6 6-6"/></svg>
</div> -->

<style>
    section {
        display: flex;
        align-items: center;
        flex-direction: column;
        /* height: 100vh; */
        background: var(--gray-12);
        padding-block: 4rem;
    }

    img {
        max-width: 100%;
        margin: auto;
        border-radius: 2px;
    }
    /* img {
        object-fit: cover;
        width: 100%;
        height: 100%;
        position: absolute;
        top: 0;
        left: 0;
    } */

    .overlay {
        width: 100%;
        height: 100%;
        position: absolute;
        top: 0;
        left: 0;
        background: var(--indigo-1);
        opacity: 0.85;
    }

    .title {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        width: 100%;
        overflow: hidden;
        text-align: center;
        display: flex;
        align-items: center;
        flex-direction: column;
        gap: 16px;
    }

    h1 {
        font-family: var(--font-family);
        font-size: clamp(2.5rem, 4.5vw + 1.5rem, 5rem);
        font-weight: 315;
        margin: 0;
        letter-spacing: -2.5px;
        color: var(--color-text);
        max-inline-size: 820px;
        line-height: 1.2;
        text-shadow: 3px 3px 4px var(--color-background);
    }

    .button {
        display: flex;
        align-items: center;
        justify-content: center;
        font-family: var(--font-family);
        font-size: 1.25rem;
        font-weight: 415;
        height: 3rem;
        padding-inline: 2rem;
        padding-bottom: 3px;
        border-radius: 2px;
        background: var(--color-accent);
        border: 1px solid transparent;
        color: var(--color-text);
        cursor: pointer;
        text-decoration: none;
        box-shadow: 3px 3px 4px var(--color-background);
    }

    .arrow-down {
        position: absolute;
        bottom: 1rem;
        left: 50%;
        transform: translate(-50%, -50%);
    }

    @media (pointer: fine) {
        .button:hover {
            background: var(--color-background);
            border: 1px solid var(--color-accent);
        }
    }
</style>