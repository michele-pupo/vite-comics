<script>
    export default{
        name: 'AppNav',

        data() {
            return {
                links: [
                        "Characters",
                        "Comics",
                        "Movies",
                        "Tv",
                        "Games",
                        "Collectibles",
                        "Videos",
                        "fans",
                        "News",
                        "Shop"
                        ]
            }
        },
    }
</script>

<template>
    <div id="navbar">
        <div id="container">
            <img src="/img/dc-logo.png" alt="">
            <ul>
                <li v-for="currentLink in links">
                    <a href="">{{currentLink}}</a>
                </li>
            </ul>
        </div>
    </div>
  
</template>

<style lang="scss">
    @use '../styles/variables' as *;

    #navbar{
        background-color: white;
        font-family: 'Barlow Condensed', sans-serif;
        padding: 20px 0px;
        z-index: 1;

        #container{
            width: 1250px;
            margin: 0 auto;
            display: flex;
            align-items: center;
            justify-content: space-between;

            ul{
                display: flex;
                gap: 35px;

                a{
                    text-decoration: none;
                    text-transform: uppercase;
                    font-weight: bold;
                    color: black;
                    &:hover{
                        color: $primaryColorBlue;
                        border-bottom: 8px solid $primaryColorBlue;
                        padding-bottom: 55px;
                    }
                }
            }
        }
    }

</style>
