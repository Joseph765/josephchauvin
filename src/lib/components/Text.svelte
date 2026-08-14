<script>
    /** @type { string } */
    export let style = "";

    /** @type { 'start' | 'center' | 'end' }*/
    export let align = "start";

    /** @type { 'default' | 'weak' } */
    export let variant = "default";

    // /** @type { 's' | 'm' | 'l' } */
    // export let size = "m";

    /** @type { boolean } */
    export let mobileCenter = true;
</script>

<p class="is-align-{align} is-{variant} {mobileCenter ? "mobile-center" : ""}" {style}>
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

    p.is-align-center {
        text-align: center;
    }

    p.is-align-start {
        text-align: start;
    }

    p.is-align-end {
        text-align: end;
    }

    p.is-weak {
        color: var(--v-color-text-weak);
    }

    @media only screen and (max-width: 1307px) {
        p.mobile-center {
            text-align: center;
        }
    }
</style>