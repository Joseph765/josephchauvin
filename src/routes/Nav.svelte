<nav>
    <ul>
        <li>
            <a class="logo" href="/">Joseph Chauvin</a>
        </li>
        <div class="links">
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
        </div>
    </ul>
</nav>

<style>
    nav {
        /* position: sticky;
        top: 0;
        left: 0; */
        width: 100%;
        z-index: 9999;
        /* background: var(--gray-5); */
        /* border-bottom: 1px solid var(--gray-6); */
    }

    ul {
        display: flex;
        align-items: center;
        justify-content: space-between;
        list-style-type: none;
        padding-inline: 2rem;
    }

    a {
        font-family: "Roboto Slab", sans-serif;
        text-decoration: none;
        color: var(--gray-12);
        font-size: 1rem;
    }

    a:hover {
        text-decoration: underline;
    }

    .links {
        display: flex;
        align-items: center;
        gap: 2rem;
    }

    .logo {
        font-family: "Roboto Slab", sans-serif;
        font-size: 1.5rem;
        font-weight: 315;
        margin: 0;
        letter-spacing: -0.5px;
        color: var(--gray-12);
        max-inline-size: 700px;
    }
</style>