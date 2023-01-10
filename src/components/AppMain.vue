<script>
import ComicsComponent from './ComicsComponent.vue';

export default {
  components: {
    ComicsComponent,
  }
}

</script>

<template>
    <div class="jumbo-container">

    </div>
    <div class="main-container">
        <div class="my-content">
            
            <ComicsComponent/>

        </div>
    </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

.jumbo-container {
    height: 400px;
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;
}
.main-container {
background-color: $primary-bg-color;
}
.my-content {
    width: 80%;
    margin: 0 auto;
    color: white;
    padding: 3rem 0;
    font-weight: bold;

    h2 {
        font-size: 2rem;
    }
}

</style>
