<script>
  import Skills from "$lib/Skills.svelte";
  import Projects from "$lib/Projects.svelte";
  import Button from "$lib/Button.svelte";
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
<body style="background-color: rgba(255, 255, 255, 0); margin: 0px;">
  <div id="overlay">
    <div class="intro">
    <Header/>
      <h1>Hi, I'm Austin Tallent</h1>
      <h2>Artist, CG Geek, and UI Designer</h2>
      <Button
        link="https://calvintallent.me"
        buttonText="download resume"
        buttonColor="--blue"
      />
    </div>
    <div class="about">
      <h2 class="rounded-header" style="background-color: var(--pale-blue-dark);">About Me</h2>
      <p>
        I love painting, Blender, and other types of art (except modern art!) 
      </p>
      <div class="image-container">
      <img src="/Images/painting.jpg" alt="Austin" class="image" />
      </div>
      <br />
      <Button
        link="/about"
        buttonText="tell me more"
        buttonColor="--blue"
      />
    </div>

    <div class="education">
      <!--<svg viewBox='0 0 1200  134' fill='none' xmlns='http://www.w3.org/2000/svg' class="svg">
      <path d='M0 22L33 19C82 13 133 14 20 29C267 44 333 67 400 70C467 74 533 59 600 40C667 22 733 0 800 0C867 0 933 22 1000 29C1067 37 1133 29 1167 26L1200 22V134H1167C1133 134 1067 134 1000 134C933 134 867 134 800 134C733 134 667 134 600 134C533 134 467 134 400 134C333 134 267 134 200 134C133 134 67 134 33 134H0V22.332Z' fill='#ddc9f0'/>
    </svg>-->
      <svg
        xmlns="http://www.w3.org/2000/svg"
        viewBox="0 0 1440 320"
        fill="none"
        class="svg"
      >
        <path
          fill="#ddc9f0"
          fill-opacity="1"
          d="M0,64L48,90.7C96,117,192,171,288,181.3C384,192,480,160,576,176C672,192,768,256,864,272C960,288,1056,256,1152,250.7C1248,245,1344,267,1392,277.3L1440,288L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"
        ></path>
      </svg>
      <h2 style="background-color: var(--pale-purple-light);">SKILLS</h2>

      <p>
        I am skilled in many areas and different software. Some of them are
        listed below.
      </p>
      <div class="progress-container">
        <Skills
          buttonText="3D ART 95%"
          closeButtonText="close"
          popupText="I have more than five years of experience with 3D, and have worked on several big projects."
          width="95%"
        />

        <Skills
          buttonText="PAINTING 75%"
          closeButtonText="close"
          popupText="I paint with oils, and am inspired by the old masters, such as the hudson river school, and Rembrandt."
          width="75%"
        />

        <Skills
          width="90%"
          buttonText="Drawing: 90%"
          closeButtonText="Close"
          popupText="I like drawing, "
        />
        <Skills
          width="70%"
          buttonText="vector art: 70%"
          closeButtonText="Close"
          popupText="Unlike some vector art, my vector art is shaded, and I try to create depth and imersion."
        />
        <Skills
          width="75%"
          buttonText="Digital art: 75%"
          closeButtonText="Close"
          popupText="I like drawing digitally "
        />
    </div>
    <p>I have learned many different software. Some of them are listed below.</p>
        <div class="progress-container">
        <Skills
          width="95%"
          buttonText="blender: 95%"
          closeButtonText="Close"
          popupText="I have used Blender for more than 5 years, and can do almost anything in the program. My skills include modeling, texturing, lighting, architectuarl visulization, and more!"
        />
        <Skills
          width="85%"
          buttonText="krita: 85%"
          closeButtonText="Close"
          popupText="Popup"
        />
        <Skills
          width="80%"
          buttonText="inkscape: 80%"
          closeButtonText="Close"
          popupText="Popup"
        />
        <Skills
          width="60%"
          buttonText="gimp: 60%"
          closeButtonText="Close"
          popupText="Popup"
        />
        <Skills
          width="50%"
          buttonText="natron: 50%"
          closeButtonText="Close"
          popupText="I use Natron (Similar to Nuke or After Effects) for my compositing, and enjoy the node-based workflow. I also do some compositing in Blender."
        />

        <Skills
          width="55%"
          buttonText="kdenlive: 55%"
          closeButtonText="Close"
          popupText="Popup"
        />
        </div>
      <Button
        link="/skills"
        buttonText="more info"
        buttonColor="--purple"
      />
    </div>
