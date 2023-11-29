<script>
export default {
    name: "AppJumbo",
    data() {
        return {
        }
    },
    mounted() {
        console.log("Componente AppJumbo caricato");
    }
}
</script>

<template>
    <div class="jumbo">dfhy</div>
</template>

<style scoped>
.jumbo {
    background-image: url(/img/jumbotron.jpg);
    background-size: cover;
    height: 25rem;
}
</style>
