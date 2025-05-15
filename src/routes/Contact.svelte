<script>
    import { Divider, Section } from "$lib/components";
</script>

<Divider />
<Section id="contact">
    <div class="container">
        <h3>Contact</h3>
        <a href="mailto:joseph.chauvin102@gmail.com">Joseph.chauvin102@gmail.com</a>
    </div>
</Section>

<style>
    h3 {
        font-family: var(--font-family);
        font-size: 2rem;
        font-weight: 350;
        color: #d5d6d8;
        letter-spacing: 1px;
        text-transform: uppercase; 
        text-align: center;
        padding-bottom: 1rem;
    }

    .container {
        max-inline-size: 900px;
        margin: auto;
        padding-inline: 2rem;
    }

    a {
        font-family: var(--font-family);
        font-size: 1rem;
        font-weight: 350;
        /* color: #d5d6d8; */
        color: var(--indigo-11);
        letter-spacing: 1px;
        text-align: center;
        padding-bottom: 1rem;
        /* text-decoration: none; */
    }

    @media (pointer: fine) {
        a:hover {
            text-decoration: underline;
        }
    }

</style>