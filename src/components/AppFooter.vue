<script>
    export default{
        name: 'AppFooter',
    }
</script>

<template>
   <div id="footer">
        <div id="container-footer">
            <button>Sign-up now!</button>
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

<style>
    #footer{
        background-color: #303030;
        padding: 30px 0;

        #container-footer{
            width: 1250px;
            margin: 0 auto;
            display: flex;
            justify-content: space-between;

            button{
                text-transform: uppercase;
                background-color: transparent;
                border:3px solid #0282f9;
                padding: 0 20px;
                font-size: 20px;
            }

            #social{
                display: flex;
                align-items: center;
                gap: 18px;

                h4{
                    text-transform: uppercase;
                    color: #0282f9;
                    font-size: 20px;
                }
            }
        }
    }
</style>