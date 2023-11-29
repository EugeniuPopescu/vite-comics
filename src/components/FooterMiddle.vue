<script>
export default {
    name: "FooterMiddle",
    data() {
        return {
            comics: [
                {
                    text: "Characters",
                },
                {
                    text: "Comics",
                },
                {
                    text: "Movies",
                },
                {
                    text: "TV",
                },
                {
                    text: "Games",
                },
                {
                    text: "Videos",
                },
                {
                    text: "News",
                }
            ],
            shops: [
                {
                    text: "Characters",
                },
                {
                    text: "Comics",
                },
                
            ],
            dcs: [
                {
                    text: "Terms Of Use",
                },
                {
                    text: "Privacy policy (New)",
                },
                {
                    text: "Ad Choices",
                },
                {
                    text: "Advertising",
                },
                {
                    text: "Jobs",
                },
                {
                    text: "Subscriptions",
                },
                {
                    text: "Talent Workshop",
                },
                {
                    text: "CPSC Certificates",
                },
                {
                    text: "Ratings",
                },
                {
                    text: "Shop Help",
                },
                {
                    text: "Contact Us",
                }
            ],
            sites: [
                {
                    text: "DC",
                },
                {
                    text: "MAD Magazine",
                },
                {
                    text: "DC Kids",
                },
                {
                    text: "DC Universe",
                },
                {
                    text: "DC Power Visa",
                }
            ]
        }
    },
    mounted() {
        console.log("Componente FooterMiddle caricato");
    }
}
</script>

<template>
<div class="footer-middle" >
    <div class="container">
        <div class="row">
            <div class="col-4 d-flex justify-content-between py-5">
                <!-- row 1 -->
                <div>
                    <div>
                        <span class="text-light fs-5">DC Comics</span>
                        <ul class="p-0">
                            <li class="text-secondary" v-for="comic in comics"><a href="#">{{ comic.text }}</a></li>
                        </ul>
                    </div>

                    <div>
                        <div>
                            <span class="text-light fs-5">Shop</span>
                            <ul class="p-0">
                                <li class="text-secondary" v-for="shop in shops"><a href="#">{{ shop.text }}</a></li>
                            </ul>
                        </div>
                    </div>

                </div>

                <!-- row 2 -->
                <div>
                    <div>
                        <span class="text-light fs-5">DC</span>
                        <ul class="p-0">
                            <li class="text-secondary" v-for="dc in dcs"><a href="#">{{ dc.text }}</a></li>
                        </ul>
                    </div>
                </div>

                <!-- row 3 -->
                <div>
                    <div>
                        <span class="text-light fs-5">SITES</span>
                        <ul class="p-0">
                            <li class="text-secondary" v-for="site in sites"><a href="#">{{ site.text }}</a></li>
                        </ul>
                    </div>
                </div>
            </div>

            <!-- DC img -->
            <div class="col-8 d-flex justify-content-end">
                <div class="bgImg"></div>
            </div>
        </div>
    </div>
</div>
</template>

<style scoped>
.footer-middle {
    background-image: url(/public/img/footer-bg.jpg);
}

.bgImg {
    width: 80%;
    background-size: cover;
    background-position: center;
    background-image: url(/img/dc-logo-bg.png);
}

span {
    font-weight: bolder;
}

li {
    list-style: none;
}

a {
    text-decoration: none;
    color: gray;
    font-size: small;
}

a:hover {
    color: white;
}
</style>