<!-- HTM & Vue -->
<template lang="">
    <footer>

    <!-- Meta  -->
    <section class="meta">
    <div id="container">
        <div>
            <div>
                <img src="../assets/img/author-logo-round-200x205.png" alt="">
            </div>
            <!-- About ME -->
            <div class="about-me">
                <h4>
                    ABOUT ME
                </h4>
                <p>
                    Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ipsam cupiditate illum voluptate, earum iste, dolorum saepe ut debitis praesentium porro quia ad a nostrum culpa reprehenderit mollitia velit beatae aut.
                </p>
            </div>
            <!-- links -->
            <div class="about-me">
                <nav id="siteslinks">
                    <h4>
                        USEFUL LINKS
                    </h4>
                    <ul>
                        <li v-for="(link, index) in shopLinks" >
                        >   {{ link.content}}
                        </li>
                    </ul>
                </nav>
            </div>
            <!-- Contacts -->
            <div class="about-me">
                <h4>
                    CONTACT INFO
                </h4>
                <p>
                   63 E. Studbaker Street Bolingbrook, IL 60440 
                </p>
                <p>
                    Phone: (800) 000-000
                </p>
                <p>
                    Mobile: (800) 000-000
                </p>
                <p>
                    Email: info@your-comany.com 
                </p>
            </div>
        </div>
    </div>
    </section>

    <!-- Copy Right-->
      <!-- Copy Right -->
      <div class="text-center text-gray pb-5">
        Copiright 2012 - 2020 | Avada Theme by ThemeFusion | All Rights Reserved | Powered by WordPress 
      </div>

    </footer>
</template>

<!-- JAvaScript -->
<script>
export default {
    // NAme Application
    name: 'AppFoter',
    // Data
    data() {
        return {
            shopLinks: [
                {
                    content: 'Latest Books',
                    url: '#',
                    active: false,
                },
                {
                    content: 'UpComing Events',
                    url: '#',
                    active: false,
                },
                {
                    content: 'Recent Articles',
                    url: '#',
                    active: false,
                },
                {
                    content: 'Bussines Enquires',
                    url: '#',
                    active: false,
                },
                {
                    content: 'Visist My Foundation',
                    url: '#',
                    active: false,
                },
            ],
        }
    },
    
}
</script>

<!-- Sass -->
<style lang="scss" scoped>

    // Use StyleSheets
    @use '../styles/partials/variables' as *;
    @use '../styles/partials/mixins' as *;

    footer{
        background-color: $main-color;
        color: white;
        background: url(../assets/img/footer-3.jpg) no-repeat top center;
        margin: 0;
        padding: 0;
        background-size: cover;
        width: 100%;
    }

    #container {
        width: 90%;
        margin: 0 auto;
        padding: 2rem;
        border-radius: 20px;  
        top: 50%;
        >div{
            display: flex;
            justify-content: space-between;
            width: 100%;
        }
        nav{
            margin: 0 3rem 0 0 ;
        }
    }

    .about-me{
        width: calc(100% / 4);
    }
    .meta{
        background-image: url(../assets/img/footer-bg.jpg);
        background-position: center;
    }

    h2{
        padding-bottom: 1.5rem;
    }

    ul{
        list-style-type: none;
        padding: 0;
        li{
            margin-bottom: 0.5rem;
        }
    }

    a {
        text-decoration: none;
        color: white;
    }

    #sign-btn{
        border: 2px solid #0282f9;
        text-align: center;
        padding: 1rem;
        font-weight: bold;
    }

    #follow-info{
        color: #0282f9;
        font-weight: bold;
        font-size: 1.5rem;
        display: inline-block;
        margin-right: 1rem;
    }

    .text-gray{
      color: rgb(150, 147, 147);
    }

</style>