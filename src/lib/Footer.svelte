<script>
  import Link from './Link.svelte';
  import GitHubIcon from './GitHubIcon.svelte';

  const copyrightYear = new Date().getFullYear();
</script>

<footer>
  <div class="social">
    <Link href="//github.com/temelm/tealman" rel="external" hasSvgIcon="true">
      <GitHubIcon />
    </Link>
  </div>
  <div class="copyright">
    <span role="img" aria-label="Copyright">©️</span>
    <span>
      {copyrightYear}
      <Link href="//www.temelm.com" text="Mustafa Temel" />
    </span>
  </div>
</footer>

<style>
  footer {
    font-size: 0.75rem;
    opacity: 0.75;
    padding: var(--spacing-lg);
    text-align: center;
  }

  .social {
    column-gap: var(--spacing-md);
    display: flex;
    justify-content: center;
    margin-bottom: var(--spacing-md);
  }

  @media (prefers-color-scheme: dark) {
    footer {
      opacity: 0.5;
    }
  }
</style>