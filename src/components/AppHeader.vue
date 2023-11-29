<script>
export default {
    name: "AppHeader",
    // dicchiare le props attraverso array
    // props: ['txtLinks'],

    // dicchiare le props attraverso oggetto, dove va dicchiarato il tipo
    props: {
        txtLinks: Object,
    },
    data() {
        return {
        }
    },
    mounted() {
        console.log("Componente AppHeader caricato");
    }
}
</script>

<template>
<header class="bg-light">
    <div class="container">
        <div class="row">
            <!-- col logo -->
            <div class="col-5">
                <img class="logo my-3" src="/public/img/dc-logo.png" alt="">
            </div>

            <!-- col links -->
            <div class="col-7 d-flex justify-content-between align-items-center">
                <a v-for="link in txtLinks" :href="link.url">{{ link.text.toLocaleUpperCase() }}</a>
            </div>
        </div>
    </div>
</header>

</template>
<style scoped>
.logo {
    width: 5rem;
}

a {
    font-size: medium;
    text-decoration: none;
    font-weight: bold;
    color: dimgray;
}

a::after {
    border-bottom: 1px solid;
}

a:hover {
    color: #3980F1;
}
</style>
