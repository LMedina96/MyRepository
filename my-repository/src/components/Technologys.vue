<template>
<div>
    <h2>{{title}}</h2>

    <ul class="technologys">
        <li v-for="item in items" :key="item.id">
            <img :src="item.img" :alt="item.alt">
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
        return{
            items: [
                {   
                    id: 1,
                    img: "https://via.placeholder.com/120",
                    alt: "mockup1",
                },
                {
                    id: 2,
                    img: "https://via.placeholder.com/120",
                    alt: "mockup2"
                },
                {
                    id: 3,
                    img: "https://via.placeholder.com/120", 
                    alt: "mockup3"
                },
                {
                    id: 4,
                    img: "https://via.placeholder.com/120", 
                    alt: "mockup4"
                },
                {
                    id: 5,
                    img: "https://via.placeholder.com/120", 
                    alt: "mockup5"
                },
            ]
        }
    }
}
</script>


<style scoped>

ul li{
    list-style: none;
    display: inline-block;
    margin: 0 10px;
}

</style>