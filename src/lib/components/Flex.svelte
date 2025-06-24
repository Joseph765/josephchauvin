<script>
    /** @type { string } */
    export let style = "";

    /** @type { 'row' | 'column' } */
    export let direction = "row";

    /** @type { 'm' | 'l' | 'xl' } */
    export let gap = "m"

    /** @type { 'start' | 'center' } */
    export let justify = "start";

    /** @type { 'start' | 'center' } */
    export let align = "start"
</script>

<div style={style} class="flex is-direction-{direction} has-gap-{gap} is-justify-{justify} is-align-{align}">
    <slot />
</div>

<style>
    .flex {
        display: flex;
        gap: var(--space-m);
    }

    .flex.is-direction-column {
        flex-direction: column;
    }

    .flex.has-gap-l {
        gap: var(--space-l);
    }

    .flex.has-gap-xl {
        gap: var(--space-xl);
    }

    .flex.is-justify-center {
        justify-content: center;
    }

    .flex.is-align-center {
        align-items: center;
    }
</style>