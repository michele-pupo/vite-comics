<script>
    export default{
        name: 'AppFooter',
    }
</script>

<template>
   <div id="footer">
        <div id="container-footer">
            <button><span>Sign-up now!</span></button>
            <div id="social">
                <h4>Follow us</h4>
                <img src="/public/img/footer-facebook.png" alt="">
                <img src="/public/img/footer-twitter.png" alt="">
                <img src="/public/img/footer-youtube.png" alt="">
                <img src="/public/img/footer-pinterest.png" alt="">
                <img src="/public/img/footer-periscope.png" alt="">
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
                border:3px solid $primaryColorBlue;
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
                    color: $primaryColorBlue;
                    font-size: 20px;
                }
            }
        }
    }
</style>