<template>
  <main id="main">
    <!--!HEADER-->
    <header>
      <h1>Lucas Medina Portfolio</h1>
      <nav>
        <form class="container-fluid justify-content-start">
          <button
            class="
              btn btn-sm btn-outline-secondary
              border border-success
              p-2
              mb-2
            "
            type="button"
          >
            Biografia
          </button>
          <button
            class="
              btn btn-sm btn-outline-secondary
              border border-success
              p-2
              mb-2
            "
            type="button"
          >
            Conocimientos
          </button>
          <button
            class="
              btn btn-sm btn-outline-secondary
              border border-success
              p-2
              mb-2
            "
            type="button"
          >
            Portfolio
          </button>
        </form>
      </nav>
    </header>

    <!--!BODY-->
    <div id="principal" class=".container-fluid rounded row">
      <div class="left-arrow col-1">
        <button>&lt;</button>
      </div>
      <div id="photo" class="col-3">
        <img
          src="./resources/images/mypicturefinal.jpg"
          alt="Cargando imagen..."
        />
      </div>
      <div class="container col-6">
        <Biography title="Biografia" />
      </div>
      <!--       <div class="container col-9">
        <Technologys title="Tecnologias" />
      </div> -->
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
import Biography from "./components/Biography.vue";
import Technologys from "./components/Technologys.vue";

export default {
  components: {
    Biography,
    Technologys,
  },
};
</script>



<style>
</style>