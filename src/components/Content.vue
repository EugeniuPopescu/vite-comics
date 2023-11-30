<script>
import AppJumbo from './AppJumbo.vue';
import AppCard from './AppCard.vue';

export default {
    components: {
        AppJumbo,
        AppCard
    },
    name: "Content",
    data() {
        return {
            cards: [
                {
                thumb: "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                price: "$19.99",
                series: "Action Comics",
                type: "comic book",
                },
                {
                thumb: "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                price: "$3.99",
                series: "American Vampire 1976",
                type: "comic book",
                },
                {
                thumb: "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                price: "$16.99",
                series: "Aquaman",
                type: "graphic novel",
                },
                {
                thumb: "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                price: "$2.99",
                series: "Batgirl",
                type: "comic book",
                },
                {
                thumb: "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                price: "$3.99",
                series: "Batman",
                type: "comic book",
                },
                {
                thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                price: "$2.99",
                series: "Batman Beyond",
                type: "comic book",
                },
                {
                thumb: "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                price: "$3.99",
                series: "Batman/Superman",
                type: "comic book",
                },
                {
                thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                price: "$4.99",
                series: "Batman/Superman Annual",
                type: "comic book",
                },
                {
                thumb: "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                price: "$5.99",
                series: "Batman: The Joker War Zone",
                type: "comic book",
                },
                {
                thumb: "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                price: "$6.99",
                series: "Batman: Three Jokers",
                type: "comic book",
                },
                {
                thumb: "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                price: "$4.99",
                series: "Batman: White Knight Presents: Harley Quinn",
                type: "comic book",
                },
                {
                thumb: "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                price: "$16.99",
                series: "Catwoman",
                type: "graphic novel",
                },
            ]
        }
    },
    mounted() {
        console.log("Componente Content caricato");
    }
}
    
</script>

<template>
    <AppJumbo />
    <div class="content">
        <div class=" container position-relative">
            <!-- btn load more -->
            <div class="pb-5">
                <a class="series">CURRENT SERIES</a>
            </div>
            
    
            <!-- card render -->
            <div class="d-flex flex-wrap justify-content-between align-items-center">
                <AppCard :image="card.thumb" :title="card.series" v-for="card in cards"/>
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
.content {
    background-color: #1C1C1C;;
}

a {
    font-size: small;
    font-weight: 500;
    text-decoration: none;
    color: lightgray;
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