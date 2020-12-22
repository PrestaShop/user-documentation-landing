<template>
  <div class="landing-intro">
    <container>
      <h1>Welcome to the PrestaShop documentation site</h1>
      <p>
        In this user documentation, you will discover how to create, maintain,
        and make the most of an online store built using the
        <a href="https://www.prestashop.com/en" target="_blank">
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

    .container {
      max-width: 940px;
    }

    h1 {
      margin-bottom: 3.2rem;
      font-size: 3.2rem;
    }

    a {
      display: block;
    }
  }
</style>
