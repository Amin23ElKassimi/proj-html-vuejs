<!-- HTML & Vue JS-->
<template lang="">
  <setion class="nav-realese">
    <!-- Content -->
    <div class="wrapper">
      <!-- Title -->
      <div class="text-center">
          <h1 class="text-capitalize">Dig A Litte depper into damon vaughn</h1>
          <p class="text-success text-uppercase">meet the author in person</p>
      </div>
      <!-- Cards -->
      <div class="wrapper-cards d-flex text-center">
        <!-- Card01 -->
        <div class="card-01 mx-4 text-center">
          <div class="d-flex flex-column align-items-center justify-content-end height-100 backdrop-filter">
            <h4 class="text-light fw-bold">About Me</h4> 
            <hr>
            <p class="danger-color">Vestiblum ante ipsum primis</p>
          </div>
        </div>
        <!-- Card02 -->
        <div class="card-02 mx-4" >
          <div class="d-flex flex-column align-items-center justify-content-end height-100 backdrop-filter">
            <h4 class="text-light">My latest Book</h4> 
            <hr>
            <p class="danger-color">Vestiblum ante ipsum primis</p>
          </div>
        </div>
        <!-- Card03 -->
        <div class="card-03 mx-4" >
          <div class="d-flex flex-column align-items-center justify-content-end height-100 backdrop-filter">
            <h4 class="text-light">Book Signing</h4> 
            <hr>
            <p class="danger-color">Vestiblum ante ipsum primis</p>
          </div>
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
    margin: 3rem auto;
    padding: 2rem;
    border-radius: 20px; 
  }

  .wrapper-cards{
    height: 500px;
    hr{
      width: 60px;
      border: solid 2px white;
    }
  }
  .card-01{
    width: calc(100% / 3);
    background-image: url(../assets/img/box-1.jpg) ;
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

    .height-100{
      height: 100%;
    }
    
    .beji-bg{
      background-color:$beji-bg;
    }

    .backdrop-filter{
      backdrop-filter: brightness(0.7);
      border-radius: 0 0 50px 0;  
    }
    
    
</style>