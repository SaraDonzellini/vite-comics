<script>
export default {
  
}
</script>

<template>
  <div class="wrapper">
    <div class="container flex">
      <button>sign-up now!</button>
      <div class="social">
        <span>Follow Us</span>
        <img src="../assets/img/footer-facebook.png" alt="facebook">
        <img src="../assets/img/footer-twitter.png" alt="twitter">
        <img src="../assets/img/footer-youtube.png" alt="youtube">
        <img src="../assets/img/footer-pinterest.png" alt="pinterest">
        <img src="../assets/img/footer-periscope.png" alt="periscope">
      </div>
    </div>

  </div>
</template>

<style lang="scss" scoped>
  .wrapper{
    height: 8rem;
    background-color: #303030;
    color: white;
    z-index: 2;
  }

  .flex{
    display: flex;
    justify-content: space-between;
    align-items: center;
  }

  .social {
    margin-top: 2rem;

    span {
      text-transform: uppercase;
      font-size: 1.5rem;
      font-weight: bolder;
      color: #0282f9;
      vertical-align: baseline;

    }

    img {
      padding-left: 1rem;
    }
  }

  button{
    margin-top: 2rem;
    padding: 1rem;
    text-transform: uppercase;
    background-color: transparent;
    color: white;
    font-size: large;
    border: 3px solid #0282f9;
  }
</style>