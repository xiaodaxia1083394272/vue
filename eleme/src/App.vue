<template>
  <div class="app">
    <!-- <img src="./assets/logo.png"> -->
    <router-view/>
    <FooterGuide></FooterGuide>
  </div>
</template>

<script>

import FooterGuide from './components/FooterGuide.vue'

export default {
  components: {
      FooterGuide
   }
}
</script>

<style lang="stylus" rel="stylesheet/stylus">
 .app 
   width 100%
   height 100%
   background width 
</style>
