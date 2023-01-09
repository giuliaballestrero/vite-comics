<script>
export default {
    data() {
      return {
        navItems: [
          {
            text: "Characters",
            active: false,
          },
          {
            text: "Comics",
            active: true,
          },
          {
            text: "Movies",
            active: false,
          },
          {
            text: "Tv",
            active: false,
          },
          {
            text: "Games",
            active: false,
          },
          {
            text: "Collectibles",
            active: false,
          },
          {
            text: "Videos",
            active: false,
          },
          {
            text: "Fans",
            active: false,
          },
          {
            text: "News",
            active: false,
          },
          {
            text: "Shop",
            active: false,
          }
        ]
      }
    }
}

</script>

<template>
  <div class="header-container">
    <div>
      <img src="../assets/img/dc-logo.png" alt="lodo dc">
    </div>

    <nav>
      <ul>
        <li v-for="item in navItems" :class="(item.active) ? 'active' : ''">
        <a href="#">{{ item.text }}</a>
        </li>
      </ul>
    </nav>
  </div>
</template>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
 .header-container{
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 80%;
  margin: 0 auto;
 }

 img {
  padding: 1rem 1rem;
  width: 80%;
 }

 nav ul {
    display: flex;

    li {
      padding: 1rem 1rem;
      font-weight: bold;
      text-transform: uppercase;

      &.active,
      &:hover {
        color: $main-color;
      } 
      }
    }

</style>
