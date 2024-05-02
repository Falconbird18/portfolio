<svelte:head>
    <title>Austin Tallent's Porfolio</title>
<link rel="stylesheet" 
href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css">
</svelte:head>



<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Austin Tallent's Portfolio</title>
<style>
  :root {
    --pale-blue-light: #c9d7f0;
    --pale-blue-dark: #9fb8e5; 
    --blue: #6186ff;
    --blue-hover: #5778e6;
    --text-blue: rgb(25, 26, 31);
    --pale-purple-light: #ddc9f0;
    --purple: #b061ff;
    --purple-hover: #9e57e6;
    --pale-purple-dark: #c29ee6;
    --green: #61ffa5;
    --green-hover: #57e695;
    --pale-green-light: #d6ffe8;
    --pale-green-dark: #c1e6d1;
    --white-hover: #e6e6e6;
    --scale: 1.25;
}
  body {
    font-family: 'Arial', sans-serif;
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
  .button-blue{
    display: inline-block;
    text-decoration: none;
    color: white;
    background-color: var(--blue);
    padding: 15px;
    border-radius: 30px;
    margin-top: 30px;
    margin-bottom: 30px;
transition: all 0.5s ease;
  }
  .button-blue:hover{
    color: var(--white-hover);
    background-color: var(--blue-hover);
    cursor: pointer;
    transform: scale(var(--scale));
    margin-left: 20px;
    margin-right: 20px;
  }
  .button-green{
    display: inline-block;
    text-decoration: none;
    color: white;
    background-color: var(--green);
    padding: 15px;
    border-radius: 30px;
    margin-top: 30px;
    margin-bottom: 30px;
transition: all 0.5s ease;
  }
  .button-green:hover{
    color: var(--white-hover);
    background-color: var(--green-hover);
    cursor: pointer;
    transform: scale(var(--scale));
    margin-left: 20px;
    margin-right: 20px;
  }
  .button-purple{
    display: inline-block;
    text-decoration: none;
    color: white;
    background-color: var(--purple);
    padding: 15px;
    border-radius: 30px;
    margin-top: 30px;
    margin-bottom: 30px;
transition: all 0.5s ease;
  }
  .button-purple:hover{
    color: var(--white-hover);
    background-color: var(--purple-hover);
    cursor: pointer;
    transform: scale(var(--scale));
    margin-left: 20px;
    margin-right: 20px;
  }
  .header{
    background-color: var(--pale-blue-light);
    padding: 30px;
  }
  .footer{
    background-color: var(--pale-blue-light);
    padding: 30px;
    text-decoration: none;
  }
  .header-text{
    display: inline-block;
    color: var(--blue);
    font-size: 20px;
    padding-left: 20px;
    padding-right: 20px;
    padding-top: 0px;
    padding-bottom: 0px;
    transition: all 0.5s ease;
    transform: scale(1);
  }
  .header-text:hover{
    color: var(--blue-hover);
    cursor: pointer;
    transform: scale(var(--scale));
    margin-left: 20px;
    margin-right: 20px;
  }
  .header-button{
    display: inline-block;
    color: white;
    background-color: var(--blue);
    border-radius: 30px;
    padding-left: 20px;
    padding-right: 20px;
    padding-top: 15px;
    padding-bottom: 15px;
    transition: all 0.5s ease;
  }
  .header-button:hover{
    color: var(--white-hover);
    background-color: var(--blue-hover);
    cursor: pointer;
    transform: scale(var(--scale));
    margin-left: 20px;
    margin-right: 20px;
  }
  h1{
    font-weight: normal;
    font-size: 45px;
    padding-top: 20px;
    padding-bottom: 20px;
    margin: 0px;
  }
  h2{
    font-weight: normal;
    font-size: 25px;
    padding-top: 20px;
    padding-bottom: 20px;
    margin: 0px;
    text-transform: uppercase;
  }
  p{
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

.education{
  background-color: var(--pale-purple-light);
  padding-bottom: 50px;
}
.svg{
  background-color: var(--pale-blue-light);
  margin: 0;
  padding: 0%;
  transform: translateY(-20px);
}
.skills{
  background-color: var(--pale-green-light);
}
.footer-text{
  font-size: 20px;
  color: var(--blue);
  text-align: center;
    display: inline-block;
    padding-left: 20px;
    padding-right: 20px;
    padding-top: 20px;
    padding-bottom: 0px;
    transition: all 0.5s ease;
    transform: scale(1);
    text-decoration: none;
}
.footer-text:hover{
    color: var(--blue-hover);
    cursor: pointer;
    transform: scale(var(--scale));
    margin-left: 20px;
    margin-right: 20px;
    text-decoration: none;
}
.copyright{
  color: var(--blue);
}
.progress-container {
    background-color: var(--pale-purple-dark); /* Set a background color for the container */
    text-align: center;
    margin: 0 auto;
    margin-top: 50px; /* Add some padding for spacing */
    margin-bottom: 50px;
    padding: 15px;
    width: 50%;
    border-radius: 30px;
}
.progress-bar{
    background-color: var(--purple); /* Set the color of the progress bar */
    height: 24px; /* Set the height of the progress bar */
    line-height: 24px; /* Vertically center the text inside the bar */
    color: #ffffff; 
    border-radius: 30px;
    text-transform: uppercase;
    margin-bottom: 30px;
    visibility: visible;
    opacity: 1;
  cursor: pointer;
transition: all 0.5s ease;
    border: none;
}
.progress-bar:hover{
  transform: scale(var(--scale)) !important;
  background-color: var(--purple-hover);
}
.progress-bar:hover + .hide {
    background-color: #8d4ecc; /* Set the color of the progress bar */
    line-height: 24px; /* Vertically center the text inside the bar */
    color: white; /* Text color */
    border-radius: 30px;
    padding-top: 60px;
    padding-bottom: 60px;
    padding-left: 30px;
    padding-right: 30px;
    visibility: visible;
    opacity: 1;
  cursor: pointer;
transition: all 0.5s ease;
position: fixed; /* or absolute */
  top: 50%;
  left: 50%;
  /* bring your own prefixes */
  transform: translate(-50%, -50%);
  /*box-shadow: rgba(0, 0, 0, 0.35) 0px 5px 15px;*/
  
}
.progress-bar-container {
    background-color: var(--purple-hover); /* Set the color of the progress bar */
    height: 24px; /* Set the height of the progress bar */
    line-height: 24px; /* Vertically center the text inside the bar */
    text-align: center; /* Center the label text */
    color: #ffffff; /* Text color */
    border-radius: 30px;
    margin-top: 30px;
}
.hide {
  visibility: hidden;
  opacity: 0;
  background-color: var(--pale-green-dark);
  line-height: 24px;
  color: #ffffff;
  border-radius: 30px;
  text-align: center;
  position: relative; /* Change this to relative */
  padding-top: 60px;
  padding-bottom: 60px;
  padding-left: 30px;
  padding-right: 30px;
  max-height: 75%;
  max-width: 50%;
}
.image{
  width: 25%;
  height: auto;
  text-align: center;
  padding: 30px;
  border-radius: 30px;
  margin-top: 50px;
  margin-bottom: 50px;
  background-color: var(--pale-blue-dark);
}
.skill-images{
  max-width: 85%;
  height: auto;
  padding: 30px;
  border-radius: 30px;
  background-color: var(--purple-hover);
  margin-top: 15px;
}
.hidden {
  display: none;
  opacity: 0;
  transition: all 0.5s ease;
}
#large-view {
  width: 100%;
  background-color: #8d4ecc;
  transition: all 0.5s ease;
  opacity: 1;
  text-align: center;
  transform: translate(0px,-100px);
  border-radius: 30px;
  padding: 30px;
  margin: 0 auto;
  transform: translateX(-5%);
  position: relative;
  z-index: 3;
  box-shadow: rgba(0, 0, 0, 0.3) 0px 19px 38px, rgba(0, 0, 0, 0.22) 0px 15px 12px;
}

/*#overlay {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  filter: blur(0px);
  transition: filter 0.5s ease;
  overflow-y: scroll;
}*/

</style>
<body>
    <div id="overlay">
    <header class="header">
        <a class="header-text">ABOUT</a>
        <a class="header-text">SKILLS</a>
        <a class="header-text">PORTFOLIO</a>
        <a class="header-text">PROJECTS</a>
        <a class="header-button">CONTACT</a>
    </header>
  <div class="intro">
    <h1>Hi, I'm Austin Tallent</h1>
    <h2>Artist, CG Geek, and UI Designer</h2>
    <a href="about.html" class="button-blue">DOWNLOAD RESUME</a>
  </div>
  <div class="about">
    <h2 style="background-color: var(--pale-blue-dark); border-radius: 0px 0px 30px 30px;">About Me</h2>
    <p>Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum. Sed ut perspi unde omnis iste natus error sit voluptatem accusantium doloremque lauda ntium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo.</p>
    <img src="/Images/test-portfolio.jpg" alt="Austin" class="image">
    <br>
    <a class="button-blue" href="about.html">TELL ME MORE!</a>
  </div>

  <div class="education">
    <!--<svg viewBox='0 0 1200  134' fill='none' xmlns='http://www.w3.org/2000/svg' class="svg">
      <path d='M0 22L33 19C82 13 133 14 20 29C267 44 333 67 400 70C467 74 533 59 600 40C667 22 733 0 800 0C867 0 933 22 1000 29C1067 37 1133 29 1167 26L1200 22V134H1167C1133 134 1067 134 1000 134C933 134 867 134 800 134C733 134 667 134 600 134C533 134 467 134 400 134C333 134 267 134 200 134C133 134 67 134 33 134H0V22.332Z' fill='#ddc9f0'/>
    </svg>-->
    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320" fill="none" class="svg">
      <path fill="#ddc9f0" fill-opacity="1" d="M0,64L48,90.7C96,117,192,171,288,181.3C384,192,480,160,576,176C672,192,768,256,864,272C960,288,1056,256,1152,250.7C1248,245,1344,267,1392,277.3L1440,288L1440,320L1392,320C1344,320,1248,320,1152,320C1056,320,960,320,864,320C768,320,672,320,576,320C480,320,384,320,288,320C192,320,96,320,48,320L0,320Z"></path>
    </svg>
    <h2 style="background-color: var(--pale-purple-light);">SKILLS</h2>

    <p>I am skilled in many areas and different software. Some of them are listed below.</p>
    <div class="progress-container">
        <div class="progress-bar-container">
          <button id="showButton" class="progress-bar" style="width:95%; transform:translateX(-2.5%)">3D ART: 95%</button>
      <div id="large-view" class="hidden">
        I have many skills!
        <img src="/Images/arch.png" alt="Visualization" class="skill-images">
      </div> 
        </div>
      </div>
<div class="progress-container">
  <div class="progress-bar-container">
    <div class="progress-bar" style="width: 95%;">3d art: 95%</div>
    <div class="hide">
      I have skills in Animation, Texturing, Modeling, Animation, and more.
      <img src="/Images/arch.png" alt="Visualization" class="skill-images">
    </div>
  </div>
  <div class="progress-bar-container">
    <div class="progress-bar" style="width: 75%;">painting: 75%</div>
    <div class="hide">I am skilled in painting using both oils and acrylics, and even digitally!</div>
  </div>
  <div class="progress-bar-container">
    <div class="progress-bar" style="width: 90%;">drawing: 90%</div>
    <div class="hide">I draw with colored pencils, regular pencils, and graphite.</div>
  </div>
  <div class="progress-bar-container">
    <div class="progress-bar" style="width: 65%;">vector graphics: 65%</div>
    <div class="hide">I create vector graphics, and enjoy the process.</div>
  </div>
  <div class="progress-bar-container">
    <div class="progress-bar" style="width: 95%;">ui design: 80%</div>
    <div class="hide">I use HTML and CSS to create stunning website designs.</div>
  </div>
</div>
<div class="progress-container">
  <div class="progress-bar-container">
    <div class="progress-bar" style="width: 95%;">
      Blender: 95%
    </div>
  </div>
  <div class="progress-bar-container">
    <div class="progress-bar" style="width: 85%;">
      Inkscape: 85%
    </div>
  </div>
  <div class="progress-bar-container">
    <div class="progress-bar" style="width: 77%;">
      krita: 77%
    </div>
  </div>
  <div class="progress-bar-container">
    <div class="progress-bar" style="width: 49%;">
      gimp: 49%
    </div>
  </div>
  <div class="progress-bar-container">
    <div class="progress-bar" style="width: 53%;">
      html & css: 53%
    </div>
  </div>
</div>
    <a class="button-purple" href="skills.html">MORE INFO</a>
</div>
  <div class="skills">
    <h2 style="background-color: var(--pale-green-dark);">projects</h2>
    <a class="button-green" href="skills.html">ALL PROJECTS</a>
</div>
                        </div>
      <footer class="footer">
        <a class="copyright">&copy 2024 Austin Tallent All Rights Reserved</a>
        <br>
        <div class="footer-text">
        <i class="fa-brands fa-artstation" href="https://www.artstation.com/austin_tallent"></i>
        </div>
        <div class="footer-text">
        <i class="fa-solid fa-envelope"></i>
        </div>
      </footer>

<script>

// Get the button and the rectangle element
var button = document.getElementById('showButton');
var rectangle = document.getElementById('large-view');
var overlay = document.getElementById('overlay');
/*
// Function to toggle the visibility of the rectangle and the overlay
function toggleRectangle() {
  // Check if the rectangle is hidden
  if (rectangle.classList.contains('hidden')) {
    rectangle.classList.remove('hidden');
    overlay.classList.add('show'); // Show the overlay
    // Wait for the next browser repaint to ensure the class change has taken effect
    window.requestAnimationFrame(function() {
      rectangle.style.opacity = '1';
    });
  } else {
    rectangle.style.opacity = '0';
    overlay.classList.remove('show'); // Hide the overlay
    // Wait for the transition to finish before hiding the element
    rectangle.addEventListener('transitionend', function hideElement() {
      rectangle.classList.add('hidden');
      rectangle.removeEventListener('transitionend', hideElement);
    });
  }
}
*/
/*function toggleRectangle() {
  if (rectangle.classList.contains('hidden')) {
    rectangle.classList.remove('hidden');
    overlay.classList.add('show');
    overlay.style.filter = 'blur(8px)';
  } else {
    rectangle.style.opacity = '0';
    overlay.classList.remove('show');
    overlay.style.filter = 'blur(0px)';
    // Wait for the transition to finish before hiding the element
    rectangle.addEventListener('transitionend', function hideElement() {
      rectangle.classList.add('hidden');
      rectangle.removeEventListener('transitionend', hideElement);
    });
  }
}*/

function toggleRectangle() {
  if (rectangle.classList.contains('hidden')) {
    rectangle.classList.remove('hidden');
    //overlay.style.filter = 'blur(8px)'
    window.requestAnimationFrame(function() {
      rectangle.style.opacity = '1';
    });
  } else {
    rectangle.style.opacity = '0';
    //overlay.style.filter = 'blur(0px)'
    rectangle.addEventListener('transitionend', function hideElement() {
      rectangle.classList.add('hidden');
      rectangle.removeEventListener('transitionend', hideElement);
    });
  }
}

// Add click event listener to the button to show the rectangle
button.addEventListener('click', toggleRectangle);
// Add click event listener to the document to hide the rectangle
document.addEventListener('click', function(event) {
  if (!rectangle.classList.contains('hidden') && event.target !== button) {
    toggleRectangle();
  }
});


</script>
</body>