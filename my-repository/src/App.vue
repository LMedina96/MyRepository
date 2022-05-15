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

export default {
  components: {
    Biography,
  },
};
</script>





<style>
* {
  box-sizing: content-box;
}

body {
  background-color: black;
  color: white;
  background-image: url("./resources/images/backgroundPortfolio.jpg");
  background-size: cover;
}

#main {
  text-align: center;
}

h1 {
  background-color: rgb(56, 56, 56);
  padding: 1rem;
}

#principal {
  background-color: rgba(61, 61, 61, 0.8);
  margin: 5rem 2rem;
  min-height: 70vh;
}
</style>
