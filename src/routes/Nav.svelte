<script>
  import imgSrcLogo from '../images/favicon.png';
</script>

<nav>
  <ul>
    <li>
      <a href="#">
        <img src={imgSrcLogo} alt="Logo" />
        Tealman
      </a>
    </li>
    <li>
      <a href="#features">Features</a>
    </li>
  </ul>
</nav>

<style>
  nav {
    background-color: #f8f8f8;
    border-bottom-left-radius: var(--border-radius);
    border-bottom-right-radius: var(--border-radius);
    max-width: var(--max-width);
    position: fixed;
    top: 0;
    width: 100%;
    z-index: 1;
  }

  nav ul {
    align-items: center;
    display: flex;
    list-style: none;
    margin: 0;
    padding: var(--spacing-md);
  }

  nav ul li {
    flex: 1;
    text-align: right;
  }

  nav ul li a {
    color: var(--color-link-text);
    text-decoration: none;
    transition: all 0.1s linear;
  }

  nav ul li a:hover {
    color: var(--color-link-text-hover);
    font-size: 1.05rem;
    text-decoration: underline;
  }

  nav ul li a:has(img) {
    align-items: center;
    display: flex;
  }

  nav ul li a img {
    height: 2rem;
    margin-right: var(--spacing-sm);
    width: 2rem;
  }
</style>
