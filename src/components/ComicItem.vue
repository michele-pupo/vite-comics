<script>
    export default{
        name: 'ComicItem',

        props:{
            comicName: String,
            comicImage: String
        }
    }
</script>

<template>

   <div id="single-comic">
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
            height: 250px;
        }
    }
   
</style>




