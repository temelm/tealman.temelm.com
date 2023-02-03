<script>
  import imgSrcLogo from '../images/favicon.png';
  import Link from '$lib/Link.svelte';
</script>

<header>
  <nav>
    <Link src={imgSrcLogo} alt="Logo" text="Tealman" />
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
  </nav>
</header>

<style>
  header {
    background-color: #f8f8f8;
    border-bottom-left-radius: var(--border-radius);
    border-bottom-right-radius: var(--border-radius);
    margin-bottom: 32px;
    max-width: var(--max-width);
    position: sticky;
    top: 0;
    width: 100%;
    z-index: 1;
  }

  header nav {
    align-items: center;
    display: flex;
    justify-content: space-between;
    padding: var(--spacing-medium);
  }

  header nav ul {
    list-style: none;
  }

  header nav ul li {
    display: inline-block;
    margin-left: var(--spacing-medium);
  }

  header nav ul li:first-child {
    margin-left: 0;
  }
</style>
