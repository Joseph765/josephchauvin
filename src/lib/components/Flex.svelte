<script>
    /** @type { 'row' | 'column' } */
    export let direction = "row";

    /** @type { 'm' | 'l' } */
    export let gap = "m"
</script>

<div class="flex is-direction-{direction}">
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
</style>