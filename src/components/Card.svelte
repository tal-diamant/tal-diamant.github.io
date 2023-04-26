<script>
    export let project;
</script>

<div class="card">
    <a href={project.url} style="width: 100%">
        <div class="card-text">
            {project.name}
        </div>
        <div>
            <img src={project.image} width="100%" alt="">
        </div>
    </a>
    <div class="card-text">
        <a href={project.github}>
            Github
        </a>
    </div>
</div>

<style>
    .card {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        border-radius: 10px;
        background-color: #aaa;
        height: auto;
        width: 100%;
        margin: 0 auto;
        overflow: hidden;
        padding: 5px;
    }

    .card-text {
        color: black;
        text-align: center;
        width: 100%;
        font-size: 1.5rem;
    }

    a:hover .card-text {
        color: white;
    }

    img {
        aspect-ratio: 1 / 1;
        width: 100%;
        height: auto;
    }
</style>