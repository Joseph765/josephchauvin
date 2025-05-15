<script>
    /** @type { string } */
    export let id;
</script>

<section {id}>
    <slot />
</section>


<style>
    section {
        padding-block: 6rem;
        background-color: var(--color-background);
    }

    @media only screen and (max-width: 1154px) {
        section {
            padding-block: 3rem;
        }
    }
</style>