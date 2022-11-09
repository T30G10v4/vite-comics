<script>
export default {
    name: "AppJumbo",
    data() {
        return {

        }
    }
}
</script>

<template>

  <section class="jumbo">

    <div class="container">

    </div>

  </section>



</template>

<style lang="scss" scoped>
  @use "../styles/partials/variables" as *;

  section.jumbo {

    background-image: url(../assets/img/jumbotron.jpg);
    height: 40vh;
    background-position: top;
    background-size: cover;


  }

</style>