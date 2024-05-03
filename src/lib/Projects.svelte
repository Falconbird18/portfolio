<script>
  export let projectTitle = "a title";
  export let projectDescription = "A description";
  export let imageSource = "image";
  export let alt = "image alt";
</script>

<div class="projects">
  <h2 style="background-color: var(--pale-green-dark;">projects</h2>
  <div class="green">
    <p>Some of the projects that I have worked on are:</p>
    <div class="project-containers">
      <h2>{projectTitle}</h2>
      <p>{projectDescription}</p>
      <img class="image" src="{imageSource}" alt="{alt}" />
    </div>
  </div>
</div>

<style>
  .projects {
    background-color: var(--pale-green-light);
  }
  h2 {
    font-weight: normal;
    font-size: 25px;
    padding-top: 20px;
    padding-bottom: 20px;
    margin: 0px;
    text-transform: uppercase;
  }
  .green {
    background-color: var(--pale-green-light);
    padding-top: 20px;
    padding-bottom: 50px;
  }
  .project-containers {
    background-color: var(--pale-green-dark);
    text-align: center;
    margin: 0 auto;
    margin-top: 50px; /* Add some padding for spacing */
    padding: 15px;
    width: 50%;
    border-radius: var(--radius);
  }
  .image{
    width: 95%;
    height: auto;
    border-radius: var(--radius);
  }
</style>
