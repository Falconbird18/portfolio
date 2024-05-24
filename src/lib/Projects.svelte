<script>
  export let projectTitle = "a title";
  export let projectDescription = "A description";
  export let imageSource = "image";
  export let alt = "image alt";
</script>
    <div class="project-containers">
      <h2>{projectTitle}</h2>
      <p>{projectDescription}</p>
      <img class="image" src="{imageSource}" alt="{alt}" />
    </div>
<style>
  h2 {
    font-weight: normal;
    font-size: 25px;
    padding-top: 20px;
    padding-bottom: 20px;
    margin: 0px;
    text-transform: uppercase;
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
