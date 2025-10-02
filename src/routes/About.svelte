<script>
    import { Section, Heading } from "$lib/components";
	import Text from "$lib/components/Text.svelte";

    let showStudioPhoto = true;
</script>

<section id="about">
    <div class="container is-size-l">
        <Heading style="padding-bottom: 2rem; color: var(--gray-1);">About</Heading>
        <div class="split">
            <div class="img-wrapper">
                <img alt="Joseph Chauvin in his home studio" src="/me-in-the-studio.jpg" style={showStudioPhoto ? "display: block" : "display: none;"} />
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
                <Text style="color: var(--gray-1);">I have a deep passion for crafting atmospheric, evocative music for metroidvania games that immerses players in captivating and challenging worlds.</Text>
                <br />
                <Text style="color: var(--gray-1);">When I'm not writing music or playing video games, I enjoy spending time whitewater kayaking with my friends in the Appalachian mountains.</Text>
            </div>
        </div>
    </div>
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
    
    img {
        height: 338px;
        max-width: 100%;
        margin: auto;
        border-radius: 2px;
    }

    .container {
        max-inline-size: 900px;
        margin: auto;
        padding-inline: 2rem;
    }

    .container.is-size-l {
        max-inline-size: 1250px;
    }

    .split {
        display: flex;
        flex-wrap: wrap;
        gap: 2rem;
        align-items: start;
        /* justify-content: center; */
    }

    .button-group {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding-block-start: 1rem;
    }

    button {
        /* background: var(--gray-4); */
        border: none;
        border-radius: 3px;
        display: flex;
        justify-content: center;
        align-items: center;
        cursor: pointer;
        height: 32px;
    }

    @media only screen and (max-width: 1307px) {
        .img-wrapper {
            width: 100%;
        }

        img {
            height: auto;
            width: 100%;
            max-width: 700px;
        }

        .button-group {
            max-width: 700px;
            margin: auto;
        }

        .split {
            flex-direction: column;
            gap: none;
            justify-content: center;
        }

        .text-content {
            margin: auto;
        }

    }

    @media (pointer: fine) {
        button:hover {
            background: var(--gray-5)
        }
    }
</style>