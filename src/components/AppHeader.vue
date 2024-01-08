<!-- HTML & Vue JS-->
<template lang="">
    <header>
        <div class="header-back">
            <nav >
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
                    content: 'charters',
                    url: '#',
                    active: false,
                },
                {
                    content: 'comics',
                    url: '#',
                    active: false,
                },
                {
                    content: 'movies',
                    url: '#',
                    active: false,
                },
                {
                    content: 'tv',
                    url: '#',
                    active: false,
                },
                {
                    content: 'games',
                    url: '#',
                    active: false,
                },
                {
                    content: 'collectibles',
                    url: '#',
                    active: false,
                },
                {
                    content: 'videos',
                    url: '#',
                    active: false,
                },
                {
                    content: 'fans',
                    url: '#',
                    active: false,
                },
                {
                    content: 'news',
                    url: '#',
                    active: false,
                },
                {
                    content: 'shop',
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



  .header-back{
    background-image: url(../assets/img/footer-3.jpg);
    object-fit: contain;
    height: 700px;
    width: 100%;
  }

  ul {
        @include flex(row,space-between,center);
        list-style-type:none ;
    }

    li{
        font-size: 1.2rem;
        padding: 3rem 1rem;
        font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
        text-transform: uppercase;
        &:hover{
            color: #f4b429;
            border-top: 5px solid #f4b429;
            padding-top: calc(3rem - 5px);  
        }
        
    }


  
</style>