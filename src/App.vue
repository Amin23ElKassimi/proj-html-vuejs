<!-- HTML Code -->
<template lang="">
  <!-- Component Header -->
  <AppHeader/>
  <!-- Component Main -->
  <AppMain/>
  <!-- Component Footer -->
  <AppFooter/>
</template>

<!-- Script Code -->
<script>
  import AppHeader from './components/AppHeader.vue';
  import AppMain from './components/AppMain.vue';
  import AppFooter from './components/AppFooter.vue';


  export default {
    name: 'App',
    components: {
      AppHeader,
      AppMain,
      AppFooter
    }
    
  }
</script>


<!-- SASS Code -->
<style lang="scss">
  @use './styles/general.scss' as *;

  
</style>
 