<script>
export default {
  data() {
    return {
      dcComicsList : [
        'characters', 'comics', 'movies', 'tv', 'games', 'videos', 'news'
      ],
      dcShopList : [
        'shop DC', 'shop DC Collectibles'
      ],
      dcList : [
        'terms of use', 'privacy policy (new)', 'ad choices', 'asvertising', 'jobs', 'subscriptions', 'talent workshops', 'CPCS certificates', 'ratings', 'shop help', 'contact us'
      ],
      dcSitesList : [
        'DC', 'MAD Magazine', 'DC Kids', 'DC Universe', 'DC Power Visa'
      ]
    }
  },
}
</script>

<template>
<div class="wrapper">
  <div class="container flex">
    <div class="flex">
      <div class="leftLists">
        <ul class="dccomics"> dc comics
          <li v-for="itemList in dcComicsList"> {{ itemList }}</li>
        </ul>
        <ul class="dcShopList"> shop
          <li v-for="itemList in dcShopList"> {{ itemList }}</li>
        </ul>
      </div>
      <div class="centLists">

        <ul class="dcList"> dc
          <li v-for="itemList in dcList"> {{ itemList }}</li>
        </ul>
      </div>
      <div class="rightLists">
        <ul class="dcSitesList"> sites
          <li v-for="itemList in dcSitesList"> {{ itemList }}</li>
        </ul>

      </div>
    </div>
    <div class="logo">
      <img src="../assets/img/dc-logo-bg.png" alt="big dc logo">
    </div>
  </div>
</div>
</template>

<style lang="scss" scoped>
  
  .wrapper{
    background-image: url('../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;
    
    
  }

  .flex{
    display: flex;
    justify-content: space-between;
  }

  ul {
    margin: 1rem;
    text-transform: uppercase;
    font-weight: bold;
    font-size: larger;
    color: white;

    li {
      text-transform: capitalize;
      font-size: smaller;
      list-style-type: none;
      color: #959595;

    }
  }

</style>