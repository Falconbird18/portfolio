      <footer class="footer">
        <span class="copyright"
          >&copy 2024 Austin Tallent All Rights Reserved</span
        >
        <br />
        <div class="footer-text">
          <i
            class="fa-brands fa-artstation"
            href="https://www.artstation.com/austin_tallent"
          ></i>
        </div>
        <div class="footer-text">
          <i class="fa-solid fa-envelope"></i>
        </div>
      </footer>

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
  .footer {
    background-color: var(--pale-blue-light);
    padding: 30px;
    text-decoration: none;
    border-radius: var(--radius) var(--radius) 0px 0px;
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
</style>
