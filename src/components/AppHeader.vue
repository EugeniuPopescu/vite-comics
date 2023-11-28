<script>
export default {
    name: "AppHeader",
    data() {
        return {
            links: [
                {
                    text: "characters",
                    url: "#characters",
                },
                {
                    text: "comics",
                    url: "#comics",
                },
                {
                    text: "movies",
                    url: "#movies",
                },
                {
                    text: "tv",
                    url: "#tv",
                },
                {
                    text: "games",
                    url: "#games",
                },
                {
                    text: "collectibles",
                    url: "#collectibles",
                },
                {
                    text: "videos",
                    url: "#videos",
                },
                {
                    text: "fans",
                    url: "#fans",
                },
                {
                    text: "news",
                    url: "#news",
                },
                {
                    text: "shop",
                    url: "#shop",
                },
            ]
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
            <div class="col-4">
                <img class="logo my-2" src="/public/img/dc-logo.png" alt="">
            </div>

            <!-- col links -->
            <div class="col-8 d-flex justify-content-between align-items-center">
                <a v-for="link in links" :href="link.url">{{ link.text.toLocaleUpperCase() }}</a>
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
    text-decoration: none;
    font-weight: bolder;
    color: dimgray;
}

a:hover {
    color: #3980F1;
}
</style>
