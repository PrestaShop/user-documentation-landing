<template>
  <div class="landing-improve">
    <container>
      <div class="landing-improve-left">
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
      <div class="landing-improve-right">
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

    & &-left {
      max-width: 520px;
      width: 100%;
    }

    & &-right {
      max-width: 100%;
      width: 47.5rem;
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
