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
        font-family: var(--font-family);
        color: var(--color-text-weak);
        font-weight: 350;
        letter-spacing: 1px;
        font-size: 1.25rem;
        max-inline-size: 67ch;
        line-height: 1.65;
    }

    @media only screen and (max-width: 1307px) {
        p.mobile-center {
            text-align: center;
        }
    }
</style>