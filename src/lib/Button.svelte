<script>
    export let link = "about.html";
    export let buttonText = "tell me more!";
    export let buttonColor = "--blue";
</script>
<a class="button" href="{link}" style="background-color: var({buttonColor});">{buttonText}</a>


<style>
    .button{
    display: inline-block;
    text-decoration: none;
    color: white;
    padding: 15px;
    border-radius: var(--radius);
    margin-top: 30px;
    margin-bottom: 30px;
    transition: all var(--time) ease;
    text-transform: uppercase;
  }
  .button:hover {
    cursor: pointer;
    transform: scale(var(--scale));
    margin-left: 20px;
    margin-right: 20px;
    filter: brightness(var(--hover-brightness));
  }
</style>