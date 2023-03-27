
<template>
  <TheHeader/>
  

  <main>
    <div class="container">
      
      <h4>content goes here</h4>
    </div>
  </main>
  <TheFooter/>
</template>

<script >
import TheHeader from './components/TheHeader.vue';
import TheFooter from './components/TheFooter.vue';

export default{
  components: {
    TheHeader,
    TheFooter,
  }

}

</script>



<style lang="scss">
@use"./styles/general.scss";
.container{
  max-width: 1170px;
  margin: auto;
}

</style>
