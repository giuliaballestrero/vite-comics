<script>

</script>

<template>
    <div class="banner-container">
        <div class="icon-container">
            <ul>
                <li>
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="digital comics">
                    <p>Digital Comics</p>
                </li>

                <li>
                    <img src="../assets/img/buy-comics-merchandise.png" alt="dc merchandise">
                    <p>Dc Merchandise</p>
                </li>

                <li>
                    <img src="../assets/img/buy-comics-subscriptions.png" alt="subscription">
                    <p>Subscription</p>
                </li>

                <li>
                    <img src="../assets/img/buy-comics-shop-locator.png" alt="comic locator">
                    <p>Comic Shop Locator</p>
                </li>

                <li>
                    <img src="../assets/img/buy-dc-power-visa.svg" alt="dc power visa">
                    <p>Dc Power Visa</p>
                </li>
            </ul>
        </div>
    </div>

</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

.banner-container  {
    background-color: $main-color;

    .icon-container  {
    margin: 0 auto;
    width: 80%;

    ul {
        display: flex;
        justify-content: space-between;
        padding: 3rem;

        li {
            display: flex;
            align-items: center;

            img {
                height: 50px;
                aspect-ratio: 0.8;
            }

            p {
                padding: 1rem;
                color: white;
                text-transform: uppercase;
                font-weight: bold;
            }
        }
    }
    }
}


</style>
