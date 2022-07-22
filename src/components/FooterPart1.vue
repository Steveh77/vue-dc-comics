@<template>
  <div class="footer-bg">
    <div class="container">
      <div class="list">
        <div>
          <ul class="dc-comics">
            <li>
              <h2>DC COMICS</h2>
            </li>
            <li v-for="link in dcComicsLinks" :key="link.id" >{{ link.text }}</li>

          </ul>
          <ul class="shop">
            <li>
              <h2>Shop</h2>
            </li>
            <li v-for="link in shopLinks" :key="link.id">{{ link.text }}</li>

          </ul>
        </div>
        <div>
          <ul class="dc">
            <li>
              <h2>DC</h2>
            </li>
            <li v-for="link in dcLinks" :key="link.id">{{ link.text }}</li>

          </ul>
        </div>
        <div>
          <ul class="site">
            <li>
              <h2>SITES</h2>
            </li>
            <li v-for="link in sitesLinks" :key="link.id">{{ link.text }}</li>

          </ul>
        </div>
      </div>
      <div class="dcLogoImg">
        <img src="../assets/img/dc-logo-bg.png" alt="">
      </div>
    </div>

  </div>
</template>

<script>
export default {
  name: "footerPart1",
  data() {
    return {
      dcComicsLinks: [
        { id: 1, text: "Characters" },
        { id: 2, text: "Comics" },
        { id: 3, text: "Movies" },
        { id: 4, text: "Tv" },
        { id: 5, text: "Games" },
        { id: 6, text: "video" },
        { id: 7, text: "News" },
      ],
      shopLinks: [
        { id: 1, text: "Shop DC" },
        { id: 2, text: "Shop DC Collectibles" },
      ],
      dcLinks: [
        { id: 1, text: "Terms Of Use" },
        { id: 2, text: "Privacy Policy(new)" },
        { id: 3, text: "Ad Choices" },
        { id: 4, text: "Advertising" },
        { id: 5, text: "Jobs" },
        { id: 6, text: "Subscription" },
        { id: 7, text: "Talent Workshop" },
        { id: 8, text: "CSPS Certificates" },
        { id: 9, text: "Ratings" },
        { id: 10, text: "Shop Help" },
        { id: 11, text: "Contact Us" },
      ],
      sitesLinks: [
        { id: 1, text: "DC" },
        { id: 2, text: "Mad Magazine" },
        { id: 3, text: "DC Kids" },
        { id: 4, text: "DC Universe" },
        { id: 5, text: "DC Power Visa" },
      ],
    }
  },

}
</script>

<style scoped>
.footer-bg {
  background-image: url(../assets/img/footer-bg.jpg);
}
.container {
  display: flex;
  height: 400px;
  justify-content: space-between;
  align-items: center;
  width: 80%;
  margin: auto;
}
.list{
  display: flex;
}

h2 {
  padding: 20px 0;
  color: white;
}

ul {
  padding-right: 50px;
  list-style-type: none;
  color: rgb(136,149,149);
}
</style>