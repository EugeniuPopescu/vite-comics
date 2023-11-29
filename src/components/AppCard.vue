<script>
export default {
    name: "AppCard",
    props: {
        dcCards: Object
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
<div class="appCard text-light" >
    <div class="container position-relative">
        <!-- btn load more -->
        <div class="pb-5">
            <a class="series">CURRENT SERIES</a>
        </div>
        

        <!-- card render -->
        <div class="d-flex flex-wrap justify-content-between align-items-center">
            <div 
            v-for="card in dcCards"
            class="dcCard d-flex flex-column my-4">
                <img :src="card.thumb" alt="">
                <a class="pt-2">{{ card.series.toLocaleUpperCase() }}</a>
            </div>
        </div>

        <!-- btn load more -->
        <div class="d-flex justify-content-center py-5">
            <div>
                <a class="load">LOAD MORE</a>
            </div>
        </div>
    
    </div>
</div>
</template>

<style scoped>
.appCard {
    background-color: #1C1C1C;;
}

img {
    width: 12rem;
    height: 12rem;
}

a {
    font-size: small;
    font-weight: 500;
    text-decoration: none;
    color: lightgray;
}

.dcCard {
    width: 15%;
}

.load {
    padding: 1rem 4rem;
    background-color: #3776E2;
    font-weight: bold;
}

.load:hover {
    color: #3776E2;
    background-color: white;
    transition: 0.3s;
}

.series {
    padding: 1rem 2rem;
    background-color: #3776E2;
    font-weight: 600;
    font-size: x-large;

    position: absolute;
    top: -2rem;
    left: -1rem;
}

.series:hover {
    color: #3776E2;
    background-color: white;
    transition: 0.3s;
}
</style>