<script>
    /** @type { string } */
    export let style = "";

    /** @type { 'start' | 'center' } */
    export let align = "start";

    /** @type { string } */
    export let href;
</script>

<a {href} {style} class="is-align-{align}">
    <slot />
</a>

<style>
    a {
        font-family: var(--v-font);
        font-size: 1.25rem;
        color: var(--v-color-text-link);
        letter-spacing: 1px;
    }

    .is-align-center {
        text-align: center;
    }

    @media (pointer: fine) {
        a:hover {
            text-decoration: underline;
            color: var(--indigo-8);
        }
    }
</style>