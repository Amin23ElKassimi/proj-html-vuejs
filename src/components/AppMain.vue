<!-- HTML & Vue JS-->
<template lang="">
    <main>
      <!-- Section 01: Audio Book-->
      <section01/>
      <!-- Section 02: What The Critics Say-->
      <section02/>
      <!-- Section 03: Upcomin Events-->
      <section03/>
      <!-- Section 04: Subscribe To My Newsletter-->
      <section04/>
      <!-- Section 05: Dig A Little Deeper Into Damon Vaughn -->
      <section05/>
      <!-- Section 06: Resent Articles-->
      <section06/>
      </main>
</template>

<!-- Script Code -->
<script>
  // Impor Components
  import section01 from './section01.vue';
  import section02 from './section02.vue';
  import section03 from './section03.vue';
  import section04 from './section04.vue';
  import section05 from './section05.vue';
  import section06 from './section06.vue';


  export default {



    components: {
      section01,
      section02,
      section03,
      section04,
      section05,
      section06,
    }


  }

</script>


<!-- SASS Code -->
<style lang="scss" scoped>
  @use '../styles/general.scss' as *;
  @use '../styles/partials/variables.scss' as *;
  @use '../styles/partials/mixins.scss' as *;



    .audio-book {
      background-color: $beji-bg;
    }

  


    // rooles
    .text-uppercase{
      text-transform: uppercase;
    }


    .danger-color{
        color: $danger-color;
        text-transform: uppercase;
    }

    .text-gray{
      color: rgb(150, 147, 147);
    }

    
    .beji-bg{
      background-color:$beji-bg;
    }

    // Margin Padding Border



</style>