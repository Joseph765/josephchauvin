<script>
    /** @type { 'm' | 'none'} */
    export let space = "m";
</script>

<div class="divider has-space-{space}"></div>

<style>
    .divider {
        border-top: 1px solid var(--color-border);
        margin-block: 2rem;
        width: 100%;
    }

    .divider.has-space-none {
        margin: 0;
    }
</style>