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
        <h5>{{ title }}</h5>
    </div>
</template>

<style lang="scss">
@use '../styles/partials/variables' as *;

.comics-element {
    width: calc(100% / 6 - 1rem);
    padding: 1rem;

    h5 {
        padding: .5rem 0;
        text-transform: uppercase;
    }

    img {
    object-fit: cover;
    object-position: top;
    width: 180px;
    height: 180px;
}


}


</style>



