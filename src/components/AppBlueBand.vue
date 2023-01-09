<script>
export default {
  data() {
    return {
      blueList : [
        {
          image: '../assets/img/buy-comics-digital-comics.png',
          text: 'digital comics'
        },
        {
          image: '../assets/img/buy-comics-merchandise.png',
          text: 'dc merchandise'
        },
        {
          image: '../assets/img/buy-comics-subscriptions.png',
          text: 'subscription'
        },
        {
          image: '../assets/img/buy-comics-shop-locator.png',
          text: 'comic shop locator'
        },
        {
          image: '../assets/img/buy-dc-power-visa.svg',
          text: 'DC power visa'
        },
      ]
    }
  },
}
</script>

<template>
  <div class="wrapper">
    <div class="container">
      <ul class="flex">
        <li v-for="item in blueList" class="flex">
          <img :src='item.image' :alt='item.text'><span>{{ item.text }}</span>
        </li>

      </ul>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  .wrapper{
    height: 10rem;
    background-color: #0282f9;
    color: white;

  }
  .flex{
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  img {
    padding-top: 4rem;
  }

  span {
    padding-top: 4rem;
    text-transform: uppercase;
  }

  
</style>