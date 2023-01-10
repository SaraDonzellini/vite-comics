<script>
export default {
  props : [
          'thumbnail',
          'price',
          'series',
          'type'
  ],
  methods: {
    
  },
}
</script>

<template>
  <div>
    <div class="img-wrapper" @mouseenter="">
      <img :src="thumbnail" >
    </div>
    <!-- <span>{{ price }} - {{ type }}</span> -->
    <p>{{ series }}</p>
  </div>
</template>

<style lang="scss" scoped>
    .img-wrapper{
    margin-top: 1rem;
    height: 192px;
    overflow: hidden;

      &:hover{
        filter: grayscale(100%);

      }
  }
  p{
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