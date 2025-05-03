<div class="layout">
        <header id="home">
            <div class="container">
                <nav>
                    <ul>
                        <li>
                            <a href="#home">Home</a>
                            <span>&nbsp;&nbsp;&nbsp;|</span>
                        </li>
                        <li>
                            <a href="#about">About</a>
                            <span>&nbsp;&nbsp;&nbsp;|</span>
                        </li>
                        <li>
                            <a href="#contact">Contact</a>
                        </li>
                    </ul>
                </nav>
            </div>
            <h1>JOSEPH CHAUVIN</h1>
            <h2>Video Game Composer</h2>
        </header>
        <div class="container">
            <section id="demos" class="demos">
                <!-- <iframe title="Mega Man Inspired Music" width="700" height="393.75" src="https://www.youtube.com/watch?v=ZJcMD57075o"></iframe> -->
                <iframe width="100%" height="515" src="https://www.youtube.com/embed/ZJcMD57075o?si=f_0gTA4hlY3ISJb2" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
            </section>
            <section id="about">
                
            </section>
            <section id="contact">
            
            </section>
        </div>
</div>

<style>
    .layout {
        display: flex;
        align-items: center;
        flex-direction: column;
        /* justify-content: center; */
        background: var(--gray-1);
        color: var(--gray-12);
        min-height: 100dvh;
    }
    
    .container {
        max-inline-size: 914px;
        width: 100%;
    }

    header {
        display: flex;
        flex-direction: column;
        align-items: center;
        padding: 2rem;
        gap: 1rem;
        width: 100%;
        background: var(--indigo-3);
    }

    nav {
        display: flex;
        align-items: center;
        justify-content: center;
    }

    h1 {
        font-family: "KronaOne", "inter";
        font-size: 3rem;
        /* font-size: 3cqw; */
        margin: 0;
        letter-spacing: -4.5px;
        color: var(--gray-12);
        font-style: italic;
    }

    h2 {
        font-family: "Gurmukhi MT", "inter";
        font-size: 16px;
        font-weight: 400;
        text-transform: uppercase;
    }

    ul {
        display: flex;
        list-style: none;
        align-items: center;
        gap: 1rem;
        margin: 0;
        padding: 0;
    }

    a {
        text-decoration: none;
        /* color: var(--blue-9); */
        color: var(--gray-12);
    }
    
    /* li span {
        color: var(--blue-9);
    } */

    a:hover {
        text-decoration: underline;
    }

    .demos {
        padding-block: 64px;
    }
</style>