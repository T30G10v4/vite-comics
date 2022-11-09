<script>

    import { toHandlers } from 'vue';

    export default {

        name: "AppSingleComic",
        props: {

            thumb: String,
            price: String,
            series: String,
            type: String

        }

    }

</script>

<template>

    <div class="card">
        <img :src="thumb" alt="series">
        <h3>{{series}}</h3>
    </div>

</template>

<style lang="scss" scoped>

.card {

    width: calc(100% / 6 - 10px);
    
    img {

        display: block;

    }

    h3 {

        color:white;
        margin-top: 1rem;

    }

}

</style>