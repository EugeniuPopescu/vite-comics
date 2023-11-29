<script>
import AppJumbo from './AppJumbo.vue';

export default {
    components: {
        AppJumbo
    },
    name: "Content",
    mounted() {
        console.log("Componente Content caricato");
    }
}
    
</script>

<template>
<AppJumbo />
</template>

<style scoped>

</style>