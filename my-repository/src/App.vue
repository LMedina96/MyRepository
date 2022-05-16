<template>
  <div id="main">
    <h1>Lucas Medina Portfolio</h1>
    <div id="principal" class=".container-fluid rounded">
      <Biography title="Biografia" />
    </div>
  </div>
</template>





<script>
import Biography from "./components/Biography.vue";
import './assets/style.css';


export default {
  components: {
    Biography,
  },
};
</script>



<style>
</style>