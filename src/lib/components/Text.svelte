<script>
    /** @type { string } */
    export let style = "";
</script>

<p {style}>
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
        p {
            text-align: center;
        }
    }
</style>