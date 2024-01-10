<!-- HTML & Vue JS-->
<template lang="">
  <div class="recent-articles beji-bg">
      <div class="wrapper" >
        <!-- Title -->
        <div class="d-flex justify-content-between">
          <div>
            <h1>
              Recent Articles
            </h1>
            <p class="text-success text-uppercase">
              Read the latest entries
            </p>
          </div>
          <button id="readTestimonials" type="button" class="btn btn-warning text-light fw-bold">All Articles</button>
        </div>
        <!-- Main Section -->
        <div class="d-flex justify-content-between">
            <!-- -->
            <div class="bg-img">
              <img src="../assets/img/20-Tips-600x353.jpg" alt="">
              <h3 class="mt-4">
                20 Crativity Tips
              </h3>
              <p>By admin | october 24th, 2019 | Categories: Events, Tips & Tricks</p>
              <p>
                 Animi necessitatibus ad natus repellendus facere praesentium aliquid voluptatibus ea temporibus expedita sint eligendi commodi, id nostrum unde ipsam, harum eaque iusto.
              </p>
            </div>
            <!--  -->
            <div class="d-flex flex-column justify-content-between cards px-4">
              <!-- card 01 -->
              <div>
                <img src="../assets/img/thumb-13-2x-320x202.jpg" alt="">
                <h3 class="mt-4">
                  20 Crativity Tips
                </h3>
                <p>By admin | october 24th, 2019 | 0 Comments</p>
              </div>
              <!-- card 02 -->
              <div>
                <img src="../assets/img/thumb-08-2x-320x202.jpg" alt="">
                <h3 class="mt-4">
                  20 Crativity Tips
                </h3>
                <p>By admin | october 24th, 2019 |  0 Comments</p>
              </div>
            </div>
        </div>
      </div>
    </div>
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


  .wrapper{
    width: 80%;
    margin: 0 auto;
    padding: 2rem;
    border-radius: 20px; 

  }

  #readTestimonials{
      height: 50px;
      width: 200px;
    }

    .bg-img{
      background-color: white;
      padding: 2rem;
      width: 63%;
      img{
        width: 100%;
      }
    }

    .cards{
      background-color: white;
      padding: 2rem;
      width: 35%;
      img{
        height: 200px;
        width: 100%;
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