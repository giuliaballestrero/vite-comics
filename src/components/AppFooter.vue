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
            <img src="../assets/img/dc-logo-bg.png" alt="logo dc background">
        </div>
    </div>

    <div class="bottom-container">
        <div class="my-footer-login">
            <div class="my-btn">
                <a href="#"> Sign-up Now!</a>
            </div>
            
            <ul>
                <li>
                    <h1>Follow Us</h1>
                </li>
                
                <li>
                    <img src="../assets/img/footer-facebook.png" alt="facebook icon">
                </li>

                <li>
                    <img src="../assets/img/footer-twitter.png" alt="twitter icon">
                </li>

                <li>
                    <img src="../assets/img/footer-youtube.png" alt="youtube icon">
                </li>

                <li>
                    <img src="../assets/img/footer-pinterest.png" alt="pinterest icon">
                </li>

                <li>
                    <img src="../assets/img/footer-periscope.png" alt="maps icon">
                </li>
                
            </ul>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

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
    }

    .my-footer-menu {
        width: 80%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        
        img {
           object-fit: cover;
           max-height: 400px;
        }
    }
    .my-footer-login {
        width: 80%;
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        padding: 4rem 0;

        .my-btn a {
            border: 3px solid $main-color;
            padding: 1rem;
            text-transform: uppercase;
            font-weight: bold;
            font-size: 1.2rem;
        }

        h1 {
            text-transform: uppercase;
            color: $main-color;
        }

        ul {
            display: flex;

            li {
                padding: 0 .5rem;
            }
        }
    
    };


</style>

