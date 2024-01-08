<!-- HTML & Vue JS-->
<template lang="">
    <header>
        <div class="header-back">
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
<style lang="scss">
  @use '../styles/general.scss' as *;
  @use '../styles/partials/mixins' as *;

    header {
        width: 100vw;
        height: 800px;
    }

    .header-back{
        background: url(../assets/img/footer-3.jpg) no-repeat center center;
        margin: 0;
        padding: 0;
        background-size: cover;
        width: 100%;
        height: 500px;
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


  
</style>