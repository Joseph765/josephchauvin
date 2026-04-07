<script>
    /** @type { 'default' | 'primary' | 'secondary' | 'outline' | 'ghost' | 'danger' } */
    export let variant = 'default';

    /** @type { boolean } */
    export let expanded = false;

    /** @type { 'm' | 'l' } */
    export let size = 'm';

    /** @type { boolean } */
    export let disabled = false;

    /** @type { string } */
    export let href = "";
</script>

<div class="button-wrapper {expanded ? "is-expanded" : undefined}">
    {#if href}
        <a {href} class="button-overlay is-size-{size}">
            <slot name="start" />
            <slot />
            <slot name="end" />
        </a>
    {:else}
        <div class="button-overlay is-size-{size}">
            <slot name="start" />
            <slot />
            <slot name="end" />
        </div>
    {/if}
    {#if href}
        <a {href} class="button is-link is-size-{size}" tabindex="0" {...$$restProps} on:click>
            <slot name="start" />
            <slot />
            <slot name="end" />
        </a>
    {:else}
        <button class="button is-{variant} is-size-{size}" disabled={disabled} tabindex="0" {...$$restProps} on:click>
            <slot name="start" />
            <slot />
            <slot name="end" />
        </button>
    {/if}
</div>

<style>
    .button-wrapper {
        position: relative;
        height: 32px;
        width: max-content;
        cursor: pointer;
    }

    .button-wrapper.is-expanded,
    .button-wrapper.is-expanded .button-overlay,
    .button-wrapper.is-expanded .button {
        width: 100%;
    }

    .button,
    .button-overlay {
        transition: clip-path 0.2s ease;
        padding-block: 0;
    }

    .button-overlay {
        position: absolute;
        top: 0;
        left: 0;
        clip-path: inset(0 100% 0 0);
        display: flex;
        align-items: center;
        justify-content: center;
        gap: var(--v-space-s);
        font-family: var(--v-font);
        font-size: var(--v-font-size-m);
        font-weight: var(--v-font-weight-regular);
        letter-spacing: var(--v-letter-spacing-m);
        line-height: var(--v-line-height-m);
        border: 1px solid var(--v-color-text);
        border-radius: var(--v-radius);
        background-color: var(--v-color-text);
        height: 32px;
        color: var(--v-color-text-contrast);
        cursor: pointer;
        padding-inline: var(--v-space-m);
        text-decoration: none;
    }

    .button-overlay.is-size-l {
        font-size: var(--v-font-size-l);
        height: auto;
        padding: var(--v-space-s) var(--v-space-l);
    }

    .button {
        display: flex;
        align-items: center;
        justify-content: center;
        gap: var(--v-space-s);
        font-family: var(--v-font);
        font-size: var(--v-font-size-m);
        font-weight: var(--v-font-weight-regular);
        letter-spacing: var(--v-letter-spacing-m);
        line-height: var(--v-line-height-m);
        border: 1px solid var(--v-accent-9);
        border-radius: var(--v-radius);
        background-color: var(--v-accent-5);
        height: 32px;
        width: max-content;
        color: var(--v-color-text);
        cursor: pointer;
        padding-inline: var(--v-space-m);
        text-decoration: none;
    }

    .button:focus-visible {
        outline: 2px solid var(--v-color-info);
        outline-offset: 2px;
    }

    .button.is-expanded {
        width: 100%;
    }

    .button.is-size-l {
        font-size: var(--v-font-size-l);
        height: auto;
        padding: var(--v-space-s) var(--v-space-l);
    }

    .button.is-secondary {
        background-color: var(--v-color-background);
        color: var(--v-accent-11);
        border-color: var(--v-accent-9);
    }

    .button.is-ghost {
        background-color: var(--v-color-background);
        border-color: transparent;
        color: var(--v-accent-11);
    }

    .button.is-danger {
        background-color: var(--v-color-danger);
        border-color: var(--v-color-danger);
        color: var(--v-color-text);
    }

    .button:disabled {
        background-color: var(--v-gray-4);
        border-color: var(--v-gray-3);
        color: var(--v-color-text-weaker);
        cursor: not-allowed;
    }

    .button.is-secondary:disabled {
        background-color: var(--v-gray-1);
        color: var(--v-gray-4);
        border-color: var(--v-gray-3);
        cursor: not-allowed;
    }

    .button.is-ghost:disabled {
        background-color: var(--v-color-background);
        border: none;
        color: var(--v-gray-4);
        cursor: not-allowed;
    }

    .button.is-danger:disabled {
        background-color: var(--v-danger-2);
        border-color: var(--v-danger-2);
        color: var(--v-gray-4);
        cursor: not-allowed;
    }

    @media (pointer: fine) {
        .button-wrapper:hover .button-overlay {
            clip-path: inset(0 0 0 0);
        }

        .button.is-secondary:hover {
            background-color: var(--v-accent-5);
            color: var(--v-color-text);
            border-color: var(--v-color-accent);
        }

        .button.is-secondary:disabled:hover {
            background-color: var(--v-gray-1);
            color: var(--v-gray-4);
            border-color: var(--v-gray-3);
        }

        .button.is-ghost:hover {
            background-color: var(--v-color-background);
            color: var(--v-accent-11);
            border: 1px solid var(--v-accent-9);
        }

        .button.is-ghost:disabled:hover {
            background-color: var(--v-color-background);
            border: none;
            color: var(--v-gray-4);
        }

        .button.is-danger:hover {
            background-color: var(--v-color-background);
            color: var(--v-color-danger);
            border-color: var(--v-color-danger);
        }

        .button:disabled:hover {
            background-color: var(--v-gray-4);
            color: var(--v-color-text-weaker);
            border-color: var(--v-gray-3);
        }
    }
</style>