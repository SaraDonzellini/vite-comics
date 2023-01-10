<script>
export default {
  props : [
          'thumbnail',
          'price',
          'series',
          'type'
  ]
}
</script>

<template>
  <div>
    <div class="img-wrapper">
      <img :src="thumbnail">
    </div>
    <p>{{ series }}</p>
  </div>
</template>

<style lang="scss">
    .img-wrapper{
    margin-top: 1rem;
    height: 192px;
    overflow: hidden;

      &:hover{
        filter: grayscale(70%);

      }
  }
  p{
    text-transform: uppercase;
    padding-top: 1rem;
  }

</style>