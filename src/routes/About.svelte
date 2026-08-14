<script>
    import { Section, Heading, Button, Container, Flex, Text, Divider } from "$lib/components";

    let showStudioPhoto = true;
</script>

<!-- <section id="about">
    <div class="container is-size-l">
        <Heading style="padding-bottom: 2rem; color: var(--v-gray-1);">About</Heading>
        <div class="split">
            <div class="img-wrapper">
                <img alt="Joseph Chauvin in his home studio" src="/me-in-the-studio-2.jpg" style={showStudioPhoto ? "display: block" : "display: none;"} />
                <img alt="Joseph Chauvin whitewater kayaking" src="/me-whitewater-kayaking.jpg" style={showStudioPhoto ? "display: none" : "display: block;"} />
                <div class="button-group">
                    <button aria-label="Previous Photo" onclick={() => showStudioPhoto = !showStudioPhoto}>
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-chevron-left-icon lucide-chevron-left"><path d="m15 18-6-6 6-6"/></svg>
                    </button>
                    <button aria-label="Next Photo" onclick={() => showStudioPhoto = !showStudioPhoto}>
                        <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-chevron-right-icon lucide-chevron-right"><path d="m9 18 6-6-6-6"/></svg>
                    </button>
                </div>
            </div>
            <div class="text-content">
                <br />
                <Text style="color: var(--v-gray-1);">I have a deep passion for crafting atmospheric, evocative music for metroidvania games that immerses players in captivating and challenging worlds.</Text>
                <br />
                <Text style="color: var(--v-gray-1);">When I'm not writing music or playing video games, I enjoy spending time whitewater kayaking with my friends in the Appalachian mountains.</Text>
            </div>
        </div>
    </div>
</section> -->

<section>
    <Heading style="padding-bottom: 2rem;">About</Heading>
    <Container>
        <Flex direction="column" gap="l" align="center">
            <img alt="Joseph Chauvin in his home studio" src="/me-in-the-studio-2.jpg" />
            <Text>Hello! I'm Joseph, a video game sound designer. I create immersive and satisfying sound effects that bring games to life.</Text>
            <!-- <div class="buttons">
                <Button variant="secondary" href="mailto:joseph.chauvin102@gmail.com" size="l" expanded>
                    <svg slot="start" xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-mail-icon lucide-mail"><path d="m22 7-8.991 5.727a2 2 0 0 1-2.009 0L2 7"/><rect x="2" y="4" width="20" height="16" rx="2"/></svg>
                    SFX Packs
                </Button>
                <Button href="mailto:joseph.chauvin102@gmail.com" size="l" expanded>
                    <svg slot="start" xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-mail-icon lucide-mail"><path d="m22 7-8.991 5.727a2 2 0 0 1-2.009 0L2 7"/><rect x="2" y="4" width="20" height="16" rx="2"/></svg>
                    Custom SFX
                </Button>
            </div> -->
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
        max-height: 600px;
    }

    .buttons {
        display: flex;
        width: 100%;
        gap: var(--v-space-m);
    }
</style>