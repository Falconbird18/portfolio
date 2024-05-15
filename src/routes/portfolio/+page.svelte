<script>
    import Skills from "$lib/Skills.svelte";
    import Projects from "$lib/Projects.svelte";
    import Button from "$lib/Button.svelte";
    import Header from "$lib/Header.svelte";
    import Footer from "$lib/Footer.svelte"
    import { Tabs, TabList, Tab, TabPanel } from '@colorfuldots/svelteit'
    import Image from "$lib/Gallery.svelte"
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
        <h1>Gallery</h1>
        <!--Use cat picture from the nine for the header background image.-->
      </div>
      <div class="about">
        <Tabs>
          <Tab>Paintings</Tab>
          <Tab>Blender</Tab>
          <Tab>Projects</Tab>

          <TabPanel>

            <h2 style="background-color: var(--pale-blue-dark); border-radius: 0px 0px 30px 30px;">Paintings</h2>
            These are my paintings.

            <div class="gallery">
              <Image />
              <Image />
              <Image />
              <Image />
              <Image />
            </div>
          </TabPanel>

          <TabPanel>
            <h2 style="background-color: var(--pale-blue-dark); border-radius: 0px 0px 30px 30px;">Blender</h2>
            These are my Blender projects.
              <Image />
              <Image />
              <Image />
              <Image />
              <Image />
              <Image />
          </TabPanel>

          <TabPanel>
            <h2 style="background-color: var(--pale-blue-dark); border-radius: 0px 0px 30px 30px;">Projects</h2>
             These are all my projects.
              <Image />
              <Image />
              <Image />
              <Image />
              <Image />
              <Image />
          </TabPanel>
        </Tabs>
      </div>
      <Footer />
    </body>
  
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
    .gallery{
      columns: 3;
    }
    body {
      font-family: "Arial", sans-serif;
      text-align: center;
    }
    .intro {
      color: white;
      padding-top: 150px;
      padding-bottom: 150px;
      background-image: url(/Images/painting.jpg);
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
    p {
      text-align: center;
      font-size: 15px;
      width: 50%;
      margin: 0 auto;
      margin-top: 50px;
    }
    .about {
      position: relative;
      background-color: var(--pale-blue-light);
      color: var(--text-blue);
    }
  </style>
  