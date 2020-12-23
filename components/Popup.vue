<template>
  <div class="landing-popup" :class="{ hidden: !isShown }" data-aos="fade-left">
    <p class="landing-popup-title">
      How to contribute? ✨
      <svg
        xmlns="http://www.w3.org/2000/svg"
        height="24"
        viewBox="0 0 24 24"
        width="24"
        @click="hide"
      >
        <path d="M0 0h24v24H0z" fill="none" />
        <path
          d="M19 6.41L17.59 5 12 10.59 6.41 5 5 6.41 10.59 12 5 17.59 6.41 19 12 13.41 17.59 19 19 17.59 13.41 12z"
        />
      </svg>
    </p>
    <p class="landing-popup-description">
      You can read the documentation but also contribute to translate, update or
      write the 1.7 user documentation.
    </p>
    <div class="landing-popup-button">
      <custom-button link="https://prestashop.gitbook.io/howtocontribute/">
        Learn more
      </custom-button>
    </div>
  </div>
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
    },
    data() {
      return {
        isShown: true
      }
    },
    methods: {
      hide() {
        this.isShown = false
      }
    }
  })
</script>

<style lang="scss" scoped>
  .landing-popup {
    position: fixed;
    background: #ffffff;
    border-radius: 8px;
    right: 1.6rem;
    top: 50%;
    transform: translateY(-50%);
    box-shadow: 0px 0px 16px 0px rgba(0, 0, 0, 0.15);
    max-width: 347px;
    width: 100%;
    padding: 2rem;
    z-index: 998;
    transition: 0.25s ease-out;

    @include breakpoint(mobile) {
      max-width: calc(100% - 4rem);
      left: 50%;
      transform: translate(-50%, -50%);
    }

    &.hidden {
      transform: translateY(-40%);
      opacity: 0;
      pointer-events: none;
    }

    & &-title {
      font-family: Montserrat;
      font-style: normal;
      font-weight: 600;
      font-size: 2.4rem;
      line-height: 2.9rem;
      color: #011638;
      display: flex;
      align-items: center;
      justify-content: space-between;

      svg {
        cursor: pointer;
        transition: 0.25s ease-out;
        margin-top: 0.2rem;
        width: 2.5rem;
        height: 2.5rem;

        &:hover {
          opacity: 0.6;
        }
      }
    }

    & &-description {
      font-style: normal;
      font-weight: normal;
      font-size: 1.6rem;
      line-height: 2.2rem;
      margin-top: 1.6rem;
    }

    & &-button {
      text-align: right;

      .btn {
        margin: 0;
        margin-top: 1.6rem;
      }
    }
  }
</style>
