<script>
  import Card from '../components/Card.svelte';
  import { projects } from '../data/projects';
</script>

<div id="projects" class="container">
  <div class="projects">
    <h2>Projects</h2>
    <div class="grid">
      {#each projects as project}
        <div class="grid-item">
          <Card project={project} />
        </div>
      {/each}
    </div>
  </div>
</div>

<style>
  .container {
    background-color: #dadada;
    padding: 60px 0;
  }

  .projects {
    margin: 0 auto;
    max-width: 1200px;
    padding: 0 20px;
  }

  .grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px,1fr));
    row-gap: 50px;
    column-gap: 20px;
  }

  h2 {
    /* text-align: center; */
    margin-bottom: 25px;
  }
</style>
