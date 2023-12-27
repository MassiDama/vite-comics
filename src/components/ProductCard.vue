<script>
export default {
    name: "ProductCard",
    props: {
        details: Object
    },
}
</script>

<template>
    <div class="prod-card">
        <img :src="details.thumb" :alt="details.series">
        <h3> {{ details.series }} </h3>
    </div>
</template>

<style  lang="scss" scoped>
@use '../styles/partials/mixins' as *;
@use '../styles/partials/variables' as *;
@use '../styles/general.scss' as *;

    .prod-card {
        width: calc(100% / 6);
        padding-right: 20px;
        padding-bottom: 20px;

        img {
            width: 100%;
            height: 200px;
            padding-bottom: 10px;
        }
    }
   


</style>