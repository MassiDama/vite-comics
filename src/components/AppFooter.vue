<script>
export default {
    name: "AppFooter",
}
</script>

<template>
    <div class="container">
        <div class="info">
            <div class="info-item">
                <img src="../../public/img/buy-comics-digital-comics.png" alt="">
                <h5> DIGITAL COMICS</h5>
            </div>
            <div class="info-item">
                <img src="../../public/img/buy-comics-merchandise.png" alt="">
                <h5> DC MERCHANDISE</h5>
            </div>
            <div class="info-item">
                <img src="../../public/img/buy-comics-subscriptions.png" alt="">
                <h5> SUBSCRIPTIONS</h5>
            </div>
            <div class="info-item">
                <img src="../../public/img/buy-comics-shop-locator.png" alt="">
                <h5> COMIC SHOP LOCATOR</h5>
            </div>
            <div class="info-item">
                <img src="../../public/img/buy-comics-digital-comics.png" alt="ciao">
                <h5> DC POWER VISA</h5>
            </div>
        </div>
    </div>
    
</template>

<style lang="scss" scoped>
@use '../styles/partials/mixins' as *;
@use '../styles/partials/variables' as *;
@use '../styles/general.scss' as *;

    .container {
        background-color: $primary;
        
        .info {
            display: flex;
            justify-content: space-around;
            align-items: center;
            margin: 30px 0;
            padding: 30px 0;

            .info-item {
                 @include flex-between();

                img {
                    width: 60px;
                    padding-right: 15px;
                }

                h5 {
                    color: white;
                }
            }
        }
    }
    

</style>