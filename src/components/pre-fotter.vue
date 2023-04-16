<script setup>
import images from "images/buy-comics-digital-comics.png"
import images2 from "images/buy-comics-merchandise.png"
import images3 from "images/buy-comics-shop-locator.png"
import images4 from "images/buy-comics-subscriptions.png"
import images5 from "images/buy-dc-power-visa.svg"


const options = [
    {
        img: `${images}`,
        text: "DIGITAL COMICS"
    },
    {
        img: `${images2}`,
        text: "DC MERCHANDISE"
        
    }, 
    {
        img: `${images3}`,
        text: "SUBCRIPTION"
        
    },
     {
        img: `${images4}`,
        text: "COMIC SHP LOCATOR"
        
    },
    {
        img: `${images5}`,
        text: "DC POWER VISA"
        
    },
]
</script>

<template>
    <div class="blue">
        <div class="container">
            <ul>
                <li v-for="buy in options">
                    <a href="">
                        <img id="buys" :src="buy.img" alt="">
                        <p>{{ buy.text }}</p>
                    </a>
                </li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss">
    @import 'style/style-preFotter.scss'
</style>