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
  }

  ul {
    padding: 0;
    margin: 0;

    li {
      list-style-type: none;
    }
  }
</style>
