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
        font-family: var(--v-font);
        font-weight: var(--v-font-weight-bold);
        color: var(--v-color-text);
        letter-spacing: 1px;
        text-align: center;
    }

    h3 {
        font-size: var(--v-font-size-3xl);
        letter-spacing: var(--v-letter-spacing-3xl);
    }

    h4 {
        font-size: var(--v-font-size-xl);
    }

    .is-align-start {
        text-align: start;
    }
</style>