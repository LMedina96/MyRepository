<template>
  <main id="main">
    <!--!HEADER-->
    <HeaderComponent title="Lucas Medina Portfolio" v-on:change-page="getPageId"/>

    <!--!BODY-->
    <div id="principal" class=".container-fluid rounded row">
      <div class="left-arrow col-1 col-sm-1">
        <button @click="removePageId()">&lt;</button>
      </div>
      <div id="bodyStructure" class="col-9 col-sm-8">
        <Biography v-if="setPageValue == 1" title="Biografia" />
        <Technologys v-else-if="setPageValue == 2" title="Tecnologias" />
        <Portfolio v-else-if="setPageValue == 3" title="Portfolio" />
      </div>
      <div class="right-arrow col-1 col-sm-1">
        <button @click="addPageId()">></button>
      </div>
      <Carrousel :CarrouselButtonsNumber = '3' v-on:get-button-index="getButtonIndex"/>
    </div>
  </main>
</template>

<script>
import "./assets/style.css";
import HeaderComponent from "./components/HeaderComponent.vue";
import Biography from "./components/Biography.vue";
import Technologys from "./components/Technologys.vue";
import Portfolio from "./components/Portfolio.vue";
import Carrousel from "./components/Carrousel.vue"

export default {
  components: {
    HeaderComponent,
    Biography,
    Technologys,
    Portfolio,
    Carrousel,
  },

  data() {
    return {
      setPageValue: 1,
    };
  },

  methods: {
    getPageId(id) {
      this.setPageValue = id;
    },

    addPageId() {
      if (this.setPageValue < 3) {
        this.setPageValue++;
      } else {
        this.setPageValue = 1;
      }
    },

    removePageId() {
      if (this.setPageValue > 1) {
        this.setPageValue--;
      } else {
        this.setPageValue = 3;
      }
    },

    getButtonIndex(index) {
      this.setPageValue = index;
    },
  },


};
</script>



<style>
</style>