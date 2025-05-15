<script>
    let showMenu = false;
</script>

<!-- <nav>
    <a class="logo" href="/">Joseph Chauvin</a>
    <ul class="desktop-links">
        <li>
            <a href="#music">
                Music
            </a>
        </li>
        <li>
            <a href="#about">About</a>
        </li>
        <li>
            <a href="#contact">
                Contact
            </a>
        </li>
    </ul>
    <button aria-label="Navigation menu" class="hamburger" onclick={() => showMenu = !showMenu}>
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
                    <a href="#music" onclick={() => showMenu = false}>
                        Music
                    </a>
                </li>
                <li>
                    <a href="#about" onclick={() => showMenu = false}>About</a>
                </li>
                <li>
                    <a href="#contact" onclick={() => showMenu = false}>Contact</a>
                </li>
            </ul>
        </div>
    {/if}
</nav> -->

<a class="temp-logo" href="/">Joseph Chauvin</a>

<style>
    .temp-logo {
        z-index: 9999;
        padding: 1rem;
        margin: auto;
        font-family: var(--font-family);
        font-size: 1.5rem;
        font-weight: 315;
        margin: 0;
        letter-spacing: -0.5px;
        color: var(--color-text);
        max-inline-size: 700px;
        white-space: nowrap;
        padding-inline-start: 1rem;
        text-shadow: 2px 2px 4px var(--color-background);
    }

    /* nav {
        width: 100%;
        z-index: 9999;
        display: flex;
        align-items: end;
        justify-content: space-between;
        padding: 1rem;
    }

    .hamburger {
        display: none;
        background: none;
        border: none;
        color: var(--color-text);
        padding-inline-end: 1rem;
    }

    .mobile-menu {
        background: var(--gray-4);
        border: 1px solid var(--gray-6);
        border-radius: 2px;
        position: absolute;
        top: 3rem;
        right: 1rem;
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
    } */

    a {
        font-family: var(--font-family);
        text-decoration: none;
        color: var(--color-text);
        font-size: 1rem;
    }

    @media (pointer: fine) {
        a:hover {
            text-decoration: underline;
        }
    }


    /* .desktop-links {
        display: flex;
        align-items: center;
        gap: 2rem;
    }

    .logo {
        font-family: var(--font-family);
        font-size: 1.5rem;
        font-weight: 315;
        margin: 0;
        letter-spacing: -0.5px;
        color: var(--color-text);
        max-inline-size: 700px;
        white-space: nowrap;
        padding-inline-start: 1rem;
    } */

    /* @media only screen and (max-width: 700px) {
        .desktop-links {
            display: none;
        }

        .hamburger {
            display: block;
        }
    } */
</style>