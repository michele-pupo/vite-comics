<script>
    import AppBooks from './AppBooks.vue';

    export default{
        name: 'AppJumbotron',
        components: { AppBooks },
    }
</script>

<template>
    <div id="container-jumbotron"></div>
    <AppBooks></AppBooks>
</template>

<style lang="scss">
    #container-jumbotron{
        background-image: url(../../public/img/jumbotron.jpg);
        background-size: cover;
        height: 510px;
    }
</style>