<template>
  <div id="app">
    <Header/>
    
    <main>
      <div class="container">
        Content goes here
      </div>
    </main>

    <PreFooter/>
    
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import PreFooter from "./components/PreFooter.vue";

export default {
  name: "App",
  components: {
    Header,
    PreFooter,
  },
};
</script>

<style lang="scss">
@import './style/General.scss';
@import './style/Common.scss';

main{
  height: 100px;
  background-color: black;
  color: white;
}

</style>
