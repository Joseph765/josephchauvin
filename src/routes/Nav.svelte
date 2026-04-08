<script>
    import Button from "$lib/components/Button.svelte";
    let showMenu = false;
</script>

<nav>
    <a class="logo" href="/">Joseph Chauvin</a>
    <ul class="desktop-links">
        <li>
            <Button href="mailto:joseph.chauvin102@gmail.com" size="l">
                <svg slot="start" xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-mail-icon lucide-mail"><path d="m22 7-8.991 5.727a2 2 0 0 1-2.009 0L2 7"/><rect x="2" y="4" width="20" height="16" rx="2"/></svg>
                Contact
            </Button>
        </li>
    </ul>
    <!-- <button aria-label="Navigation menu" class="hamburger" onclick={() => showMenu = !showMenu}>
        {#if showMenu}
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-x-icon lucide-x"><path d="M18 6 6 18"/><path d="m6 6 12 12"/></svg>
        {:else}
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-menu-icon lucide-menu"><path d="M4 12h16"/><path d="M4 18h16"/><path d="M4 6h16"/></svg>
        {/if}
    </button>
    {#if showMenu}
        <div class="mobile-menu">
            <ul class="mobile-links">
                <li>
                    <a href="#demoreel" onclick={() => showMenu = false}>
                        Demo Reel
                    </a>
                </li>
                <li>
                    <a href="mailto:joseph.chauvin102@gmail.com" onclick={() => showMenu = false}>Contact</a>
                </li>
            </ul>
        </div>
    {/if} -->
</nav>

<style>
    nav {
        position: fixed;
        background: var(--v-gray-2);
        border-bottom: 1px solid var(--v-gray-3);
        top: 0;
        width: 100%;
        z-index: 9999;
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 1.5rem;
    }

    .hamburger {
        touch-action: manipulation;
        display: none;
        background: none;
        border: none;
        color: var(--v-color-text);
        padding-inline-end: 1rem;
    }

    .mobile-menu {
        touch-action: manipulation;
        background: var(--v-gray-4);
        border: 1px solid var(--v-gray-6);
        border-radius: 2px;
        position: absolute;
        top: var(--header-height);
        right: 0;
        padding: 2rem 1rem;
        width: 10rem;
    }

    .mobile-links {
        display: flex;
        gap: 1.25rem;
        flex-direction: column;
        padding: 0;
        margin: 0;
    }

    ul {
        display: flex;
        align-items: center;
        justify-content: space-between;
        list-style-type: none;
    }

    a {
        font-family: var(--v-font);
        text-decoration: none;
        color: var(--v-color-text);
        font-size: 1rem;
    }

    @media (pointer: fine) {
        a:hover {
            text-decoration: underline;
        }

        .contact:hover {
            background: var(--v-color-background);
            color: var(--v-color-text);
        }
    }


    .desktop-links {
        display: flex;
        align-items: center;
        gap: 2rem;
        margin: 0;
        padding: 0;
        /* padding-inline-end: 3rem; */
    }

    .logo {
        font-family: var(--v-font);
        font-weight: var(--v-font-weight-black);
        font-size: var(--v-font-size-3xl);
        line-height: 1;
        letter-spacing: var(--v-letter-spacing-3xl);
        /* padding: 0 var(--v-space-m) var(--v-space-m) var(--v-space-m); */
    }

    @media only screen and (max-width: 700px) {
        .desktop-links {
            display: none;
        }

        nav {
            padding: 1rem 0;
        }

        .logo {
            padding-inline-start: 1rem;
        }

        .hamburger {
            display: block;
        }
    }
</style>