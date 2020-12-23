<template>
  <layout>
    <template #header>
      <Header />
    </template>

    <intro />
    <docs />
    <improve />
    <translate />

    <popup />

    <template #footer>
      <PreviousVersions />
    </template>
  </layout>
</template>

<script>
  export default {}
</script>

<style lang="scss">
  html,
  body,
  textarea {
    font-family: $font-family;
  }

  html {
    font-size: 10px;
  }

  body {
    font-size: 1.6rem;
    min-height: 100vh;
    padding-top: 7rem;
  }

  body,
  a,
  span,
  strong {
    color: #011638;
    text-decoration: none;
  }

  p {
    color: #7a7a7a;
  }

  a {
    color: $link-color;
  }

  h1,
  h2,
  h3,
  h4 {
    font-size: 3.2rem;
    font-family: Montserrat, sans-serif;
    font-weight: 600;

    @include breakpoint(mobile) {
      font-size: 2.4rem;
    }
  }

  ul {
    padding: 0;
    margin: 0;

    li {
      list-style-type: none;
    }
  }

  p {
    a {
      position: relative;

      &::after {
        content: '';
        height: 0.1rem;
        background: $link-color;
        width: 0;
        position: absolute;
        bottom: 0;
        left: 0;
        transition: 0.25s ease-out;
      }

      &:hover {
        &::after {
          width: 100%;
        }
      }
    }
  }

  .landing-part {
    @include breakpoint(mobile) {
      padding: 2rem !important;
    }
  }
</style>
