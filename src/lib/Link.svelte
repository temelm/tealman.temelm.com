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
  a {
    align-items: center;
    color: var(--color-link-text);
    display: inline-flex;
    text-decoration: overline;
    text-decoration-color: transparent;
    transition: text-decoration-color 0.2s ease-in-out;
  }

  a:hover {
    color: var(--color-link-text-hover);
    text-decoration-color: var(--color-primary);
  }

  a img {
    height: 2rem;
    width: 2rem;
  }

  a:has(img) span {
    margin-left: var(--spacing-sm);
  }

  a.button {
    background-color: var(--color-button);
    border: 1px solid var(--color-button-border);
    border-radius: var(--border-radius);
    padding: var(--spacing-sm);
    transition: background-color 0.2s ease-in-out;
  }

  a.button:hover {
    background-color: var(--color-button-hover);
    text-decoration: none;
    color: white;
  }

  a.button.button-primary {
    background-color: var(--color-primary);
    border: none;
    color: white;
    font-weight: var(--font-weight-bold);
    padding: var(--spacing-md);
    transition: transform 0.2s ease-in-out;
  }

  a.button.button-primary:hover {
    transform: scale(1.02);
  }

  a.button.button-primary img {
    height: 4rem;
    width: 4rem;
  }

  a.button.button-primary:has(img) span {
    margin-left: var(--spacing-md);
  }
</style>
