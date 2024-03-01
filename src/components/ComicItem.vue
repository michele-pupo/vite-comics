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
        }

        h4{
            font-family: 'Barlow Condensed', sans-serif;
            text-transform: uppercase;
            font-size: 18px;
        }

        span{
            color: $primaryColorBlue;
            text-transform: uppercase;
            font-weight: bold;
            position: relative;
            top: 190px;
            right: -120px;
        }

        strong{
            text-transform: uppercase;
            color: $primaryColorBlue;
            font-size: 15px;
        }
    }
   
</style>




