<template>
  <div class="container">
    <h2>{{ title }}</h2>

    <ul>
      <li class="card" v-for="proyect in proyects" :key="proyect.id">
        <img
          class="card-img-bottom"
          :src="proyect.proyectImage"
          alt="Proyect Image"
        />
        <div class="card-body">
          <h5 class="card-title">{{proyect.proyectTitle}}</h5>
          <p class="card-text">
            {{proyect.proyectDescription}}
          </p>
        </div>
        <div class="card-body">
          <a href="#" class="card-link">Ingresar al sitio</a>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  props: {
    title: String,
  },

  data() {
    return {
      proyects: [
        {
          id: 1,
          proyectImage: "https://via.placeholder.com/300",
          proyectTitle: "Proyecto 1",
          proyectDescription:
            "Lorem ipsum dolor sit amet, sint occaecat cupidatat non proident, sunt in culpa  non proident",
        },
        {
          id: 2,
          proyectImage: "https://via.placeholder.com/300",
          proyectTitle: "Proyecto 2",
          proyectDescription:
            "Lorem ipsum dolor sit amet, sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
        },
        {
          id: 3,
          proyectImage: "https://via.placeholder.com/300",
          proyectTitle: "Proyecto 3",
          proyectDescription:
            "Lorem ipsum dolor sit amet, sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
        },
        {
          id: 4,
          proyectImage: "https://via.placeholder.com/300",
          proyectTitle: "Proyecto 4",
          proyectDescription:
            "Lorem ipsum dolor sit amet, sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
        },
      ],
    };
  },
};
</script>

<style>

ul{
    list-style: none;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}

.card{
    width: 16rem;
    max-height: 400px;
    margin: 1rem;
    background-color: rgb(20, 20, 20);
}

.card img{
    height: 120px;
}

.card a{
    color: white;
}

.card p{
    font-size: 14px;
    height: 150px;
}

</style>