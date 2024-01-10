<!-- HTML & Vue JS-->
<template lang="">
    <div class="upcoming-events beji-bg">
        <!-- Content -->
        <div class="wrapper-sec03">
        <!-- Title -->
        <div class="text-center">
            <h1 tex>Upcoming Events</h1>
            <p>meet the author in person</p>
        </div>
        <!-- Cards -->
        <div class="d-flex">
            <!-- Card01 -->
            <div class="card mx-4" style="width: 18rem;">
            <img src="../assets/img/event-05.jpg" class="card-img-top" alt="...">
            <div class="card-body">
                <h3>chicago book singing</h3>
                <hr>
                <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
            </div>
            </div>
            <!-- Card02 -->
            <div class="card mx-4" style="width: 18rem;">
            <img src="../assets/img/event-04.jpg" class="card-img-top" alt="...">
            <div class="card-body">
                <h3>meet @ greet with amanda</h3>
                <hr>
                <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
            </div>
            </div>
            <!-- Card03 -->
            <div class="card mx-4" style="width: 18rem;">
            <img src="../assets/img/event-07.jpg" class="card-img-top" alt="...">
            <div class="card-body">
                <h3>open bool: dialouges</h3>
                <hr>
                <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
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

  .wrapper-sec03{
    width: 70%;
    margin: 0 auto;
    padding: 2rem;
    border-radius: 20px; 
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