<template>
  <div id="app">
    <headerSite/>
    <mainSite/>
    <footerSite/>
  </div>
</template>

<script>
import HeaderSite from './components/headerSite.vue'
import mainSite from './components/mainSite.vue'
import footerSite from './components/footerSite.vue'


export default {
  name: 'App',
  components: {
    HeaderSite,
    mainSite,
    footerSite,
  }
}
</script>

<style lang="scss">
@import '~@/assets/scss/variables.scss';
</style>
