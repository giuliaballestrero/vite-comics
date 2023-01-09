<script>
export default {
    data() {
      return {
        
      }
    }
}
</script>

<template>
    <div class="footer-top-container">
        <div class="my-footer-menu">
            <nav>
                <ul>
                    <li>
                        Menu di Navigazione
                    </li>
                </ul>
            </nav>
        </div>
    </div>

    <div class="footer-bottom-container">
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

<style scoped>

    .my-footer-login {
    display: flex;
    justify-content: space-between;
    height: 200px;
}
    .my-footer-menu,
    .my-footer-login {
        width: 80%;
        margin: 0 auto;
        border: 1px solid black;
    }

    .my-footer-menu {
        height: 400px;
    };

</style>

