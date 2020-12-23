<template>
  <div class="landing">
    <header>
      <slot name="header"></slot>
    </header>

    <main>
      <slot></slot>
    </main>

    <footer>
      <slot name="footer"></slot>
    </footer>
  </div>
</template>

<script>
  import Vue from 'vue'

  export default Vue.extend({
    name: 'Layout'
  })
</script>
