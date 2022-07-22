<template>
  <div id="app">
    <MyHeader />
    <MainPart1 />
    <MainPart2 />
    
  </div>
</template>

<script>
import MyHeader from './components/MyHeader.vue';
import MainPart1 from './components/MainPart1.vue';
import MainPart2 from './components/MainPart2.vue';


export default {
  name: 'App',
  components: {
    MyHeader,
    MainPart1,
    MainPart2,
}
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
