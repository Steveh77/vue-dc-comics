@<template>
  <div class="container">
    <div class="cards-container">
      <div v-for="(card,i) in cards" :key="i" class="card">
        <div class="img-container">
          <img
            :src="card.thumb"
            alt="">
        </div>
        <h3>{{card.series}}</h3>
      </div>
    </div>
    <button>LOAD MORE</button>
  </div>
</template>

<script>

export default {
props: {
  cards: Array
}
}
</script>

<style lang="scss" scoped>
.container {
  display: flex;
  flex-direction: column;
  background-color: black;
  align-items: center;
}

.cards-container {
  width: 60%;
  margin: auto;
  display: flex;
  flex-wrap: wrap;
  padding-top: 40px;
  padding-bottom: 40px;
}

.card {
  width: calc(100%/6);
  padding: 10px;

  .img-container {
    height: 150px;

    img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      object-position: top;
    }
  }

}
button{
  height: 50px;
  width: 150px;
  margin-bottom: 50px;
  background-color: rgb(2,130,249);
  color: white;
  border: none;
}
h3 {
  color: white;
}
</style>