<script>
export default {
    name: "AppCard",
    props: {
        image: String,
        title: String,
    },
    data() {
        return {
        }
    },
    methods() {
        
    },
    mounted() {
        console.log("Componente AppCard caricato");
    }
}
</script>

<template>

    <!-- card render -->
    <div class="dcCard">
        <div class=" d-flex flex-column my-4">
            <img :src="image" alt="">
            <a class="pt-2">{{ title.toUpperCase() }}</a>
        </div>
    </div>

</template>

<style scoped>
.dcCard {
    width: calc(100% / 6);
}

img {
    width: 12rem;
    height: 15rem;
}

a {
    font-size: small;
    font-weight: 500;
    text-decoration: none;
    color: lightgray;
}
</style>