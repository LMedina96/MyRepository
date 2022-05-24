<template>
  <div>
    <h2>{{ title }}</h2>
    <div class="row">
      <div id="photo">
        <img
          src="../resources/images/mypicturefinal.jpg"
          alt="Cargando imagen..."
        />
      </div>
      <div class="col-8">
        <p class="textBiography">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Sed
          perspiciatis, a dolores fugiat quos molestias blanditiis nulla illo
          quod reprehenderit, rem ipsam beatae repudiandae facere, quia
          distinctio amet ratione placeat optio vitae magni incidunt. Fuga
          architecto nostrum dolorem voluptatum ipsa, corporis repellat
          reprehenderit sint animi perferendis deserunt mollitia necessitatibus
          suscipit id natus et omnis temporibus, autem quo consectetur,
          molestiae voluptate ab! Quae nam in quam quasi delectus tempora sunt
          neque necessitatibus. Id ducimus, veritatis nihil accusamus eius
          aliquam fuga nulla voluptatem reiciendis porro deleniti quae animi
          illum iusto quo dolorum est a dignissimos totam vel harum consequuntur
          eveniet. Distinctio iste soluta inventore dolorum vitae facilis ipsum
          non animi aliquam nisi ut illo, mollitia quod blanditiis quae
          deleniti. Tempore nobis itaque fugit error consectetur commodi ullam
          ratione ex culpa, obcaecati similique sapiente quisquam tenetur nihil
          totam debitis, mollitia quam magni non veniam autem? Aut deleniti quis
          minus quod magnam, temporibus veniam. Alias commodi doloribus tempora
          itaque iure voluptatibus nihil praesentium voluptas! Quis, voluptatem
          laudantium. Ullam impedit sapiente temporibus rerum assumenda. Aliquid
          quae asperiores exercitationem deleniti animi odit tempore ad
          dignissimos consectetur a? Eius quae similique hic minima, dolorem
          cupiditate repellat sunt! Illum animi quasi soluta, fugiat aspernatur
          culpa! Accusamus, eligendi cumque.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: String,
  },
};
</script>

<style>

.row{
  display: flex;
  flex-wrap: wrap;
  justify-content:space-between
}

#photo{
  width: 250px;
  height:400px;
  margin: auto 0;
  padding: 0;
}

#photo img{
  object-fit: cover;
  width:100%;
  height:100%;
}
</style>