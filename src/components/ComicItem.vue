<script>
    export default{
        name: 'ComicItem',

        props:{
            comicName: String,
            comicImage: String,
            comicPrice: String,
            comicType: String
        }
    }
</script>

<template>

   <div id="single-comic">
        <span>{{ comicPrice }}</span>
        <strong>{{ comicType }}</strong>
        <img :src="comicImage" alt="">
        <h4>{{ comicName }}</h4>
    </div>
   
</template>

<style lang="scss">
    @use '../styles/variables' as *;

    #single-comic{
        width: calc(100% / 6 - 30px / 6 * 5);

        img{
            width: 100%;
            height: 200px;
            cursor: pointer;
            &:hover{
                animation: comic 3s ease infinite;
            }
            
        }

        h4{
            font-family: 'Barlow Condensed', sans-serif;
            text-transform: uppercase;
            font-size: 18px;
        }

        span{
            color: $primaryColor;
            text-transform: uppercase;
            font-weight: bold;
            position: relative;
            top: 190px;
            right: -120px;
        }

        strong{
            text-transform: uppercase;
            color: $primaryColor;
            font-size: 15px;
        }
    }

    @keyframes comic {
    0% {
        transform: scale(1);
    }

    50% {
        transform: scale(0.9);
    }

    100% {
        transform: scale(1);

    }
}
   
</style>




