<template>
    <nav class="container">
        <img src="/assets/img/Logo.svg" alt="">
        <ul>
            <li><a href="">Home</a></li>
            <li><a href="">Services</a></li>
            <li><a href="">Work</a></li>
            <li><a href="">About</a></li>
        </ul>
        <a href="">
            <img src="/assets/img/mobile.svg" alt="">
            <span>(01) 666 - 693 - 456</span>
        </a>
        <button><img src="/assets/img/menu.svg" alt=""></button>
    </nav>
</template>

<script>
    export default {
        name: "Nav"
    }
</script>

<style lang="scss" scoped>
    @import "../assets/scss/mixin";

    nav {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding-top: 60px;
        padding-bottom: 36px;

        ul {
            display: flex;

            @include mobile {
                display: none;
            }

            li {
                padding: 0 27px;
            }
        }

        a {
            text-decoration: none;
            display: flex;
            align-items: center;

            @include tablet-portrait {
                letter-spacing: 1px;
            }

            @include mobile {
                display: none;
            }

            img {
                margin-right: 18px;

                @include tablet-portrait {
                    margin-right: 9px;
                }
            }
        }

        button {
            border: none;
            background-color: transparent;
        }
    }

</style>
