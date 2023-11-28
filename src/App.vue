<script>
import AppHeader from './components/AppHeader.vue'
import Content from './components/Content.vue'
import AppFooter from './components/AppFooter.vue'

export default {
	components: {
		AppHeader,
		Content,
		AppFooter,
	}
}
</script>

<template>
	<!-- component AppHeader -->
	<AppHeader />

	<main>
	<!-- component Content -->
		<Content />
	</main>

	<!-- component AppFooter --> 
	<AppFooter />
</template>

<style scoped></style>
