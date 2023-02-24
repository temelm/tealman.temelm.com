<script>
  import imgSrcLogo from '../assets/favicon.png';
  import Link from './Link.svelte';
  import ChromeIcon from './ChromeIcon.svelte';
</script>

<section>
  <div>
    <h1>Tealman</h1>
  </div>
  <div class="hero-image">
    <img src={imgSrcLogo} alt="Logo" />
  </div>
  <div>
    <p>
      Extends Chrome DevTools to display data sent to Adobe Analytics, Google Analytics, Tealium
      Collect and Twitter
    </p>
  </div>
  <div>
    <Link
      href="//chrome.google.com/webstore/detail/tealman/kbppiimbnpoalogphgccdikkjhjolmfn"
      rel="external"
      className="button"
      hasSvgIcon="true"
      text="Add to Chrome"
    >
      <ChromeIcon width="1.25rem" />
    </Link>
  </div>
</section>

<style>
  section {
    display: grid;
    row-gap: 2rem;
  }

  h1 {
    margin-bottom: 0;
  }

  .hero-image {
    display: grid;
    place-items: center;
  }

  img {
    max-width: 256px;
  }

  p {
    font-size: 1.25rem;
    line-height: 1.25;
  }
</style>