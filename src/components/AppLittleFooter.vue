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
    background-color: #1c1c1c;
    color: white;
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