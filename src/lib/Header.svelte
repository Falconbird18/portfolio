<header class="header">
    <a href="/about" class="header-text">ABOUT</a>
    <a href="/skills" class="header-text">SKILLS</a>
    <a href="/portfolio" class="header-text">PORTFOLIO</a>
    <a href="/contact" class="header-button">CONTACT</a>
</header>

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
    .header {
      background-color: var(--pale-blue-light);
      padding: 30px;
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
      text-decoration: none;
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
      text-decoration: none;
    }
    .header-button:hover {
      cursor: pointer;
      transform: scale(var(--scale));
      margin-left: 20px;
      margin-right: 20px;
      filter: brightness(var(--hover-brightness));
    }
</style>