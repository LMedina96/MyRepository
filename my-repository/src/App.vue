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
      <div class="left-arrow col-1">&lt;</div>
      <div id="photo" class="col-3">
        <img src="./resources/images/mypicturefinal.jpg" alt="Cargando imagen..." />
      </div>
      <div class="container col-6">
        <Biography title="Biografia" />
      </div>
      <div class="right-arrow col-1">></div>

      <div class="container carrousel">
        <button
          type="button"
          data-bs-target="#carouselExampleIndicators"
          data-bs-slide-to="0"
          class="active"
          aria-current="true"
          aria-label="Slide 1"
        ></button>
        <button
          type="button"
          data-bs-target="#carouselExampleIndicators"
          data-bs-slide-to="1"
          aria-label="Slide 2"
        ></button>
        <button
          type="button"
          data-bs-target="#carouselExampleIndicators"
          data-bs-slide-to="2"
          aria-label="Slide 3"
        ></button>
      </div>
    </div>
  </main>
</template>





<script>
import Biography from "./components/Biography.vue";
import "./assets/style.css";

export default {
  components: {
    Biography,
  },
};
</script>



<style>
</style>