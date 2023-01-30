<script>
  import Nav from './Nav.svelte';
</script>

<Nav />

<slot />

<style>
  :global(:root) {
    --border-radius: 0.125rem;
    --color-background: white; /* @todo: review */
    --color-link-text: #333333;
    --color-link-text-hover: black;
    --color-text: #333333;
    --font-family: 'Roboto Mono', monospace;
    --font-weight: 300;
    --font-weight-bold: 500;
    --max-width: 48rem;
    --spacing-lg: 2rem;
    --spacing-md: 1rem;
    --spacing-sm: 0.5rem;
  }

  :global(body) {
    background-color: #e8e8e8;
    color: var(--color-text);
    font-family: var(--font-family);
    font-weight: var(--font-weight);
    margin: 0 auto;
    max-width: var(--max-width);
  }

  :global(section) {
    background-color: var(--color-background);
    border-radius: var(--border-radius);
    margin-bottom: var(--spacing-lg);
    padding: var(--spacing-lg) var(--spacing-md);
    text-align: center;
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
    font-weight: var(--font-weight-bold);
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
</style>
