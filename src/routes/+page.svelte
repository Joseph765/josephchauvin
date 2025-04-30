<div class="layout">
    <div class="container">
        <header id="home">
            <h1>Joseph Chauvin</h1>
            <h2>Composer</h2>
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
        </header>
        <section id="demos">
            <iframe title="Mega Man Inspired Music" width="700" height="393.75" src="https://www.youtube.com/watch?v=ZJcMD57075o"></iframe>
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
        justify-content: center;
    }
    
    .container {
        max-inline-size: 700px;
    }

    header {
        display: flex;
        flex-direction: column;
        align-items: center;
        padding: 2rem;
        gap: 1rem;
    }

    h1 {
        font-family: "KronaOne", "inter";
        font-size: 3rem;
        margin: 0;
        letter-spacing: -4.5px;
        color: black;
    }

    h2 {
        font-family: "Gurmukhi MT";
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
        color: black;
    }

    a:hover {
        text-decoration: underline;
    }
</style>