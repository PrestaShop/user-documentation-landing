<template>
  <div class="landing-previous">
    <container>
      <h2>User documentations for previous versions of PrestaShop</h2>
      <p>
        If you wish to read documentations of versions prior to PrestaShop 1.4,
        send an email to
        <a
          href="mailto:documentation@prestashop.com"
          target="_blank"
          rel="noreferrer"
        >
          documentation@prestashop.com.
        </a>
      </p>

      <ul class="landing-previous-list">
        <li>
          <doc-link
            link="https://prestashop.gitbook.io/prestashop-1-6-documentations/"
            data-aos="fade-down"
          >
            <img src="mini-ps.png" alt="PrestaShop Logo Mini" />
            <p>PrestaShop 1.6 Documentation</p>
          </doc-link>
        </li>
        <li>
          <doc-link
            link="https://prestashop.gitbook.io/prestashop-1-5-documentations/"
            data-aos="fade-down"
            data-aos-delay="100"
          >
            <img src="mini-ps.png" alt="PrestaShop Logo Mini" />
            <p>PrestaShop 1.5 Documentation</p>
          </doc-link>
        </li>
        <li>
          <doc-link
            link="https://prestashop.gitbook.io/prestashop-1-4-documentations/"
            data-aos="fade-down"
            data-aos-delay="200"
          >
            <img src="mini-ps.png" alt="PrestaShop Logo Mini" />
            <p>PrestaShop 1.4 Documentation</p>
          </doc-link>
        </li>
      </ul>
    </container>
  </div>
</template>

<script>
  export default {}
</script>

<style lang="scss">
  .landing-previous {
    padding: 6.4rem 0;
    text-align: center;

    .container {
      max-width: 940px;
    }

    h2 {
      margin-bottom: 3.2rem;
    }

    ul {
      display: flex;
      flex-wrap: wrap;
      align-items: flex-start;
      margin-top: 0.8rem;
    }
  }
</style>
