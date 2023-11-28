<script>
export default {
    name: "FooterBottom",
    data() {
        return {
            imags: [
                {
                    img: "/public/img/footer-facebook.png",
                },
                {
                    img: "/public/img/footer-twitter.png",
                },
                {
                    img: "/public/img/footer-youtube.png",
                },
                {
                    img: "/public/img/footer-pinterest.png",
                },
                {
                    img: "/public/img/footer-periscope.png",
                },
            ]
        }
    },
    mounted() {
        console.log("Componente FooterBottom caricato");
    }
}
</script>

<template>
<div class="footer-bottom text-light" >
    <div class="container">
        <div class="row py-5">
            <div class="col-6">
                <a>SIGN-UP NOW!</a>
            </div>
    
            <div class="col-6 d-flex justify-content-end align-items-center">
                <span class="me-3">FOLLOW US</span>
                <img class="mx-2" v-for="img in imags" :src="img.img" alt="">
            </div>
        </div>
    </div>
</div>
</template>

<style scoped>
.footer-bottom {
    background-color: #303030;;
}

a {
    text-decoration: none;
    padding: 1rem;
    border: 2px solid #3776E2;
    font-weight: bolder;
}

a:hover {
    color: black;
    border-color: white;
    background-color: #3776E2;
}

span {
    color: #3776E2;
    font-weight: bolder;
    transition: 0.4s;
}
</style>