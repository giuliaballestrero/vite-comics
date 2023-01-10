<script>
export default {
    props: {
        img: String,
        title: String
    }
}
</script>

<template>
    <div>
        <img :src="img" :alt="title">
        <h3>{{ title }}</h3>
    </div>
</template>

<style lang="scss">
@use '../styles/partials/variables' as *;

</style>



