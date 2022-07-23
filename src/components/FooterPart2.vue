@<template>
  <div class="footer-bg">
    <div class="container">
      <div>
        <!-- button -->
        <button>SIGN-UP NOW!</button>
      </div>
      <div class="social">
        <!-- follow + icone -->
        <h3>FOLLOW US</h3>
        <img src="../assets/img/footer-facebook.png" alt="">
        <img src="../assets/img/footer-twitter.png" alt="">
        <img src="../assets/img/footer-youtube.png" alt="">
        <img src="../assets/img/footer-pinterest.png" alt="">
        <img src="../assets/img/footer-periscope.png" alt="">

      </div>

    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style scoped>
.footer-bg {
  background-color: rgb(48, 48, 48);
  position: relative;
}

.container {
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 150px;
  width: 80%;
  margin: auto;
}

button {
  padding: 10px;
  background-color: rgb(48, 48, 48);
  color: white;
  border: 2px solid rgb(2, 130, 249);
  cursor: pointer;
}

h3 {
  color: rgb(2, 130, 249);
  padding-right: 10px;
  display: flex;
  align-items: center;
}

.social {
  display: flex;
}

img {
  padding: 0 10px;
}
</style>