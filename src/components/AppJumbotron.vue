<script>
export default {
    name: "AppJumbotron",
}
</script>

<template>
    <section class="jumbotron">

    </section>
</template>

<style lang="scss" scoped>
@use '../styles/partials/mixins' as *;
@use '../styles/partials/variables' as *;
@use '../styles/general.scss' as *;

    .jumbotron {
        width: 100%;
        height: 350px;
        background-image: url("../../public/img/jumbotron.jpg");
        background-size: cover;
    }

</style>