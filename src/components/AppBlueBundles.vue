<script>
    export default{
        name: 'AppBlueBundles',

        data() {
            return {
                cards:[
                    {
                        img: '/public/img/buy-comics-digital-comics.png',
                        text: 'digital comics'
                    },
                    {
                        img: '/public/img/buy-comics-merchandise.png',
                        text: 'dc merchandise'
                    },
                    {
                        img: '/public/img/buy-comics-subscriptions.png',
                        text: 'subscriptions'
                    },
                    {
                        img: '/public/img/buy-comics-shop-locator.png',
                        text: 'comic shop locator'
                    },
                    {
                        img: '/public/img/buy-dc-power-visa.svg',
                        text: 'dc power visa'
                    },
                ]
            }
        },
    }
</script>

<template>
    <div id="container-blue-bundles">
        <div id="blue-bundles">
            <div id="card" v-for="currentCard in cards">
                <img :src="currentCard.img" alt="">
                <h2>{{currentCard.text}}</h2>
            </div>
        </div>
    </div>
</template>

<style>
   #container-blue-bundles{
        background-color: #0282f9;
        height: 155px;
        display: flex;
        align-items: center;
        z-index: 1;

        #blue-bundles{
            width: 1170px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;
            align-items: center;
            gap: 17px;
            
            #card{
                display: flex;
                gap: 17px;
                height: 55px;

                img{
                    height: 100%;
                }

                h2{
                    font-size: 15px;
                    text-transform: uppercase;
                }
            }
        }
   }
</style>