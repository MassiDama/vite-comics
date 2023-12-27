<script>
export default {
    name: "ProductCard",
    props: {
        details: Object
    },
}
</script>

<template>
    <div class="cards">
        <div class="prod-card">
        <img :src="details.thumb" :alt="details.series">
        <h3> {{ details.series }} </h3>
    </div>
    </div>
</template>

<style  lang="scss" scoped>
@use '../styles/partials/mixins' as *;
@use '../styles/partials/variables' as *;
@use '../styles/general.scss' as *;

    .cards {
        padding: 50px 0;
        display: flex;

        img {
        width: 150px;
        height: 200px;
    }
    }

   


</style>