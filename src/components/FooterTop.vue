<script>
export default {
    name: "FooterTop",
    props: {
        shopCards: Object
    },
    data() {
        return {
        }
    },
    methods() {
    },
    mounted() {
        console.log("Componente FooterTop caricato");
    }
}
</script>

<template>
<div class="footer-top text-light" >
    <div class="container d-flex justify-content-between align-items-center px-4">
        <!-- card render -->
        <div 
        v-for="card in shopCards"
        class="my-5">
            <img :src="card.img" alt="">
            <a class="mx-2">{{ card.text.toLocaleUpperCase() }}</a>
        </div>

    </div>
</div>
</template>

<style scoped>
.footer-top {
    background-color: #3980F1;;
}

img {
    width: 3rem;
}

a {
    text-decoration: none;
    color: white;
}
</style>