<!-- HTML & Vue JS-->
<template lang="">
    <div class="newsletter">
      <div class="wrapper">
        <div class="text-center">
            <h1 class="text-light">Subscribe To My 
              <br>
              Newsletter
            </h1>
            <p class="danger-color">be notified about book signing tour dates</p>
        </div>
        <div class="d-flex"> 
          <input type="email" class="form-control" id="exampleInputEmail1" placeholder="Insert your email ...*">
          <button type="submit" class="btn btn-success">Subscribe</button>
          
        </div>
        <p class="text-gray mt-4 text-center">cumque ipsa porro et exercitationem commodi corporis,<br> dolor unde nemo eveniet odio.</p>
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


  .newsletter{
    background-image: url('../assets/img/banner-2.jpg');
    input{
      width: 250px;
      margin-right: 1rem;
    }
  }
  .wrapper{
    width: 70%;
    margin: 0 auto;
    padding: 2rem;
    border-radius: 20px;
    height: 470px; 
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
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