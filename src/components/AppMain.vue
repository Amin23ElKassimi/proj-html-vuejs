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
        <div id="audio-detail">
          <div class="photoaudio cardaudio">
            <img src="../assets/img/audible-app-2x.png" alt="">
          </div>
          <div class="cardaudio text-light">
            <h3>
              New AudioBook
            </h3>
            <p class="">
              no time to read? no problem. listen to it
            </p>
          </div>
        </div>
              <!-- Section 02: What The Critics Say-->
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

    #audio-detail{
      display: flex;
      justify-content: center;
      align-items: center;
      background-image: url('../assets/img/banner.jpg');
      height: 670px;
      img{
        height:500px ;
      }
    }

    .photoaudio{
      align-self: flex-end;
    }

    .cardaudio{
      margin: 0 3rem;
    }


    //  Section 02: What The Critics Say

  
</style>