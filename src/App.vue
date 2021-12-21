<template>
  <div id="app">
    <Header/>
    
    <main>
      <Jumbotron/>

      <ProductsList/>
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
import Jumbotron from "./components/Jumbotron.vue";
import ProductsList from "./components/ProductsList.vue";


export default {
  name: "App",
  components: {
    Header,
    PreFooter,
    Footer,
    LoginSocial,
    Jumbotron,
    ProductsList,
  },
};
</script>

<style lang="scss">
@import './style/General.scss';
@import './style/Common.scss';

// main{
//   height: 100px;
//   display: flex;
//   align-items: center;
//   background-color: black;
//   color: white;
// }

</style>
