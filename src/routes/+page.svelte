<svelte:head>
    <title>Austin Tallent's Porfolio</title>
</svelte:head>

<style>
.photo{
    background-image: url(Images/flower.jpg);
    background-size: 100%;
    background-position-y: 30%;
    text-decoration: none;
    background-attachment: fixed;
    width: fit-content;
    height: auto;
    
}
.header{
    color: white;
    text-align: left;
    font-size: 80px;
    padding-left: 19%;
    padding-top: 90px;
    padding-bottom: 30px;
}
.small-header{
    color: white;
    text-align: left;
    font-size: 30px;
    padding-left: 19%;
    padding-right: 19%;
    padding-bottom: 300px;
}
.about{
    color: #131313;
    background-color: white;
    padding-left: 19%;
    padding-top: 100px;
    padding-right: 19%;
    padding-bottom: 150px;
    font-size: 30px;
}
.button{
    text-align: center;
    text-decoration: none;
    color: white;
    font-size: 40px;
    background-color: #333;
    padding: 30px;
}
.button:hover {
    color: #b1b1b1; /* Set the color for the link when hovered */
    text-decoration: none; /* Remove underline on hover */
    cursor: pointer; /* Add a pointer cursor on hover */
    background-color: #131313;
}
.nav{
    padding: 30px;
    background-color: #333;
    text-align: right;
}
.nav-logo{
    text-decoration: none;
    text-align: left;
    padding-top: 30px;
    padding-bottom: 30px;
    padding-left: 15px;
    padding-right: 15;
    transform: 50%,0%;
    color: white;
    font-size: 15px;
}
.nav-logo:hover{
    padding-left: 30px;
}

.nav-text{
    text-decoration: none;
    text-align: right;
    padding-top: 30px;
    padding-bottom: 30px;
    padding-left: 35px;
    padding-right: 35px;
    color: white;
    font-size: 15px;
}
.nav-text:hover {
    color: #b1b1b1; /* Set the color for the link when hovered */
    text-decoration: none; /* Remove underline on hover */
    cursor: pointer; /* Add a pointer cursor on hover */
    background-color: #131313;
}

.skills{
    color: black;
    background-color: white;
    padding-top: 180px;
    padding-left: 30px;
    font-size: 30px;
    width: 33%;
    height: auto;
}

.header-skills{
    color: black;
    text-align: left;
    font-size: 80px;
    padding-left: 19%;
    padding-top: 300px;
    padding-bottom: 30px;
}


.footer{
    text-align: left;
    color: white;
    background-color: #333;
    padding: 40px;
    padding-left: 19%;
    font-size: 11px;
}



body {
    font-family: Arial, sans-serif;
    background-color: #f9f9f9;
    margin: 0;
    padding: 0;
}
.container {
    padding-left: 19%;
    padding-right: 19%;
    padding-top: 50px;
    padding-bottom: 100px;
    background-color: #D8E4FF;
}
.skill {
    display: flex;
    align-items: center;
}
.skill img {
    width: 100%;
    height: auto;
    text-align: left;
}
.skill-description {
    flex: 1;
    font-size: 30px;
}
.learn-more {
    color: #ffffff;
    padding: 10px 20px;
    text-decoration: none;
    font-weight: bold;
    background-color: #333;
}
.learn-more:hover {
    text-decoration: none; /* Remove underline on hover */
    cursor: pointer; /* Add a pointer cursor on hover */
    background-color: #131313;
}
.white{
    background-color: #D8E4FF;
}
</style>






<div class="nav">
    <a class="nav-text" , href="about.html">ABOUT</a>
    <a class="nav-text" , href="gallery.html">GALLERY</a>
    <a class="nav-text" , href="my-process.html">MY PROCESS</a>
    <a class="nav-text" , href="contact.html">CONTACT</a>
</div>

<div class="photo">
    <div class="header">
        Hi, I'm Austin Tallent!
    </div>
    <div class="small-header">
        I'm 15 years old and I'm a passonate artist with skills in painting, drawing, animation, vector art and
        more!
    </div>
    <div class="about">
        Hi there!
        <br>
        I'm Austin Tallent, a passionate artist, painter, photographer, animator, and CG Geek based in the dry city
        of Richland, Washington. With a background in
        art, I've honed my expertise in painting and 3D art. Here's a glimpse into my journey:
        <br>
        My journey has taken me through many art related experiences. Whether it's
        recreating my house in 3D, capuring a moment of beauty with a camera, leading the production of a feature
        length movie, or painting with oils, I thrive in anything art related (Except Modern Art).

        Looking ahead, I'm excited about honing my skills in many ways. Whether it's improving my paintings or
        creating the next big movie, I'm
        committed to self improvment.
        <br>
        <br>
        <br>
        <br>
        <a class="button" , href="about.html">TELL ME MORE!</a>
    </div>
</div>
<!-- </div> -->
<div class="white">
    <a class="header-skills">SKILLS</a>
    <div class="container">
        <div class="skill">
            <div class="skill-description">

                <h2>PAINTING</h2>
                <img src="Images/painter.jpg" alt="Painting">
                <p>I am skilled in painting, both in oils and acrylics. I mostly paint landscapes, still lives, and
                    portraits.</p>
                <a href="#" class="learn-more">LEARN MORE!</a>
            </div>
        </div>
        <div class="skill">
            <div class="skill-description">

                <h2>DRAWING</h2>
                <img src="Images/drawing.jpg" alt="Drawing">
                <p>I enjoy drawing with pencils, graphite, or pens. I especially enjoy drawing architecture, nature,
                    or other objects.</p>
                <a href="#" class="learn-more">LEARN MORE!</a>
            </div>
        </div>
        <div class="skill">
            <div class="skill-description">

                <h2>BLENDER 3D</h2>
                <img src="Images/blender.jpeg" alt="Blender">
                <p>I love Blender. I use Blender for many of my projects, and am skilled in 3D modeling, texturing,
                    environment creation, lighting, compositing, video editing, and am getting better at animation.
                </p>
                <a href="#" class="learn-more">LEARN MORE!</a>
            </div>
        </div>
        <div class="skill">
            <div class="skill-description">

                <h2>DIGITAL & VECTOR ART</h2>
                <img src="Images/krita.jpg" alt="Blender">
                <p>I enjoy drawing with pencils, graphite, or pens. I especially enjoy drawing architecture,
                    nature,
                    or other objects.</p>
                <a href="#" class="learn-more">LEARN MORE!</a>
            </div>
        </div>
    </div>
</div>
<!-- </div> -->
<footer class="footer">
    &copy; Austin Tallent 2024 All Rights Reserved
</footer>