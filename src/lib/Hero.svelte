<script>
  import imgSrcLogo from '../images/favicon.png';
  import imgSrcChrome from '../images/chrome.svg';
  import Link from '$lib/Link.svelte';
</script>

<section>
  <div>
    <div>
      <h1>Tealman</h1>
    </div>
    <div>
      <img src={imgSrcLogo} alt="Logo" id="hero-image" />
    </div>
    <div>
      <p>
        Extends Chrome DevTools to display data sent to Adobe Analytics, Google Analytics, Tealium
        Collect and Twitter
      </p>
    </div>
    <div>
      <Link
        href="https://chrome.google.com/webstore/detail/tealman/kbppiimbnpoalogphgccdikkjhjolmfn"
        className="button button-primary"
        src={imgSrcChrome}
        alt="Chrome"
        text="Add to Chrome"
      />
    </div>
  </div>
</section>

<style>
  section {
    margin-top: calc(3 * var(--spacing-lg)); /* 🐒 patch */
  }

  #hero-image {
    height: 12rem;
    width: 12rem;
  }
</style>
