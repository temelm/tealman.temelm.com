<script>
  import Link from '$lib/Link.svelte';
  const copyrightYear = new Date().getFullYear();
</script>

<footer>
  <span role="img" aria-label="Copyright">©️</span>
  <span>2019-{copyrightYear}</span>
  <Link href="https://www.temelm.com" text="Mustafa Temel" />
</footer>

<style>
  footer {
    margin-bottom: var(--spacing-large);
    text-align: center;
  }
</style>
