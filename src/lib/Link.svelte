<script>
  export let href = '#';
  export let target = undefined;
  export let className = undefined;
  export let src = undefined;
  export let alt = undefined;
  export let text = undefined;
</script>

<a {href} {target} class={className}>
  {#if src}
    <img {src} {alt} />
  {/if}
  {#if text}
    <span>{text}</span>
  {/if}
</a>

<style>
  :root {
    --color-button: lightslategray;
    --color-button-border: slategray;
    --color-button-border-hover: var(--color-primary);
    --color-button-hover: var(--color-primary);
    --color-button-text: white;
    --color-link-text: #333333;
    --color-link-text-hover: black;
  }
  a {
    align-items: center;
    color: var(--color-link-text);
    display: inline-flex;
    text-decoration: overline;
    text-decoration-color: transparent;
    transition: color 0.2s ease-in-out, text-decoration-color 0.2s ease-in-out;
  }

  a:hover {
    color: var(--color-link-text-hover);
    text-decoration-color: var(--color-link-text-hover);
  }

  a img {
    height: 2rem;
    width: 2rem;
  }

  a:has(img) span {
    margin-left: var(--spacing-small);
  }

  a.button {
    background-color: var(--color-button);
    border: 1px solid var(--color-button-border);
    border-radius: var(--border-radius);
    color: var(--color-button-text);
    padding: var(--spacing-small);
    text-align: center;
    transition: background-color 0.2s ease-in-out;
  }

  a.button:hover {
    background-color: var(--color-button-hover);
    border-color: var(--color-button-border-hover);
    text-decoration: none;
  }

  a.button.button-primary {
    background-color: var(--color-primary);
    border: none;
    font-weight: var(--font-weight-bold);
    padding: var(--spacing-medium);
    transition: transform 0.2s ease-in-out;
  }

  a.button.button-primary:hover {
    transform: scale(1.02);
  }
</style>
