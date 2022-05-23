<template>
  <main id="main">
    <!--!HEADER-->
    <HeaderComponent title="Lucas Medina Portfolio" :buttons="['Biografia', 'Tecnologias', 'Portfolio']"/>

    <!--!BODY-->
    <div id="principal" class=".container-fluid rounded row">
      <div class="left-arrow col-1">
        <button>&lt;</button>
      </div>
      <div class="col-9">
        <Biography title="Biografia" />
        <Technologys title="Tecnologias" />
        <Portfolio title="Portfolio" />
      </div>
      <div class="right-arrow col-1">
        <button>></button>
      </div>

      <div class="container carrousel">
        <button type="button" class="active"></button>
        <button type="button"></button>
        <button type="button"></button>
      </div>
    </div>
  </main>
</template>

<script>
import "./assets/style.css";
import HeaderComponent from "./components/HeaderComponent.vue";
import Biography from "./components/Biography.vue";
import Technologys from "./components/Technologys.vue";
import Portfolio from "./components/Portfolio.vue";

export default {
  components: {
    HeaderComponent,
    Biography,
    Technologys,
    Portfolio,
  },
};
</script>



<style>
</style>