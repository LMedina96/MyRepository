<template>
  <header>
    <h1>{{ title }}</h1>
    <nav>
      <form class="container-fluid justify-content-start">
        <button
          type="button"
          class="
            btn btn-sm btn-outline-secondary
            border border-success
            p-2
            mb-2"
          @click="changePage(button.id)"
          v-for="button in buttons"
          :key="button.id"
          v-bind:class="[{active: button.isActive}]"
        >
          <a href="#">{{button.text}}</a>
        </button>
      </form>
    </nav>
  </header>
</template>

<script>
export default {
  props: {
    title: String,
  },

  data() {
    return {
      
      buttons: [
        {
          id: 1,
          text: "Biografia",
          isActive: true,
        },
        {
          id: 2,
          text: "Tecnologias",
          isActive: false,
        },
        {
          id: 3,
          text: "Portfolio",
          isActive: false,
        },
      ],
      
    };
  },

  methods: {
    changePage(id) {
      this.$emit("change-page", id);
      this.buttons.forEach(button => {
        if(button.id == id) {
          button.isActive = true;
        } else {
          button.isActive = false;
        }
      });
    },
  },
}
</script>

<style scoped>
header {
  background-color: rgb(25, 26, 25);
  padding: 1rem;
  width: 90vw;
  margin: 0rem auto;
  border-radius: 20px;
  border: 1px solid rgb(78, 159, 61);
}

header button {
  width: 150px;
  margin: 0 1rem;
  border: 3px solid rgb(78, 159, 61) !important;
  border-radius: 20px !important;
}

button a {
  text-decoration: none;
  color: rgb(78, 159, 61);
}

button:active{
  background-color: rgb(78, 159, 61);
  color: rgb(25, 26, 25);
}

.active{
  background-color: rgb(82, 82, 82);
  color: rgb(25, 26, 25);
}

</style>