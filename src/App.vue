<!-- HTML Code -->
<template lang="">
  <!-- Component Header -->
  <AppHeader :links="navLinks"/>
  <!-- Component Main -->
  <AppMain/>
  <!-- Component Footer -->
  <AppFooter/>
</template>

<!-- Script Code -->
<script>
  // Impor Components
  import AppHeader from './components/AppHeader.vue';
  import AppMain from './components/AppMain.vue';
  import AppFooter from './components/AppFooter.vue';


  export default {
    name: 'App',
    components: {
      AppHeader,
      AppMain,
      AppFooter
    },

    // Variabili
    data() {
        return {
            navLinks: [
                {
                    content: 'Home',
                    url: '#',
                    active: false,
                },
                {
                    content: 'About Me',
                    url: '#',
                    active: false,
                },
                {
                    content: 'Testimonials',
                    url: '#',
                    active: false,
                },
                {
                    content: 'My Blog',
                    url: '#',
                    active: false,
                },
                {
                    content: 'Meetsup',
                    url: '#',
                    active: false,
                },
                {
                    content: 'shop',
                    url: '#',
                    active: false,
                },
                {
                    content: 'Contact Me',
                    url: '#',
                    active: false,
                },
                {
                    content: 'Carrello',
                    url: '#',
                    active: false,
                },
            ],
        }
     },

    
  }
</script>


<!-- SASS Code -->
<style lang="scss">
  @use './styles/general.scss' as *;

  
</style>
 