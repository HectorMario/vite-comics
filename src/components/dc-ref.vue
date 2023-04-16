<script setup>
import images from 'images/footer-facebook.png'
import images2 from 'images/footer-periscope.png'
import images3 from 'images/footer-pinterest.png'
import images4 from 'images/footer-twitter.png'
import images5 from 'images/footer-youtube.png'
const links = {
                "DC COMICS": [
                    {
                        name: "Characters",
                        url: "#"
                    },
                    {
                        name: "Comics",
                        url: "#"
                    },
                    {
                        name: "Movies",
                        url: "#"
                    },
                    {
                        name: "TV",
                        url: "#"
                    },
                    {
                        name: "Games",
                        url: "#"
                    },
                    {
                        name: "Videos",
                        url: "#"
                    },
                    {
                        name: "News",
                        url: "#"
                    }
                ],
                "SHOP": [
                    {
                        name: "Shop DC",
                        url: "#"
                    },
                    {
                        name: "Shop DC Collectibles",
                        url: "#"
                    }
                ],

                "DC": [
                    {
                        name: "Terms Of Use",
                        url: "#"
                    },
                    {
                        name: "Privacy policy(New)",
                        url: "#"
                    },
                    {
                        name: "Ad Choices",
                        url: "#"
                    },
                    {
                        name: "Advertising",
                        url: "#"
                    },
                    {
                        name: "Jobs",
                        url: "#"
                    },
                    {
                        name: "Subscriptions",
                        url: "#"
                    },
                    {
                        name: "Talet Workshops",
                        url: "#"
                    },
                    {
                        name: "CPSC Certificates",
                        url: "#"
                    },
                    {
                        name: "Ratings",
                        url: "#"
                    },
                    {
                        name: "Shop Help",
                        url: "#"
                    },
                    {
                        name: "Contact Us",
                        url: "#"
                    }
                ],
                "SITES": [
                    {
                        name: "DC",
                        url: "#"
                    },
                    {
                        name: "MAD Magazine",
                        url: "#"
                    },
                    {
                        name: "DC Kids",
                        url: "#"
                    },
                ]
                
            }
const social = [
    {
        name: `${images}`
    },
    {
        name: `${images2}`
    }, 
    {
        name: `${images3}`
    },
    {
        name: `${images4}`
    },
    {
        name: `${images5}`
    },
]

</script>

<template>
   <div class="backgraund">
        <div class="container">
            <div class="left">
                <ul v-for=" (sites,key)  in links">
                    <strong>
                        {{ key }}
                    </strong>
                    <li v-for="link in sites">
                        <a href="">
                            {{ link.name }}
                        </a>
                    </li>
                </ul>
            </div>
            <div class="right">
                <img src="../assets/img/dc-logo-bg.png" alt="" id="dc-logo">
            </div>
        </div>
    </div>
    <div class="contact">
        <div class="container">
            <div class="left-contact">
                <button>
                    SIGN-UP NOW!
                </button>
            </div>
            <div class="right-contact">
                <strong>
                    FOLLOW US
                </strong>
                <ul>
                    <li v-for="image in social">
                        <a href="">
                            <img :src="image.name" alt="" id="social">
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style lang="scss">
    @import 'style/fotter.scss';
</style>