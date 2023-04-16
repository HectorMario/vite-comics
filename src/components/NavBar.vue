<script setup>
    const list = [
        {
            option : "CHARACTERS",
            active : false
        },
        {
            option : "COMICS",
            active : true,
        },
        {
            option : "TV",
            active : false
        }, {
            option : "GAMES",
            active : false
        }, {
            option : "COLLECTIBLES",
            active : false
        },
        {
            option : "VIDEOS",
            active : false
        }, {
            option : "FANS",
            active : false
        }, {
            option : "NEWS",
            active : false
        },
        {
            option : "SHOP",
            active : false
        }
    ]
</script>

<template>
    <div class="white-container">
        <div class="container">
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="" id="logo">
            </div>
            <div class="options">
                <ul>
                    <li v-for="option in list" :class="option.active ? 'active' : ''">
                        {{ option.option }}
                    </li>
                </ul>
            </div>
        </div>
    </div>
</template>

<style lang="scss">
    @import 'style/style-nav.scss'
</style>