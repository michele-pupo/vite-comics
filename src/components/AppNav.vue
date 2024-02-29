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

<style>
    #navbar{
        background-color: white;
        padding: 20px 0px;

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
                }
            }
        }
    }

</style>
