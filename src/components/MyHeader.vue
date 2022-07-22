@<template>
  <div class="container">
    <nav>
      <div>
        <!-- immagine -->
        <img src="../assets/img/dc-logo.png" alt="">
      </div>
      <div class="ul-container">
        <!-- lista di links -->
        <ul>
          <li v-for="link in links" :key="link.id" :class="{'active': link.active}">{{link.text}}</li>
          
        </ul>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  name:"MyHeader",
  data() {
    return {
      links:[
        {id:1, text:"Charachters" , active: false},
        {id:2, text:"Comics" , active: true},
        {id:3, text:"Movie" , active: false},
        {id:4, text:"Tv" , active: false},
        {id:5, text:"Games" , active: false},
        {id:6, text:"Collectibles" , active: false},
        {id:7, text:"Video" , active: false},
        {id:8, text:"Fans" , active: false},
        {id:9, text:"News" , active: false},
        {id:10, text:"Shop" , active: false},

      ]
    }
  },
}
</script>

<style scoped>
.container {
  border-top: 30px solid black;
}

nav {
  display: flex;
  justify-content: space-between;
  width: 80%;
  margin: auto;
  padding: 20px;
}

img {
  width: 70px;
}

ul {
  display: flex;
  list-style-type: none;
  height: 100%;
}
li {
  padding: 10px;
  height: 100%;
  display: flex;
  align-items: center;
}
li:hover{
  border-bottom: 1px inset rgb(2,130,249);
  cursor: pointer;
  color: rgb(2,130,249);
}
li.active{
  border-bottom: 1px inset rgb(2,130,249);
  cursor: pointer;
  color: rgb(2,130,249);
}
</style>