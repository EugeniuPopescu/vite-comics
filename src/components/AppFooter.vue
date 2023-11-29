<script>
import FooterTop from './FooterTop.vue';
import FooterMiddle from './FooterMiddle.vue';
import FooterBottom from './FooterBottom.vue';

export default {
	components: {
		FooterTop,
		FooterMiddle,
		FooterBottom,
	},
	data() {
		return {
			cards: [
                {
                    img: "/img/buy-comics-digital-comics.png",
                    text: "digital comics",
                },
                {
                    img: "/img/buy-comics-merchandise.png",
                    text: "dc merchandise",
                },
                {
                    img: "/img/buy-comics-subscriptions.png",
                    text: "subscription",
                },
                {
                    img: "/img/buy-comics-shop-locator.png",
                    text: "comic shop locator",
                },
                {
                    img: "/img/buy-dc-power-visa.svg",
                    text: "dc power visa",
                },
            ]
		}
	}
}
</script>

<template>
    <FooterTop :shopCards="cards" />
    <FooterMiddle />
    <FooterBottom />
</template>

<style scoped>

</style>
