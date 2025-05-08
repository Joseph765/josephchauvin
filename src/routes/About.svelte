<section id="about">
    <div class="container is-size-l">
        <h3>About</h3>
        <div class="split">
            <img alt="Joseph Chauvin next to a creek" src="/Creek.jpg" />
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
        </div>
    </div>
</section>


<style>
    section {
        padding-block: 6rem;
        background-color: var(--gray-1);
    }

    img {
        /* height: 338px; */
        max-width: 100%;
        margin: auto;
        border-radius: 2px;
    }

    .container {
        max-inline-size: 900px;
        margin: auto;
        padding-inline: 2rem;
    }

    .container.is-size-l {
        max-inline-size: 1100px;
    }

    .split {
        display: flex;
        flex-wrap: wrap;
        gap: 2rem;
        align-items: start;
        justify-content: center;
    }

    h3 {
        font-family: "Roboto Slab", sans-serif;
        font-size: 2rem;
        font-weight: 350;
        color: #d5d6d8;
        letter-spacing: 1px;
        text-transform: uppercase; 
        text-align: center;
        padding-bottom: 2rem;
    }

    p {
        font-family: "Roboto Slab", sans-serif;
        font-size: 1rem;
        font-weight: 350;
        color: #d5d6d8;
        letter-spacing: 1px;
        padding-bottom: 1rem;
        max-inline-size: 67ch;
    }
</style>