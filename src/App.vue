<script>
    import AppNav from './components/AppNav.vue';
    import AppContent from './components/AppContent.vue';
    import AppBlueBundles from './components/AppBlueBundles.vue';

    export default{

    
    components: {
        AppNav,
        AppContent,
        AppBlueBundles
    },

}
</script>

<template>
    
    <AppNav></AppNav>
    <AppContent></AppContent>
    <AppBlueBundles></AppBlueBundles>

</template>

<style lang="scss">
  @use './styles/general.scss' as *;
</style>
