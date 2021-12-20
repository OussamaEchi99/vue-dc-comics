<template>
  <div id="app">
    <Header/>
    
    <main>
      <div class="container">
        <h2>&#8249; Content goes here &#8249;-- </h2>
      </div>
    </main>

    <PreFooter/>

    <Footer/>

    <LoginSocial/>
    
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import PreFooter from "./components/PreFooter.vue";
import Footer from "./components/Footer.vue";
import LoginSocial from "./components/LoginSocial.vue";


export default {
  name: "App",
  components: {
    Header,
    PreFooter,
    Footer,
    LoginSocial,
  },
};
</script>

<style lang="scss">
@import './style/General.scss';
@import './style/Common.scss';

main{
  height: 100px;
  display: flex;
  align-items: center;
  background-color: black;
  color: white;
}

</style>
