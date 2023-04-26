<script>
    //
</script>

<div id="skills" class="container">
    <div class="skills">
        <h2>Skills</h2>
        <div class="cols">
            <div class="col col-left">
                <p>HTML</p>
                <p>CSS</p>
                <p>JavaScript</p>
                <p>React</p>
                <p>Redux</p>
                <p>Svelte</p>
                <p>Tailwind</p>
            </div>
            <div class="col col-right">
                <p>Node.js</p>
                <p>Express</p>
                <p>MongoDB</p>
                <p>React Native</p>
                <p>TypeScript</p>
                <p>Next.js</p>
            </div>
        </div>
    </div>
</div>

<style>
    .container {
        background-color: white;
        padding: 60px 0;
    }

    .skills {
        margin: 0 auto;
        max-width: 1200px;
        text-align: center;
    }

    .cols {
        display: flex;
        justify-content: space-between;
        width: 70%;
        margin: 0 auto;
    }

    .col {
        display: flex;
        flex-direction: column;
        gap: 15px;
    }

    h2 {
        margin-bottom: 50px;
    }

    p {
        font-size: 1.5rem;
    }

    @media (max-width: 500px) {
        .cols {
            flex-direction: column;
        }

        .col-left {
            margin-bottom: 15px;
        }
    }
</style>