<template>
  <div class="landing-translate landing-part">
    <container>
      <p data-aos="fade-down">
        If you wish to translate PrestaShop software in your language, join the
        community of translators on Crowdin!
      </p>
      <custom-button
        link="https://crowdin.com/project/prestashop-official"
        data-aos="fade-down"
        white
      >
        Join the community
      </custom-button>
    </container>
  </div>
</template>

<script>
  export default {}
</script>

<style lang="scss">
  .landing-translate {
    background-color: $secondary;
    padding: 3.2rem 0;
    text-align: center;

    .container {
      max-width: 940px;
    }

    p {
      margin-bottom: 2.4rem;

      @include breakpoint(mobile) {
        text-align: left;
      }
    }
  }
</style>
