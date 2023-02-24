<script>
  import imgSrcLogo from '../assets/favicon.png';
  
  import Link from './Link.svelte';
  import ChromeIcon from './ChromeIcon.svelte';
</script>

<header>
  <nav>
    <Link src={imgSrcLogo} alt="Tealman" />
    <ul>
      <li>
        <Link
          href="//chrome.google.com/webstore/detail/tealman/kbppiimbnpoalogphgccdikkjhjolmfn"
          rel="external"
          className="button"
          hasSvgIcon="true"
          text="Add to Chrome"
        >
          <ChromeIcon width="1.25rem" />
        </Link>
      </li>
    </ul>
  </nav>
</header>

<style>
  header {
    --header-color: rgb(245, 245, 245, 0.95);
    
    background-color: var(--header-color);
    position: sticky;
    top: 0;
    width: 100%;
    z-index: 1;
  }

  header nav {
    align-items: center;
    display: flex;
    justify-content: space-between;
    margin: 0 auto;
    max-width: var(--max-width);
    padding: var(--spacing-md);
  }

  header nav ul {
    list-style: none;
  }

  header nav ul li {
    display: inline-block;
    margin-left: var(--spacing-sm);
  }
  
  header nav ul li:first-child {
    margin-left: 0;
  }

  @media (prefers-color-scheme: dark) {
    header {
      --header-color: rgb(64, 64, 64, 0.95);
    }
  }
</style>