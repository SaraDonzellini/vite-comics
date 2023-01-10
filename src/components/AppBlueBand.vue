<script>
export default {
  data() {
    return {
      blueList: [
        {
          image: 'img/buy-comics-digital-comics.png',
          text: 'digital comics'
        },
        {
          image: 'img/buy-comics-merchandise.png',
          text: 'dc merchandise'
        },
        {
          image: 'img/buy-comics-subscriptions.png',
          text: 'subscription'
        },
        {
          image: 'img/buy-comics-shop-locator.png',
          text: 'comic shop locator'
        },
        {
          image: 'img/buy-dc-power-visa.svg',
          text: 'DC power visa'
        },
      ]
    }
  },
  methods: {
    getImagePath: function (imgPath) {
      return new URL(`../assets/${imgPath}`, import.meta.url).href;

    }
  },
}
</script>

<template>
  <div class="wrapper">
    <div class="container">
      <ul class="list flex">
        <li v-for="item in blueList" class="flex">
          <img :src='getImagePath(item.image)' :alt='item.text'><span>{{ item.text }}</span>
        </li>

      </ul>
    </div>
  </div>
</template>

<style lang="scss" scoped>
.wrapper {
  height: 10rem;
  background-color: #0282f9;
  color: white;

}

.flex {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.list {
  padding-top: 3rem;
}

img {
  height: 60px;
}

span {
  text-transform: uppercase;
  padding-left: 0.5rem;
}
</style>