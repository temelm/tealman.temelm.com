<script>
  import imgSrcLogo from '../images/favicon.png';
  import Link from '$lib/Link.svelte';
</script>

<nav>
  <div class="nav-brand">
    <Link src={imgSrcLogo} alt="Logo" text="Tealman" />
  </div>
  <div class="nav-links">
    <ul>
      <li>
        <Link href="https://github.com/temelm/tealman" target="_blank" text="GitHub" />
      </li>
      <li>
        <Link
          href="https://chrome.google.com/webstore/detail/tealman/kbppiimbnpoalogphgccdikkjhjolmfn"
          className="button"
          text="Add to Chrome"
        />
      </li>
    </ul>
  </div>
</nav>

<style>
  nav {
    background-color: var(--color-nav);
    border-bottom-left-radius: var(--border-radius);
    border-bottom-right-radius: var(--border-radius);
    display: flex;
    left: 50%;
    max-width: var(--max-width);
    position: fixed;
    top: 0;
    transform: translateX(-50%);
    width: 100%;
    z-index: 1;
  }

  .nav-brand {
    display: flex;
    flex: 1;
    padding: var(--spacing-md);
    padding: var(--spacing-sm);
  }

  .nav-links {
    flex: 2;
    padding: var(--spacing-md);
    padding: var(--spacing-sm);
  }

  .nav-links ul {
    align-items: center;
    display: flex;
    justify-content: flex-end;
    list-style: none;
    margin: 0;
    padding: 0;
  }

  .nav-links ul li:not(:first-child) {
    margin-left: var(--spacing-md);
  }
</style>
