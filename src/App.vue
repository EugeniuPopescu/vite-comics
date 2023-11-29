<script>
import AppHeader from './components/AppHeader.vue'
import Content from './components/Content.vue'
import AppFooter from './components/AppFooter.vue'

export default {
	components: {
		AppHeader,
		Content,
		AppFooter,
	},
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
}
</script>

<template>
	<!-- component AppHeader -->
	<!-- passo le props -->
	<AppHeader :txtLinks="links" />

	<main>
        <!-- <font-awesome-icon icon="fa-solid fa-user-secret" /> -->
	<!-- component Content -->
		<Content />
	</main>

	<!-- component AppFooter --> 
	<AppFooter />
</template>

<style scoped></style>
