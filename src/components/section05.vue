<!-- HTML & Vue JS-->
<template lang="">
  <setion class="nav-realese">
    <!-- Content -->
    <div class="wrapper">
      <!-- Title -->
      <div class="text-center">
          <h1 tex>Upcoming Events</h1>
          <p>meet the author in person</p>
      </div>
      <!-- Cards -->
      <div class="wrapper-cards d-flex text-center">
        <!-- Card01 -->
        <div class="card-01 mx-4 text-center">
          <div>
            <p>About Me</p> 
            <hr>
            <p>Vestiblum ante ipsum primis</p>
          </div>
        </div>
        <!-- Card02 -->
        <div class="card-02 mx-4" >
        
        </div>
        <!-- Card03 -->
        <div class="card-03 mx-4" >
       
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

  
  .wrapper{
    width: 80%;
    margin: 0 auto;
    padding: 2rem;
    border-radius: 20px; 
  }

  .wrapper-cards{
    height: 500px;
    hr{
      width: 50px;
    }
  }
  .card-01{
    width: calc(100% / 3);
    background-image: url(../assets/img/box-1.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    border-radius: 0 0 50px 0;  
  }
  .card-02{
    width: calc(100% / 3);
    background-image: url(../assets/img/box-4.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    border-radius: 0 0 50px 0;  
  }
  .card-03{
    width: calc(100% / 3);
    background-image: url(../assets/img/box-3.jpg);
    background-repeat: no-repeat;
    background-size: cover;
    border-radius: 0 0 50px 0;  
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