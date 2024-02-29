<script>
    export default{
        name: 'AppMain',
        data() {
            return {
                links:[
                    {
                        title: "Dc comics",
                        list:[
                            'Characters',
                            'Comics',
                            'Movies',
                            'TV',
                            'Games',
                            'Videos',
                            'News'
                        ]
                    },
                    {
                        title: "Shop",
                        list:[
                            'Shop DC',
                            'Shop DC Collectibles'
                        ]
                    },
                    {
                        title: "DC",
                        list:[
                            'Terms Of Use',
                            'Privacy policy (New)',
                            'Ad Choices',
                            'Advertising',
                            'Jobs',
                            'Subscriptions',
                            'Talent Workshops',
                            'CPSC Certificates',
                            'Ratings',
                            'Shop Help',
                            'Contact Us'
                        ]
                    },
                    {
                        title: "Sites",
                        list:[
                            'DC',
                            'MAD Magazine',
                            'DC Kids',
                            'DC Universe',
                            'DC Power Visa'
                        ]
                    }
                ]
            }
        },
    }
</script>

<template>
    <div id="bg-image">
        <div id="links-image">
            <div id="links-list-title">
                <div v-for="linkList in links" id="links-list">
                    <h3>{{linkList.title}}</h3>
                    <ul>
                        <li v-for="currentLink in linkList.list">
                            {{currentLink}}
                        </li>
                    </ul>
                </div>
            </div>
            <div id="image-logo">
                <img src="/public/img/dc-logo-bg.png" alt="">
            </div>
        </div>
    </div>
</template>

<style>
    #bg-image{
        height: 400px;
        background-image: url(/public/img/footer-bg.jpg);
        background-size: cover;

        #links-image{
            width: 1250px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;


            img{
                width: 100%;
                position: relative;
                top: -100px;
                z-index: 0;
            }
        }

        #links-list-title{
            display: flex;
            column-gap: 20px;
            
            h3{
                font-size: 30px;
                text-transform: uppercase;
            }

            ul{
                
                list-style-type: none;
                padding: 0px;
                font-size: 15px;
                color: #959595;
            }
        }
    }
  
</style>