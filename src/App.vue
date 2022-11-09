<script>

  import AppHeader from "./components/AppHeader.vue";
  import AppJumbo from "./components/AppJumbo.vue"
  import AppComics from "./components/AppComics.vue"

  export default {

    components: {

      AppHeader,
      AppJumbo,
      AppComics

    }

  }

</script>

<template>

  <AppHeader />
  <AppJumbo />
  <AppComics />
</template>

<style lang="scss">
  @use "./styles/general.scss" as *;
</style>