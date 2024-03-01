<script>
    export default{
        name: 'AppFooter',

        data() {
            return {
                socials: [
                    {
                        name: 'facebook',
                        icon: '/img/footer-facebook.png'
                    },
                    {
                        name: 'twitter',
                        icon: '/img/footer-twitter.png'
                    },
                    {
                        name: 'youtube',
                        icon: '/img/footer-youtube.png'
                    },
                    {
                        name: 'pinterest',
                        icon: '/img/footer-pinterest.png'
                    },
                    {
                        name: 'periscope',
                        icon: '/img/footer-periscope.png'
                    },
                ]
            }
        },
    }
</script>

<template>
   <div id="footer">
        <div id="container-footer">
            <button><span>Sign-up now!</span></button>
            <div id="social">
                <h4>Follow us</h4>
                <ul>
                    <li v-for="currentSocial in socials">
                        <img :src="currentSocial.icon" :alt="currentSocial.name">
                    </li>
                </ul>
            </div>
        </div>
   </div>
</template>

<style lang="scss">
    @use '../styles/variables' as *;

    #footer{
        background-color: #303030;
        padding: 30px 0;
        position: absolute;
        width: 100%;
       
        #container-footer{
            width: 1250px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;

            button{
                text-transform: uppercase;
                background-color: transparent;
                border:3px solid $primaryColor;
                padding: 15px;
                cursor: pointer;

                span{
                    font-size: 20px;
                }
            }

            #social{
                display: flex;
                align-items: center;
                gap: 18px;

                h4{
                    text-transform: uppercase;
                    color: $primaryColor;
                    font-size: 20px;
                }

                ul{
                    display: flex;
                    gap: 18px;

                    li{
                        list-style-type: none;
                    }
                }
            }
        }
    }
</style>