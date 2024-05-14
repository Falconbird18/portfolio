<script>
  import Skills from "$lib/Skills.svelte";
  import Projects from "$lib/Projects.svelte";
  import Button from "$lib/Button.svelte";
  import ButtonImage from "../../lib/Button_Image.svelte";
  import Header from "$lib/Header.svelte";
  import Footer from "$lib/Footer.svelte";
</script>

<svelte:head>
  <title>Austin Tallent's Porfolio</title>
  <link
    rel="stylesheet"
    href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css"
  />

  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
</svelte:head>
<body>
  <div id="overlay">
    <Header />
    <div class="intro">
      <h1>ABOUT ME</h1>
    </div>

    <div class="about">
      <h2
        style="background-color: var(--pale-green-dark); border-radius: 0px 0px 30px 30px;"
      >
        MY STORY
      </h2>

      <ButtonImage
        transform="-10px,320px"
        text="I was born on April 25, 2008."
      />
      <ButtonImage
        transform="-10px,320px"
        text="In December of 2024, I finished my first oil paintings, and now oil paints are my medium of choice."
        buttonImageSource="/Images/oils.svg"
      />
      <div class="image-container">
        <img src="/Images/my-story-background.svg" alt="Austin" class="image" />
      </div>

      <br />
      <Button
        link="https://calvintallent.me"
        buttonText="CONTACT ME!"
        buttonColor="--green"
      />
    </div>
    <Footer />
  </div></body
>

<style>
  :root {
    --pale-blue-light: #c9d7f0;
    --pale-blue-dark: #9fb8e5;
    --blue: #6186ff;
    --text-blue: rgb(25, 26, 31);
    --pale-purple-light: #ddc9f0;
    --purple: #b061ff;
    --pale-purple-dark: #c29ee6;
    --green: #61ffa5;
    --pale-green-light: #d6ffe8;
    --pale-green-dark: #c1e6d1;
    --scale: 1.25;
    --time: 0.5s;
    --radius: 30px;
    --hover-brightness: 0.9;
  }
  body {
    font-family: "Arial", sans-serif;
    text-align: center;
  }
  .intro {
    color: white;
    padding-top: 150px;
    padding-bottom: 500px;
    background-image: url(/Images/grapes.jpg);
    background-attachment: fixed;
    background-size: 100%;
  }
  .header {
    background-color: var(--pale-blue-light);
    padding: 30px;
  }
  .footer {
    background-color: var(--pale-blue-light);
    padding: 30px;
    text-decoration: none;
  }
  .header-text {
    display: inline-block;
    color: var(--blue);
    font-size: 20px;
    padding-left: 20px;
    padding-right: 20px;
    padding-top: 0px;
    padding-bottom: 0px;
    transition: all var(--time) ease;
    transform: scale(1);
  }
  .header-text:hover {
    cursor: pointer;
    transform: scale(var(--scale));
    margin-left: 20px;
    margin-right: 20px;
    filter: brightness(var(--hover-brightness));
  }
  .header-button {
    display: inline-block;
    color: white;
    background-color: var(--blue);
    border-radius: var(--radius);
    padding-left: 20px;
    padding-right: 20px;
    padding-top: 15px;
    padding-bottom: 15px;
    transition: all var(--time) ease;
  }
  .header-button:hover {
    cursor: pointer;
    transform: scale(var(--scale));
    margin-left: 20px;
    margin-right: 20px;
    filter: brightness(var(--hover-brightness));
  }
  h1 {
    font-weight: normal;
    font-size: 45px;
    padding-top: 20px;
    padding-bottom: 20px;
    margin: 0px;
  }
  h2 {
    font-weight: normal;
    font-size: 25px;
    padding-top: 20px;
    padding-bottom: 20px;
    margin: 0px;
    text-transform: uppercase;
  }
  .about {
    position: relative;
    background-color: var(--pale-green-light);
    color: var(--text-blue);
  }
  .footer-text {
    font-size: 20px;
    color: var(--blue);
    text-align: center;
    display: inline-block;
    padding-left: 20px;
    padding-right: 20px;
    padding-top: 20px;
    padding-bottom: 0px;
    transition: all var(--time) ease;
    transform: scale(1);
    text-decoration: none;
  }
  .footer-text:hover {
    color: var(--blue-hover);
    cursor: pointer;
    transform: scale(var(--scale));
    margin-left: 20px;
    margin-right: 20px;
    text-decoration: none;
  }
  .copyright {
    color: var(--blue);
  }
  .image-container {
    width: 75%;
    height: auto;
    text-align: center;
    padding: 30px;
    border-radius: var(--radius);
    background-color: var(--pale-green-dark);
    margin: 0 auto;
    margin-top: 50px;
    margin-bottom: 50px;
  }
  .image {
    width: 100%;
    height: auto;
    text-align: center;
    border-radius: var(--radius);
  }
</style>
