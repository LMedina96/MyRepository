<template>
  <header>
    <h1>{{title}}</h1>
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
          <a href="#">{{buttons[0]}}</a>
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
          <a href="#">{{buttons[1]}}</a>
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
          <a href="#">{{buttons[2]}}</a>
        </button>
      </form>
    </nav>
  </header>
</template>

<script>
export default {
  props: {
    title: String,
    buttons: Array,
  },
};
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
  border: 2px solid rgb(78, 159, 61) !important;
  border-radius: 20px !important;
}

button a{
    text-decoration: none;
    color: rgb(78, 159, 61);
}

</style>