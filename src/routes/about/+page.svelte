<script>
  import Skills from "$lib/Skills.svelte";
  import Projects from "$lib/Projects.svelte";
  import Button from "$lib/Button.svelte";
  import ButtonImage from "../../lib/Button_Image.svelte";
  import Header from "$lib/Header.svelte";
  import Footer from "$lib/Footer.svelte";
</script>

<svelte:head>
  <title>Austin Tallent's Portfolio</title>
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
      <div class="image-container">
        <ButtonImage
          style="transform:translate(-40px,30px)"
          text="I was born on April 25, 2008."
          MarkerText="2008 I was born"
        />
        <img src="/Images/my-story-background.svg" alt="Austin" class="image" />

        <ButtonImage
          transform="90px,-1770px"
          text="I started using prismacolor pencils and produced my first actually good artwork in 2018."
          MarkerText="2018 Pencils"
        />
        <ButtonImage
          transform="-20,-10000px"
          text="In 2019, I started learning Blender."
          MarkerText="2019 Blender"
        />
        <ButtonImage
          transform="-20,15540px"
          text="In 2020, I started learning Inkscape"
          MarkerText="2020 Inkscape"
        />      <ButtonImage
        transform="-20,15540px"
        text="In 2021, I started learning acrylics."
        MarkerText="2021 Acrylic Paints"
      />
        <ButtonImage
          transform="-30,-190px"
          text="In 2023, I won the regional VFW art contest for the second time."
          MarkerText="2023 VFW Art"
        />
        <ButtonImage
          transform="-20px,-190px"
          text="In September of 2023, I started learning web design using HTML and CSS"
          MarkerText="2023 Web Design"
        />
        <ButtonImage
          transform="-20,15540px"
          text="In November of 2023, Blender 4.0 was released, and exciting improved version of Blender with many new and improved features!"
          MarkerText="2023 Blender 4.0"
        />
        <ButtonImage
          transform="-60px,-190px"
          text="In December of 2024, I finished my first oil paintings, and now oil paints are my medium of choice."
          MarkerText="2024 Oil Paints"
        />
      </div>
      <br />
      <Button link="/contact" buttonText="CONTACT ME!" buttonColor="--green" />
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
