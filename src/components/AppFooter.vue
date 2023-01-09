<script>
export default {
    data() {
      return {
        dcComicsItems: [
          {
            text: "Characters",
          },
          {
            text: "Comics",
          },
          {
            text: "Movies",
          },
          {
            text: "Tv",
          },
          {
            text: "Games",
          },
          {
            text: "Videos",
          },
          {
            text: "News",
          },
        ],
        shopItems: [
          {
            text: "Shop DC",
          },
          {
            text: "Shop DC Collectibles",
          },
        ],
        dcItems: [
          {
            text: "Term Of Use",
          },
          {
            text: "Privacy policy (New)",
          },
          {
            text: "Ad Choices",
          },
          {
            text: "Advertising",
          },
          {
            text: "Jobs",
          },
          {
            text: "Subscriptions",
          },
          {
            text: "Talent Workshop",
          },
          {
            text: "CPSC Certificates",
          },
          {
            text: "Ratings",
          },
          {
            text: "Shop Help",
          },
          {
            text: "Contact Us",
          },
        ],
        sitesItems: [
          {
            text: "DC",
          },
          {
            text: "MAD Magazine",
          },
          {
            text: "DC Kids",
          },
          {
            text: "DC Universe",
          },
          {
            text: "DC Power Visa",
          },
        ],
      }
    }
}
</script>

<template>
    <div class="top-container">
        <div class="my-footer-menu">
            <nav>
                <div>
                    <ul>
                    <li>
                        <h3>Dc Comics</h3>
                    </li>
                    <li v-for="item in dcComicsItems">
                        <a href="#">{{ item.text }}</a>
                    </li>
                </ul>

                <ul>
                    <li>
                        <h3>Shop</h3>
                    </li>
                    <li v-for="item in shopItems">
                        <a href="#">{{ item.text }}</a>
                    </li>
                </ul>
                </div>
                
                <div>
                    <ul>
                    <li>
                        <h3>Dc</h3>
                    </li>
                    <li v-for="item in dcItems">
                        <a href="#">{{ item.text }}</a>
                    </li>
                </ul>
                </div>

                <div>

                <ul>
                    <li>
                        <h3>Sites</h3>
                    </li>
                    <li v-for="item in sitesItems">
                        <a href="#">{{ item.text }}</a>
                    </li>
                </ul>
                </div>

            </nav>
        </div>
    </div>

    <div class="bottom-container">
        <div class="my-footer-login">
            <a href="#"> Sign-up button </a>
            <ul>
                <li>
                    Lista Social Media
                </li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    * {
        color: white;
    }

    h3 {
        text-transform: uppercase;
        padding-bottom: .5rem;
        font-weight: bold;
        font-size: 1.3rem;
    }

    nav {
        display: flex;

        ul {
            padding: 1rem 1rem 0 1rem;
        }

        li {
            padding: .3rem 0;
            font-size: .8rem;
            color: grey;
        }

        div {
            padding: 2rem 0;
        }
    }

    .top-container {
        background-image: url(../assets/img/footer-bg.jpg);
        background-repeat: no-repeat;
        background-size: cover;
    };

    .bottom-container {
        background-color: #303030;
        height: 200px;
    }

    .my-footer-menu {
        width: 80%;
        margin: 0 auto;
    }
    .my-footer-login {
        width: 80%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
    };


</style>

