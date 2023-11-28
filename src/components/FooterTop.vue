<script>
export default {
    name: "FooterTop",
    data() {
        return {
            cards: [
                {
                    img: "/public/img/buy-comics-digital-comics.png",
                    text: "digital comics",
                },
                {
                    img: "/public/img/buy-comics-merchandise.png",
                    text: "dc merchandise",
                },
                {
                    img: "/public/img/buy-comics-subscriptions.png",
                    text: "subscription",
                },
                {
                    img: "/public/img/buy-comics-shop-locator.png",
                    text: "comic shop locator",
                },
                {
                    img: "/public/img/buy-dc-power-visa.svg",
                    text: "dc power visa",
                },
            ]
        }
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
        v-for="card in cards"
        class="my-4">
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