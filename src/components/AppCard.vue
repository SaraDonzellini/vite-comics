<script>
export default {
  props: [
    'thumbnail',
    'price',
    'series',
    'type'
  ],

}
</script>

<template>
  <div>
    <div class="img-wrapper">
      <img :src="thumbnail">
    </div>
    <!-- <span>{{ price }} - {{ type }}</span> -->
    <p>{{ series }}</p>
  </div>
</template>

<style lang="scss" scoped>
.img-wrapper {
  margin-top: 1rem;
  height: 192px;
  overflow: hidden;

  &:hover {
    filter: grayscale(80%);

  }
}

p {
  text-transform: uppercase;
  padding-top: 1rem;
}

// span{
//   position: relative;
//   bottom: 100px;
//   left: 10px;
//   text-transform: uppercase;
//   display: none;

//   &:hover{
//     display: inline;
//   }
// }
</style>