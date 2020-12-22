<template>
  <a
    class="btn"
    :class="{ 'btn-outline': outline, 'btn-white': white }"
    :href="link"
    :target="target"
    rel="noreferrer"
  >
    <slot></slot>
  </a>
</template>

<script>
  import Vue from 'vue'

  export default Vue.extend({
    name: 'Header',
    props: {
      outline: {
        type: Boolean,
        default: false
      },
      white: {
        type: Boolean,
        default: false
      },
      link: {
        type: String,
        default: '#'
      },
      target: {
        type: String,
        default: '_blank'
      }
    }
  })
</script>

<style lang="scss" scoped>
  .btn {
    font-style: normal;
    font-weight: 600;
    font-size: 1.6rem;
    line-height: 2.2rem;
    text-align: center;
    color: #353535;
    transition: 0.25s ease-out;
    margin: 0 1.6rem;
    display: inline-block;

    &:hover {
      opacity: 0.8;
    }

    &:not(.btn-outline) {
      padding: 0.8rem 1.6rem;
      border-radius: 0.4rem;
      color: #fff;
      background-color: $primary;
    }

    &.btn-white {
      background-color: #fff;
      color: $link-color;
    }
  }
</style>
