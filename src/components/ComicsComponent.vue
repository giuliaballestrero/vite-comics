<script>
export default {
    props: {
        img: String,
        title: String
    }
}
</script>

<template>
    <div class="comics-element">
        <img :src="img" :alt="title">
        <h4>{{ title }}</h4>
    </div>
</template>

<style lang="scss">
@use '../styles/partials/variables' as *;

.comics-element {
    width: calc(100% / 6);
    padding: 1rem;

    h4 {
        padding: .5rem 0;
        text-transform: uppercase;
    }

    img {
    object-fit: cover;
    width: 180px;
    height: 180px;
}


}


</style>



