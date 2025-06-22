<script>
    /** @type { 'row' | 'column' } */
    export let direction = "row";

    /** @type { 'm' | 'l' | 'xl' } */
    export let gap = "m"

    /** @type { 'start' | 'center' } */
    export let justify = "start"
</script>

<div class="flex is-direction-{direction} has-gap-{gap} is-justify-{justify}">
    <slot />
</div>

<style>
    .flex {
        display: flex;
        align-items: center;
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
</style>