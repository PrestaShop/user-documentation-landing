<template>
  <div class="landing-intro landing-part">
    <container>
      <h1>Welcome to the PrestaShop documentation site</h1>
      <p>
        In this user documentation, you will discover how to create, maintain,
        and make the most of an online store built using the
        <a
          href="https://www.prestashop.com/en"
          target="_blank"
          rel="noreferrer"
        >
          PrestaShop™ e-commerce solution.
        </a>
      </p>
    </container>
  </div>
</template>

<script>
  export default {}
</script>

<style lang="scss">
  .landing-intro {
    background-color: $secondary;
    padding: 6.4rem 0;
    text-align: center;

    @include breakpoint(mobile) {
      text-align: left;
    }

    .container {
      max-width: 940px;
    }

    h1 {
      margin-bottom: 3.2rem;
      font-size: 3.2rem;

      @include breakpoint(mobile) {
        font-size: 2.4rem;
        margin-bottom: 1.6rem;
      }
    }

    a {
      display: inline-block;
    }
  }
</style>
