<template>
  <div class="landing-improve landing-part">
    <container>
      <div
        class="landing-improve-left"
        data-aos="fade-right"
        data-aos-anchor-placement="center-bottom"
      >
        <h2>Improve the documentation ✨</h2>
        <p>
          Just like PrestaShop itself, the documentation is open to everyone for
          suggestions, ideas, and modifications! Anyone is welcome and even
          encouraged, to contribute to translate, update, or write the 1.7 user
          documentation.
        </p>

        <custom-button link="https://prestashop.gitbook.io/howtocontribute/">
          Contribute
        </custom-button>
      </div>
      <div
        class="landing-improve-right"
        data-aos="fade-left"
        data-aos-anchor-placement="center-bottom"
      >
        <img src="illustration.svg" alt="Improve PrestaShop" />
      </div>
    </container>
  </div>
</template>

<script>
  export default {}
</script>

<style lang="scss">
  .landing-improve {
    padding: 8rem 0;
    position: relative;

    @include breakpoint(mobile) {
      padding: 2.8rem 2rem;
      padding-bottom: 10rem !important;
    }

    & &-left {
      max-width: 520px;
      width: 100%;

      .btn {
        @include breakpoint(mobile) {
          position: absolute;
          bottom: 3.2rem;
          left: 50%;
          transform: translateX(-50%);
        }
      }
    }

    & &-right {
      max-width: 100%;
      width: 47.5rem;

      img {
        max-width: 100%;
      }
    }

    h2 {
      margin-bottom: 3.1rem;
    }

    .container {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
    }

    p {
      padding-right: 4rem;
      text-align: justify;
    }

    .btn {
      &:not(.btn-outline) {
        display: inline-block;
        margin: 0;
        margin-top: 3.1rem;
      }
    }
  }
</style>
