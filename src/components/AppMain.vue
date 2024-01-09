<!-- HTML & Vue JS-->
<template lang="">
    <main>
              <!-- Section 01: Audio Book-->
        <div class="audio-book d-flex justify-content-center">
            <div class="pubblication">
              <img src="../assets/img/ebay-logotan-2x.png" alt="">
            </div>
            <div class="pubblication">
              <img src="../assets/img/audible-logotan-2x.png" alt="">
            </div>
            <div class="pubblication">
              <img src="../assets/img/bb-logotan-2x.png" alt="">
            </div>
            <div class="pubblication">
              <img src="../assets/img/kindlefire-logotan-2x.png" alt="">
            </div>
        </div>
              <!-- Section 02: Audio Book-->
        <setion class="critics">

        </setion>
              <!-- Section 03: Upcomin Events-->
        <setion class="upcoming-events">

        </setion>
              <!-- Section 04: Subscribe To My Newsletter-->
        <setion class="newsletter">

        </setion>
              <!-- Section 05: Dig A Little Deeper Into Damon Vaughn -->
        <setion class="nav-realese">

        </setion>
              <!-- Section 06: Resent Articles-->
        <setion class="recent-articles">

        </setion>
      </main>
</template>

<!-- Script Code -->
<script>
export default {
    
}
</script>


<!-- SASS Code -->
<style lang="scss">
  @use '../styles/general.scss' as *;
  @use '../styles/partials/variables.scss' as *;
  @use '../styles/partials/mixins.scss' as *;



    .audio-book {
      background-color: $beji-bg;
    }

    //Section 01: Audio Book
    
    .pubblication{
      margin: 3rem;
      img{
        width: 200px;
        height: 80px;
    }
  }

  
</style>