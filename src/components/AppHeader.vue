<!-- HTML & Vue JS-->
<template lang="">
    <header>
        <div class="header-back">
            <!-- List Links -->
            <nav>
                <div>
                    <img src="../assets/img/author-logo-round-small.png" alt="">
                </div>
                <ul class="m-0">
                    <li v-for="(link, index) in navLinks" >
                    {{ link.content}}
                    </li>
                </ul>
            </nav>
            <!-- Author Detail -->
            <div id="author-detail">
                <div>
                    <h2>Damon Vaugh</h2>
                    <p>Best-selling author and the most influential public intellectul in the western world right now.</p>
                    <span>- The New York Times</span>
                </div>
                <!-- Latest Release -->
                <div>
                    <div class="square">
                        Demos
                    </div>
                    <div class="square">
                        $39
                        on Sale
                    </div>
                    <div id="realese-section">
                        <img src="../assets/img/book-widget.png" alt="">
                        <div>
                            <p>Latest Books Release</p>
                            <div class="danger-color">D.VAUGHN AUTOBIOGRAPHY</div>
                            <div>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dolorem repellendus autem pariatur odit voluptatum delectus et sunt hic ipsa distinctio architecto minima voluptatibus, laudantium a perspiciatis ipsam placeat quaerat corrupti?</div>
                        </div>
                    </div>
                </div>
            </div>

        </div>
    </header>
</template>

<!-- Script Code -->
<script>

export default {

    name: 'AppHeader',
    // Variabili
    data() {
        return {
            navLinks: [
                {
                    content: 'Home',
                    url: '#',
                    active: false,
                },
                {
                    content: 'About Me',
                    url: '#',
                    active: false,
                },
                {
                    content: 'Testimonials',
                    url: '#',
                    active: false,
                },
                {
                    content: 'My Blog',
                    url: '#',
                    active: false,
                },
                {
                    content: 'Meetsup',
                    url: '#',
                    active: false,
                },
                {
                    content: 'shop',
                    url: '#',
                    active: false,
                },
                {
                    content: 'Contact Me',
                    url: '#',
                    active: false,
                },
                {
                    content: 'Carrello',
                    url: '#',
                    active: false,
                },
            ],
        }
    },




}
</script>

<!-- SASS Code -->
<style lang="scss" scoped>
  @use '../styles/general.scss' as *;
  @use '../styles/partials/mixins' as *;
  @use '../styles/partials/variables' as *;

    header {
        width: 100vw;
        color: white;
    }

    .header-back{
        background: url(../assets/img/footer-3.jpg) no-repeat center center;
        margin: 0;
        padding: 0;
        background-size: cover;
        width: 100%;
    }

    nav {
        display: flex;
        justify-content: space-around;
    }

    ul {
            @include flex(row,space-between,center);
            list-style-type:none ;
            color: white;
        }

    li{
        font-size: 0.8rem;
        padding: 3rem 1rem;
        font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
        text-transform: uppercase;
        height: 100%;
        &:hover{
            color: #f4b429;
            border-top: 5px solid #f4b429;
            padding-top: calc(3rem - 5px);  
        }
        
    }

    #author-detail{
        margin-left: 10rem;
        display: flex;
        justify-content: space-between;
    }

    div h2 {
        color: #f4b429;
    }

    #realese-section{
        background-color: white;
        position: relative;
        width: 600px;
        left:calc(100% - 600px);
        display: flex;
        p{
            color: black;
            margin: 2rem;
        }
        img{
            padding: 3rem;
        }
    }

    .square{
            color: gray;
            background-color: white;
            padding: 1rem;
            border-radius: 5px;
            width: 80px;
            height: 80px;
            position: relative;
            left:calc(100% - 90px);
            bottom:50px ;
            margin-bottom: 0.5rem;
        }

    .danger-color{
        color: $danger-color;
    }
  
</style>