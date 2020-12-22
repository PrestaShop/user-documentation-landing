<template>
  <div class="landing-header">
    <container>
      <logo />

      <div class="landing-header-right">
        <custom-button link="#" outline>Sign up</custom-button>
        <custom-button link="#">Log in</custom-button>
      </div>
    </container>
  </div>
</template>

<script>
  import Vue from 'vue'

  export default Vue.extend({
    name: 'Header'
  })
</script>

<style lang="scss">
  .landing-header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 1.6rem;
    box-shadow: 0px 8px 16px rgba(0, 0, 0, 0.1);
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    background-color: #fff;
    z-index: 999;

    .container {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
    }

    & &-right {
      display: flex;
      flex-wrap: wrap;
      align-items: center;
    }
  }
</style>
