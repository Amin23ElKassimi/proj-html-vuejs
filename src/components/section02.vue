<!-- HTML & Vue JS-->
<template lang="">
        <setion class="critics">
            <div class="wrapper-sec02" >
              <!-- Title -->
              <div class="d-flex justify-content-between">
                <div>
                  <h1>
                    What The Critics Say
                  </h1>
                  <p class="text-success text-uppercase">
                    tesimonials from around the world
                  </p>
                </div>
                <button id="readTestimonials" type="button" class="btn btn-warning text-light fw-bold">Read All Testiomonials</button>
              </div>
              <!-- Main Section -->
              <div class="d-flex">
                  <!-- What the critics Say -->
                  <div class="what-critics">
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
                    <div class="mb-3 p-2 beji-bg">
                      <h3 class="text-capitalize">a ture masterpiece, bravo!</h3>
                      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quasi earum pariatur ut perferendis non quibusdam maiores ex. Porro veritatis facilis numquam, ut facere pariatur harum, et nisi corrupti quis est.
                    </div>
                    <p class="mb-5">
                      <img src="../assets/img/theguardian-xsmall.png" alt="">
                      Gerald Hendley, The Guardian
                    </p>
                    <div class="mb-3 p-2 beji-bg">
                      <h3 class="text-capitalize">a ture masterpiece, bravo!</h3>
                      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Quasi earum pariatur ut perferendis non quibusdam maiores ex. Porro veritatis facilis numquam, ut facere pariatur harum, et nisi corrupti quis est.
                    </div>
                    <p class="mb-5">
                      <img src="../assets/img/globe-xsmall.png" alt="">
                      Mary Maxey, The Globe And Mail
                    </p>
                  </div>
              </div>
            </div>
        </setion>
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


    .wrapper-sec02{
    width: 70%;
    margin: 0 auto;
    padding: 2rem;
    border-radius: 20px; 

  }
  #readTestimonials{
      height: 50px;
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