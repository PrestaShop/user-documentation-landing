<template>
  <div class="landing-docs">
    <container>
      <p>Choose your language among the 6 available languages:</p>

      <ul class="landing-previous-list">
        <li>
          <doc-link
            link="https://prestashop.gitbook.io/english-documentation-for-prestashop-1-7/"
          >
            <img src="us.png" alt="PrestaShop Logo Mini" />
            <p>English documentation for PrestaShop 1.7</p>
          </doc-link>
        </li>
        <li>
          <doc-link
            link="https://prestashop.gitbook.io/documentation-en-francais-pour-prestashop-1-7/"
          >
            <img src="fr.png" alt="PrestaShop Logo Mini" />
            <p>Documentation en français pour PrestaShop 1.7</p>
          </doc-link>
        </li>
        <li>
          <doc-link
            link="https://prestashop.gitbook.io/documentacion-espanola-para-prestashop-1-7/"
          >
            <img src="es.png" alt="PrestaShop Logo Mini" />
            <p>Documentación española para PrestaShop 1.7</p>
          </doc-link>
        </li>
        <li>
          <doc-link
            link="https://prestashop.gitbook.io/documentazione-italiana-per-prestashop-1-7/"
          >
            <img src="it.png" alt="PrestaShop Logo Mini" />
            <p>Documentazione italiana per PrestaShop 1.7</p>
          </doc-link>
        </li>
        <li>
          <doc-link
            link="https://prestashop.gitbook.io/nederlandse-documentatie-voor-prestashop-1-7/"
          >
            <img src="ne.png" alt="PrestaShop Logo Mini" />
            <p>Nederlandse documentatie voor PrestaShop 1.7</p>
          </doc-link>
        </li>
        <li>
          <doc-link
            link="https://app.gitbook.com/@prestashop/s/asnad-farsy-bray-prestashop-1-7/"
          >
            <img src="fa.png" alt="PrestaShop Logo Mini" />
            <p>Farsi PrestaShop 1.7</p>
          </doc-link>
        </li>
      </ul>

      <p>
        Each documentation is synchronized with a repository on GitHub. Both
        interfaces are open to contributions. Click on your language to visit
        the corresponding repository:
        <span class="lang-links">
          <a
            href="https://github.com/PrestaShop/user-documentation-en"
            target="_blank"
            rel="noreferrer"
          >
            English
          </a>
          ,
          <a
            href="https://github.com/PrestaShop/user-documentation-fr"
            target="_blank"
            rel="noreferrer"
          >
            French
          </a>
          ,
          <a
            href="https://github.com/PrestaShop/user-documentation-es"
            target="_blank"
            rel="noreferrer"
          >
            Spanish
          </a>
          ,
          <a
            href="https://github.com/PrestaShop/user-documentation-it"
            target="_blank"
            rel="noreferrer"
          >
            Italian
          </a>
          ,
          <a
            href="https://github.com/PrestaShop/user-documentation-nl"
            target="_blank"
            rel="noreferrer"
          >
            Dutch
          </a>
          ,
          <a
            href="https://github.com/PrestaShop/user-documentation-fa"
            target="_blank"
            rel="noreferrer"
          >
            Farsi
          </a>
          .
        </span>
      </p>
      <div class="lang-link-responsive">
        <a
          href="https://github.com/PrestaShop/user-documentation-en"
          target="_blank"
          rel="noreferrer"
        >
          🇺🇸
        </a>
        <a
          href="https://github.com/PrestaShop/user-documentation-fr"
          target="_blank"
          rel="noreferrer"
        >
          🇫🇷
        </a>
        <a
          href="https://github.com/PrestaShop/user-documentation-es"
          target="_blank"
          rel="noreferrer"
        >
          🇪🇸
        </a>
        <a
          href="https://github.com/PrestaShop/user-documentation-it"
          target="_blank"
          rel="noreferrer"
        >
          🇮🇹
        </a>
        <a
          href="https://github.com/PrestaShop/user-documentation-nl"
          target="_blank"
          rel="noreferrer"
        >
          🇩🇪
        </a>
        <a
          href="https://github.com/PrestaShop/user-documentation-fa"
          target="_blank"
          rel="noreferrer"
        >
          🇮🇷
        </a>
      </div>
    </container>
  </div>
</template>

<script>
  export default {}
</script>

<style lang="scss">
  .landing-docs {
    padding: 3.2rem 0;
    text-align: center;

    @include breakpoint(mobile) {
      padding: 2rem;
      text-align: left;
    }

    .container {
      max-width: 940px;

      .lang-link-responsive {
        display: none;

        @include breakpoint(mobile) {
          display: flex;
          align-items: center;
          justify-content: space-around;
          margin-top: 1.6rem;

          a {
            font-size: 3.2rem;
          }
        }
      }

      > p {
        &:last-of-type {
          margin-top: 2rem;
        }

        @include breakpoint(mobile) {
          .lang-links {
            display: none;
          }
        }
      }
    }

    ul {
      display: flex;
      flex-wrap: wrap;
      align-items: flex-start;
      margin-top: 0.8rem;

      > li {
        @include breakpoint(mobile) {
          width: 100%;
        }
      }
    }
  }
</style>
