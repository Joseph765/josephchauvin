<script>
    /** @type { 's' | 'm' }*/
    export let size = "m";

    /** @type { 'start' | 'center' }*/
    export let align = "center";

    /** @type { string } */
    export let style = "";
</script>

{#if size === "m"}
    <h3 {style} class="is-align-{align}">
        <slot />
    </h3>
{:else if size === "s"}
    <h4 {style} class="is-align-{align}">
        <slot />
    </h4>
{/if}

<style>
    h3, 
    h4 {
        font-family: var(--font-family);
        color: var(--color-text-weak);
        font-weight: 350;
        letter-spacing: 1px;
        text-transform: uppercase; 
        text-align: center;
    }

    h3 {
        font-size: 2rem;
    }

    h4 {
        font-size: 1.25rem;
    }

    .is-align-start {
        text-align: start;
    }
</style>