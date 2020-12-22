<template>
  <div class="landing-docs">
    <container>
      <p>Choose your language among the 6 available languages:</p>

      <ul class="landing-previous-list">
        <li>
          <doc-link link="#">
            <img src="us.png" alt="PrestaShop Logo Mini" />
            <p>English documentation for PrestaShop 1.7</p>
          </doc-link>
        </li>
        <li>
          <doc-link link="#">
            <img src="fr.png" alt="PrestaShop Logo Mini" />
            <p>Documentation en français pour PrestaShop 1.7</p>
          </doc-link>
        </li>
        <li>
          <doc-link link="#">
            <img src="es.png" alt="PrestaShop Logo Mini" />
            <p>Documentación española para PrestaShop 1.7</p>
          </doc-link>
        </li>
        <li>
          <doc-link link="#">
            <img src="it.png" alt="PrestaShop Logo Mini" />
            <p>Documentazione italiana per PrestaShop 1.7</p>
          </doc-link>
        </li>
        <li>
          <doc-link link="#">
            <img src="ne.png" alt="PrestaShop Logo Mini" />
            <p>Nederlandse documentatie voor PrestaShop 1.7</p>
          </doc-link>
        </li>
        <li>
          <doc-link link="#">
            <img src="fa.png" alt="PrestaShop Logo Mini" />
            <p>Farsi PrestaShop 1.7</p>
          </doc-link>
        </li>
      </ul>

      <p>
        Each documentation is synchronized with a repository on GitHub. Both
        interfaces are open to contributions. Click on your language to visit
        the corresponding repository:
        <a href="#">English</a>
        ,
        <a href="#">French</a>
        ,
        <a href="#">Spanish</a>
        ,
        <a href="#">Italian</a>
        ,
        <a href="#">Dutch</a>
        ,
        <a href="#">Farsi</a>
        .
      </p>
    </container>
  </div>
</template>

<script>
  export default {}
</script>

<style lang="scss">
  .landing-docs {
    padding: 3.2rem 0;
    text-align: center;

    .container {
      max-width: 940px;

      > p {
        &:last-of-type {
          margin-top: 2rem;
        }
      }
    }

    ul {
      display: flex;
      flex-wrap: wrap;
      align-items: flex-start;
      margin-top: 0.8rem;
    }
  }
</style>
