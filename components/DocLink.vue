<template>
  <a class="doc-link" :href="link" target="_blank" rel="noreferrer">
    <slot></slot>
  </a>
</template>

<script>
  import Vue from 'vue'

  export default Vue.extend({
    name: 'Header',
    props: {
      link: {
        type: String,
        default: '#'
      }
    }
  })
</script>

<style lang="scss" scoped>
  .doc-link {
    width: 296px;
    background: #ffffff;
    border: 1px solid #d2d2d2;
    box-sizing: border-box;
    border-radius: 4px;
    padding: 1.6rem;
    margin: 0.8rem;
    display: block;
    padding-left: 4.9rem;
    position: relative;
    transition: 0.25s ease-out;
    min-height: 7.8rem;

    &:hover {
      box-shadow: 0px 4px 16px rgba(0, 0, 0, 0.1);
    }

    img {
      position: absolute;
      left: 1.6rem;
      top: 1.6rem;
    }

    p {
      font-style: normal;
      font-weight: normal;
      font-size: 16px;
      line-height: 22px;
      color: #353535;
      text-align: left;
    }
  }
</style>
