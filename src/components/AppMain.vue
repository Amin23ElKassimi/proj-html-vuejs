<!-- HTML & Vue JS-->
<template lang="">
    <main>
              <!-- Section 01: Audio Book-->
        <!-- Where Listen AudioBook  -->
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
              <!-- Section 02: What The Critics Say-->
        <setion class="critics">
            <div class="wrapper-sec02" >
              <!-- What the critics Say -->
              <div class="what-critics">
                <h1>
                  What The Critics Say
                </h1>
                <p class="text-success text-uppercase">
                  tesimonials from around the world
                </p>
                <!-- Background img -->
                <div class="text-light">
                  <h2>
                    Best Author Of His Generation
                  </h2>
                  <hr>
                  <p>
                    This Book Will change your perspective on life
                  </p>
                  <div>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Optio dicta aliquam corporis officia modi libero minima hic iste eveniet tenetur! Accusantium quae quidem velit labore provident reiciendis eveniet dolor maiores.
                  </div>
                  <div>
                    Lorem ipsum dolor sit amet consectetur adipisicing elit. Optio dicta aliquam corporis officia modi libero minima hic iste eveniet tenetur! Accusantium quae quidem velit labore provident reiciendis eveniet dolor maiores.
                  </div>
                  <p class="mt-5">
                    <img src="../assets/img/nytimes-logo-white-xsmall.png" alt="">
                    Justine Kilpatrick, 
                    <span class="fw-bold text-success mt-5">The New York Times</span>
                  </p>
                </div>
              </div>
              <!-- Testimonials -->
              <div class="testimonials px-4">
                <button type="button" class="btn btn-warning text-light fw-bold">Read All Testiomonials</button>
                <div class="mb-3">
                  <h3 class="text-capitalize">a ture masterpiece, bravo!</h3>
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quasi earum pariatur ut perferendis non quibusdam maiores ex. Porro veritatis facilis numquam, ut facere pariatur harum, et nisi corrupti quis est.
                </div>
                <p class="mb-5">
                  <img src="../assets/img/theguardian-xsmall.png" alt="">
                  Gerald Hendley, The Guardian
                </p>
                <div class="mb-3">
                  <h3 class="text-capitalize">a ture masterpiece, bravo!</h3>
                  Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quasi earum pariatur ut perferendis non quibusdam maiores ex. Porro veritatis facilis numquam, ut facere pariatur harum, et nisi corrupti quis est.
                </div>
                <p class="mb-5">
                  <img src="../assets/img/globe-xsmall.png" alt="">
                  Mary Maxey, The Globe And Mail
                </p>
              </div>
            </div>
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
<style lang="scss" scoped>
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

    //  Section 02: What The Critics Say

    .wrapper-sec02{
      display: flex;
      align-items: end;
      width: 70%;
      margin: 0 auto;
      padding: 2rem;
      border-radius: 20px; 
    }



    .what-critics{
      width: 60%;
    }

    .what-critics > div{
        background-image: url(../assets/img/testimonial2-2x.jpg);
        background-repeat: no-repeat;
        background-size: 100% 100%;
        height: 585px;
        border-radius: 0 0 100px 0px;
        width: 100%;
        padding: 3rem;
      }

      .testimonials{
        width: 40%;
        display: flex;
        flex-direction: column;
        button{
          align-self: flex-end;
          width: 200px;
          margin-bottom: 4rem;
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

    // Margin Padding Border



</style>