<!-- HTML & Vue JS-->
<template lang="">
    <header>

        <!-- Section Background Image -->
        <section class="header-back">
            <!-- List Links -->
            <nav>
                <div>
                    <img src="../assets/img/author-logo-round-small.png" alt="">
                </div>
                <ul class="m-0">
                    <li v-for="(link, index) in links" >
                    {{ link.content}}
                    </li>
                </ul>
            </nav>
            <!-- Author Detail -->
            <div id="author-detail">
                <div class="pe-5">
                    <div class="rem3 danger-color dancing-script">Damon Vaugh</div>
                    <p class="rem2 salsa">Best-selling author and the most influential public intellectul in the western world right now.</p>
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
                        <!-- Img LAtest Book -->
                        <div>
                            <img src="../assets/img/book-widget.png" alt="">
                            <div>
                                <p>Latest Books Release</p>
                                <div class="danger-color">D.VAUGHN AUTOBIOGRAPHY</div>
                                <div class="color-black">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dolorem repellendus autem pariatur odit voluptatum delectus et sunt hic ipsa distinctio architecto minima voluptatibus, laudantium a perspiciatis ipsam placeat quaerat corrupti?</div>
                            </div>
                        </div>
                        <!-- Buttons Group -->
                        <div class="btn-group" role="group" aria-label="Basic outlined example">
                                <button type="button" class="btn btn-outline-success">Buy on Amazon</button>
                                <button type="button" class="btn btn-outline-success">Buy on AppStore</button>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Section Author Detail -->
        <section id="author-section">
            <div class="text-center mt-5 text-black">
                <div class="rem3 danger-color mb-3 dancing-script">More About Damon Vaugh</div>
                <p class="rem2">
                    Damon Vough is a professor of psychology at the university of Toronto, a clinical psychologist
                    and the author of the multi-milion copy bestseller "The story of my life."
                </p>
                <button type="button" class="btn btn-success mt-4">Meet the Author</button>
            </div>
        </section>

    </header>
</template>

<!-- Script Code -->
<script>

export default {

        // Props provenienti dal padre
        props: {
            links : {
                type : Array,
                require: true,
            }
        },

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
        margin-left: 16rem;
        display: flex;
        justify-content: space-between;
    }


    div h2 {
        color: #f4b429;
    }

    #realese-section{
        background-color: white;
        position: relative;
        width: 650px;
        left:calc(100% - 650px);
    }

    #realese-section > div{
        display: flex;
        p{
            color: black;
            margin: 2rem;
        }
        img{
            padding: 3rem;
        }
    }

    #author-section{
        @include my-wrapper;
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

    .rem4{
        font-size: 3rem;
    }
    .rem3{
        font-size: 3.5rem;
    }
    .rem2{
        font-size: 2rem;
    }

    .color-black{
        color: black;
    }

    // Fonts Family
    .salsa{
        font-family: salsa;
    }

    .dancing-script{
        font-family: 'Caveat', cursive;
        font-family: 'Dancing Script', cursive;
    } 
  
</style>