<template>
  <main class="main-layout full">
      <app-header/>
      <hero/>
      <about/>
  </main>
</template>

<script>
import appHeader from './components/app-header.vue';
import twoPartResponsive from './components/two-part-responsive.vue';
import hero from './components/hero.vue';
import about from './components/about.vue'
  export default {
    
    components: {
      appHeader,
      twoPartResponsive,
      hero,
      about
    }
  }
</script>

<style lang="scss" scoped>

</style>