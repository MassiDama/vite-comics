<script>
export default {
    name: "AppFooter",
}
</script>

<template>

    <section class="blue-bar">
        <div class="container">

            <!-- prima parte del footer (info) -->
            <div class="infobar">
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
    </section>

    <section class="footer-info">

         <!-- parte info section -->
        <div class="info-section">
            

        </div>

    </section>

   
    
</template>

<style lang="scss" scoped>
@use '../styles/partials/mixins' as *;
@use '../styles/partials/variables' as *;
@use '../styles/general.scss' as *;

    .blue-bar {
        width: 100%;
        background-color: $primary;

        .container {
        
            
            .infobar {
                display: flex;
                justify-content: space-around;
                align-items: center;
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
    }

    .footer-info {
        background-image: url(../../public/img/footer-bg.jpg);
        width: 100%;
        height: 500px;
    }
    

</style>