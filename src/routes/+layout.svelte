<script>
  import imgSrcLogo from '../images/favicon.png'
</script>

<nav>
  <ul>
    <li>
      <a href="/">
        <img src={imgSrcLogo} alt="Logo">
        Tealman
      </a>
    </li>
  </ul>
</nav>

<slot></slot>

<style>
  :global(:root) {
    --border-radius: 0.125rem;
    --color-background: white;
    --color-link-text: #333333;
    --color-link-text-hover: black;
    --color-text: #333333;
    --font-family: 'Roboto Mono', monospace;
    --font-weight: 300;
    --font-weight-bold: 300;
    --max-width: 48rem;
    --spacing-lg: 2rem;
    --spacing-md: 1rem;
    --spacing-sm: 0.5rem;
  }

  :global(body) {
    background-color: var(--color-background);
    color: var(--color-text);
    font-family: var(--font-family);
    font-weight: var(--font-weight);
    margin: 0 auto;
    max-width: var(--max-width);
  }

  :global(section) {
    padding-left: var(--spacing-md);
    padding-right: var(--spacing-md);
    margin-top: calc(3 * var(--spacing-lg)); /* 🐒 patch */
  }

  :global(h1) {
    font-size: xx-large;
    margin: 0;
  }

  :global(p) {
    margin: 0;
  }

  :global(.linkbutton) {
    align-items: center;
    background-color: teal;
    border-radius: var(--border-radius);
    color: white;
    display: inline-flex;
    padding: var(--spacing-md);
    text-decoration: none;
    transition: all 0.1s linear;
  }

  :global(.linkbutton:hover) {
    transform: scale(1.05);
  }

  :global(.linkbutton img) {
    height: 2rem;
    margin-right: var(--spacing-md);
    width: 2rem;
  }

  nav {
    background-color: #e0e0e0;
    border-bottom-left-radius: var(--border-radius);
    border-bottom-right-radius: var(--border-radius);
    max-width: var(--max-width);
    position: fixed;
    top: 0;
    width: 100%;
    z-index: 1;
  }

  nav ul {
    display: flex;
    list-style: none;
    margin: 0;
    padding: var(--spacing-md);
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