<div class="projects">
  <h2 class="rounded-header" style="background-color: var(--pale-green-dark;">projects</h2>
  <div class="green">
    <p>Some of the projects that I have worked on are:</p>
      <Projects 
      projectTitle="supper froggy"
      projectDescription="Supper Froggy is a full length movie in development. Currently, I have completed about a minute and a half of footage, created in Blender."
      imageSource="/Images/supper_froggy.png"
      alt="Supper Froggy"
      />
      <Projects 
      projectTitle="my house"
      projectDescription="I have been working on a 3D version of my house. It is about fifty percent complete."
      imageSource="/Images/supper_froggy.png"
      alt="My house"
      />
      <Projects 
      projectTitle="737 max project"
      projectDescription="I have just started working on a 737 MAX for FlightGear"
      imageSource="/Images/supper_froggy.png"
      alt="737 MAX cockpit"
      />
      <Button
        link="/skills"
        buttonText="view all projects"
        buttonColor="--green"
      />
  </div>
  <div class="yellow">
  <h2 class="rounded-header" style="background-color: var(--pale-yellow-dark;">software</h2>
  <p>The links to the software I use are listed below.</p>
  <a href="">Blender</a>
  <a href="">Inkscape</a>
  <a href="">GIMP</a>
  <a href="">Krita</a>
  <a href="">Kdenlive</a>
  <a href="">Natron</a>
  </div>
      <Footer />
  </div>
  </div>
  </body
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
      --pale-yellow-light: #fffad6;
      --pale-yellow-dark: #e6e1c1;
      --yellow: #FFEA61;
  }
  body {
    font-family: "Arial", sans-serif;
    text-align: center;
  }
  .intro {
    color: white;
    padding-top: 10%;
    padding-bottom: 20%;
    background-image: url(/Images/painting.jpg);
    background-attachment: fixed;
    background-size: 100%;
  }
  .yellow{
    background-color: var(--pale-yellow-light);
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
  .rounded-header{
    border-radius: var(--radius) var(--radius) var(--radius) var(--radius);
    transform: translate(0px, -40px)
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

  .education {
    background-color: var(--pale-purple-light);
    padding-bottom: 50px;
  }
  .svg {
    background-color: var(--pale-blue-light);
    margin: 0;
    padding: 0%;
    transform: translateY(-20px);
  }
  .progress-container {
    background-color: var(
      --pale-purple-dark
    ); /* Set a background color for the container */
    text-align: center;
    margin: 0 auto;
    margin-top: 50px; /* Add some padding for spacing */
    margin-bottom: 50px;
    padding: 15px;
    width: 50%;
    border-radius: var(--radius);
  }
  .image-container {
    width: 25%;
    height: auto;
    text-align: center;
    padding: 30px;
    border-radius: var(--radius);
    background-color: var(--pale-blue-dark);
    margin: 0 auto;
    margin-top: 50px;
    margin-bottom: 50px;
  }
  .image{
    width: 100%;
    height: auto;
    text-align: center;
    border-radius: var(--radius);
}
  .projects {
    background-color: var(--pale-green-light);
  }
  .green {
    background-color: var(--pale-green-light);
    padding-top: 20px;
    padding-bottom: 50px;
  }
  @media only screen and (max-width: 768px) {
    p {
      width: 75%;
    }
    .progress-container {
      width: 75%;
    }
    .image-container {
      width: 50%;
    }
}
</style>
