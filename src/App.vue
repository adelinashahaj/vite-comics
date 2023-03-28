
<template>
  <TheHeader/>
  
  <main>
    <div class="container">
      
     
    </div>
  </main>
 
<CallActionsBonus/>
  <TheFooter/>

</template>

<script >
import TheHeader from './components/TheHeader.vue';
import TheFooter from './components/TheFooter.vue';
import CallActionsBonus from './components/CallActionsBonus.vue';


export default{
  components: {
    TheHeader,
    TheFooter,
    CallActionsBonus
   
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
