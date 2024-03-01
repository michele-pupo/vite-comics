<script>
    import AppNav from './components/AppNav.vue';
    import AppJumbotron from './components/AppJumbotron.vue';
    import AppMain from './components/AppMain.vue';
    import AppFooter from './components/AppFooter.vue';

    export default{

    components: {
        AppNav,
        AppJumbotron,
        AppMain,
        AppFooter
    },

}
</script>

<template>
    
    <AppNav></AppNav>
    <AppJumbotron></AppJumbotron>
    <AppMain></AppMain>
    <AppFooter></AppFooter>

</template>

<style lang="scss">
  @use './styles/general.scss' as *;
</style>
