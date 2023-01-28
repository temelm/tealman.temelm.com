<script>
  import imgSrcLogo from '../images/favicon.png';
  import imgSrcChrome from '../images/chrome.svg';
</script>

<section>
  <div class="grid">
    <div>
      <h1>Tealman</h1>
    </div>
    <div>
      <img src={imgSrcLogo} alt="Logo" id="hero-image">
    </div>
    <div>
      <p>Extends Chrome DevTools to display data sent to Adobe Analytics, Google Analytics, Tealium Collect and Twitter</p>
    </div>
    <div>
      <a href="https://chrome.google.com/webstore/detail/tealman/kbppiimbnpoalogphgccdikkjhjolmfn" class="linkbutton">
        <img src={imgSrcChrome} alt="Chrome">
        Add to Chrome
      </a>
    </div>
  </div>
</section>

<style>
  section {
    margin-top: calc(3 * var(--spacing-lg)); /* 🐒 patch */
  }

  .grid {
    display: grid;
    row-gap: var(--spacing-lg);
  }

  #hero-image {
    height: 12rem;
    width: 12rem;
  }
</style>