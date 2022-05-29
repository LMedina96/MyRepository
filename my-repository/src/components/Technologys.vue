<template>
<div>
    <h2>{{title}}</h2>

    <ul class="technologys">
        <li v-for="item in items" :key="item.id">
            <img :src="item.img" :alt="item.alt">
            <p>{{item.name}}</p>
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
                    img: "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg",
                    alt: "Html5 Icono",
                    name: "HTML5",
                },
                {
                    id: 2,
                    img: "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg",
                    alt: "Css3 Icono",
                    name: "CSS3",
                },
                {
                    id: 3,
                    img: "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg", 
                    alt: "JavaScript Icono",
                    name: "JavaScript",
                },
                {
                    id: 4,
                    img: "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vuejs/vuejs-original.svg", 
                    alt: "VueJs Icono",
                    name: "Vue Js",
                },
                {
                    id: 5,
                    img: "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg", 
                    alt: "Python Icono",
                    name: "Python"
                },
                {
                    id: 6,
                    img: "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg", 
                    alt: "React Icono",
                    name: "React"
                },
                {
                    id: 7,
                    img: "https://cdn.jsdelivr.net/gh/devicons/devicon/icons/angularjs/angularjs-original.svg", 
                    alt: "Angular Icono",
                    name: "Angular"
                },
            ]
        }
    }
}
</script>


<style scoped>

.technologys{
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    margin: 0 auto;
    padding: 0;
}

img{
    width: 100px;
    height: 100px;
}

ul li{
    list-style: none;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    margin: 1rem;
}

</style>