<template>
  <div id="app">
    <Header />
  </div>
</template>

<script>
import Header from '@/components/Header'

export default {
  name: 'App',
  components: {
    Header,

  }
}
</script>

<style lang="scss">
  // GENERAL
  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }

  body {
    font-family: 'Source Sans Pro', sans-serif;
  }

  li {
    list-style: none;
    a {
      text-decoration: none;
      color: currentColor;
    }
  }


  // UTILITIES
  .container {
    max-width: 1200px;
    margin: 0 auto;
  }
</style>
