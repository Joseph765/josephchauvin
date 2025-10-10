<script>
    /** @type { 'm' | 'l' } */
    export let size;
</script>

<div class="container is-size-{size}">
    <slot />
</div>

<style>
    .container {
        max-inline-size: 900px;
        margin: auto;
        padding-inline: 2rem;
        /* width: 100%; */
    }

    .container.is-size-l {
        max-inline-size: 1200px;
    }
</style>