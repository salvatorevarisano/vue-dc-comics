<template>
  <div id="app">
    <Header />
    <Hero/>
    <Series/>
    <Footer />

  </div>
</template>

<script>
import Header from '@/components/Header'
import Hero from '@/components/Hero'
import Series from '@/components/Series'
import Footer from '@/components/Footer'


export default {
  name: 'App',
  components: {
    Header,
    Hero,
    Series,
    Footer,

  },

}
</script>

<style lang="scss">
  @import '@/style/general.scss';
  @import '@/style/layout';

</style>
