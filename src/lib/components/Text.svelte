<script>
    /** @type { string } */
    export let style = "";

    /** @type { boolean } */
    export let mobileCenter = true;
</script>

<p class={mobileCenter ? "mobile-center" : ""} {style}>
    <slot />
</p>

<style>
    p {
        font-family: var(--v-font);
        color: var(--v-color-text);
        letter-spacing: 1px;
        font-size: 1.25rem;
        max-inline-size: 60ch;
        line-height: 1.65;
    }

    @media only screen and (max-width: 1307px) {
        p.mobile-center {
            text-align: center;
        }
    }
</style>