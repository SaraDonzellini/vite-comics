<script>
export default {
  data() {
    return {
      mainMenu : [
        {
          text : 'characters',
          status: false,
        },
        {
          text : 'comics',
          status: true,
        },
        {
          text : 'movies',
          status: false,
        },
        {
          text : 'tv',
          status: false,
        },
        {
          text : 'games',
          status: false,
        },
        {
          text : 'collectibles',
          status: false,
        },
        {
          text : 'videos',
          status: false,
        },
        {
          text : 'fans',
          status: false,
        },
        {
          text : 'news',
          status: false,
        },
        {
          text : 'shop',
          status: false,
        },
      ]
    }
  },
}
</script>

<template>
  <div class="container">
    <div class="wrapper">
      <div class="logo">
        <img src="../assets/img/dc-logo.png" alt="dc mini logo">
      </div>
      <div class="navbar">
        <ul class="wrapper">
          <li v-for="menuItem in mainMenu" :class="(menuItem.status) ? 'active' : ''"> {{ menuItem.text }} </li>
        </ul>
      </div>

    </div>
  </div>
</template>

<style lang="scss" scoped>

  img {
    height: 80px;
    padding-top: 1rem;
  }

  .wrapper{
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  ul li {
    list-style-type: none;
    text-transform: uppercase;
    padding: 2rem 1rem;
    font-size: smaller;
    font-weight: bold;
    border-bottom: 0.5rem solid #ffffff;

    &:hover,
    &:active{
      border-bottom: 0.5rem solid #0282f9;
      color: #0282f9;
    }
  }


</style>