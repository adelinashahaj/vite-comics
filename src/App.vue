
<template>
  <TheHeader/>
  <Jumbotron/>
  <main>
    <div class="container">
      <ProductList />
     
    </div>
  </main>
 
<CallActionsBonus/>
  <TheFooter/>

</template>

<script >
import TheHeader from './components/TheHeader.vue';
import TheFooter from './components/TheFooter.vue';
import CallActionsBonus from './components/CallActionsBonus.vue';
import ProductList from "./components/ProductList.vue";
import Jumbotron from './components/Jumbotron.vue';


export default{
  components: {
    TheHeader,
    TheFooter,
    CallActionsBonus,
    ProductList,
    Jumbotron
   
  }

}

</script>



<style lang="scss">
@use "./styles/general.scss";
.container{
  max-width: 1170px;
  margin: auto;
}

</style>
