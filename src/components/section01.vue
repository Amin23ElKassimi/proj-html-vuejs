<!-- HTML & Vue JS-->
<template lang="">
  <section>
    <!-- Where Listen AudioBook  -->
    <div class="audio-book d-flex justify-content-center beji-bg">
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
    <!-- Detail -->
    <div id="audio-detail">
      <div class="wrapper-sec01">
        <!-- Image home -->
        <div class="photoaudio cardaudio">
          <img src="../assets/img/audible-app-2x.png" alt="">
        </div>
        <!-- Detail AudioBook -->
        <div class="cardaudio text-light mb-5">
          <h3>
            New AudioBook
          </h3>
          <p class="danger-color">
            no time to read? no problem. listen to it
          </p>
          <p class="text-gray">
            Et quibusdam quo ipsa id soluta recusandae dicta ipsum quas eum deserunt iure dolores iusto ad reiciendis, necessitatibus consectetur explicabo tenetur unde!
          </p>
          <div class="size-img">
            <img src="../assets/img/audible-logo.png" alt="">
            <img src="../assets/img/bn-logo-tall.png" alt="">
            <img src="../assets/img/kindle-logo-tall.png" alt="">
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<!-- Script Code -->
<script>
export default {
    
}
</script>


<!-- SASS Code -->
<style lang="scss" scoped>
  @use '../styles/general.scss' as *;
  @use '../styles/partials/variables.scss' as *;
  @use '../styles/partials/mixins.scss' as *;

  //Section 01: Audio Book
    
    .pubblication{
      margin: 3rem;
      img{
        width: 200px;
        height: 80px;
    }
    }

    #audio-detail{
      background-image: url('../assets/img/banner.jpg');

    }

    .wrapper-sec01{
      display: flex;
      justify-content: center;
      align-items: end;
      width: 70%;
      margin: 0 auto;
      height: 470px;
      img{
        height:400px ;
      }
    }

    .cardaudio{
      text-align: center;
      margin: 0 3rem;
      .size-img{
        img{
        height: 50px;
        width: 100px;
        margin: 0.8rem;
        }
      }
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



    
</style>