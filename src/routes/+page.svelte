<script>
  import imgSrcLogo from '../images/favicon.png';
  import imgSrcChrome from '../images/chrome.svg';
</script>

<section>
  <h1>Tealman</h1>
  <img src={imgSrcLogo} alt="Logo">
  <p>Extends Chrome DevTools to display data sent to Adobe Analytics, Google Analytics, Tealium Collect and Twitter.</p>
  <a href="https://chrome.google.com/webstore/detail/tealman/kbppiimbnpoalogphgccdikkjhjolmfn" class="linkbutton">
    <img src={imgSrcChrome} alt="Chrome">
    Add to Chrome
  </a>
</section>

<style>
  section {
    text-align: center;
  }

  section > * {
    margin-bottom: var(--spacing-lg);
  }

  section > img {
    height: 8rem;
    width: 8rem;
  }
</style>