<script>
    import { Divider, Section } from "$lib/components";
</script>

<Divider />
<Section id="about">
    <div class="container is-size-l">
        <h3>About</h3>
        <div class="split">
            <img alt="Joseph Chauvin next to a creek" src="/Creek.jpg" />
            <div class="text-content">
                <p>Hi! I'm Joseph Chauvin, a music composer for 2D action games based in Asheville, North Carolina.</p>
                <br />
                <p>I have a deep passion for crafting retro-styled action music that empowers players to overcome any challenge.</p>
                <br />
                <p>When I'm not writing music or playing video games, I enjoy spending time whitewater kayaking with my friends in the Appalachian mountains.</p>
            </div>
        </div>
    </div>
</Section>


<style>
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
        max-inline-size: 1100px;
    }

    .split {
        display: flex;
        flex-wrap: wrap;
        gap: 2rem;
        align-items: start;
        /* justify-content: center; */
    }

    h3 {
        font-family: var(--font-family);
        font-size: 2rem;
        font-weight: 350;
        color: #d5d6d8;
        letter-spacing: 1px;
        text-transform: uppercase; 
        text-align: center;
        padding-bottom: 2rem;
    }

    p {
        font-family: var(--font-family);
        font-size: 1rem;
        font-weight: 350;
        color: #d5d6d8;
        letter-spacing: 1px;
        max-inline-size: 67ch;
        line-height: 1.65;
        /* text-align: center; */
    }

    @media only screen and (max-width: 1154px) {
        img {
            height: auto;
            width: 100%;
            max-width: 700px;
        }

        .split {
            flex-direction: column;
            gap: none;
            justify-content: center;
        }

        .text-content {
            margin: auto;
        }

        p {
            text-align: center;
        }
    }
</style>