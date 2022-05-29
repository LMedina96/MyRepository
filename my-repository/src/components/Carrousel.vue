<template>
   <div class="container carrousel">
        <button
          v-for="carrouselButton in CarrouselButtonsNumber"
          :key="carrouselButton"
          @click="getButtonIndex()">
        </button>
      </div>
</template>

<script>
export default {
    props: {
        CarrouselButtonsNumber: Number,
    },

    method: {
        getButtonIndex(index) {
            this.$emit("get-button-index", index);
            console.log(index)
        },
    }
}
</script>

<style>
</style>