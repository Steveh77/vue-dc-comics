<template>
  <div id="app">
    <MyHeader />
    <MyJumbo />
    <MainPart1 :cards="cards" />
    <MainPart2 />
    <FooterPart1 />
    <FooterPart2 />
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue';
import MainPart1 from './components/MainPart1.vue';
import MainPart2 from './components/MainPart2.vue';
import FooterPart1 from './components/FooterPart1.vue';
import FooterPart2 from './components/FooterPart2.vue';
import MyJumbo from './components/MyJumbo.vue';
import CardJson from './assets/dc-comics.json';


export default {
  name: 'App',
  components: {
    MyHeader,
    MainPart1,
    MainPart2,
    FooterPart1,
    FooterPart2,
    MyJumbo
},
data() {
  return {
    cards:CardJson
  }
},
}
</script>

<style lang="scss">
  *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  body{
    font-family: 'Oswald', sans-serif;
  }
</style>
