<template>
    <nav class="container">
        <img src="/assets/img/Logo.svg" alt="">
        <ul :class="{ open: isOpen }">
            <li><a href="">Home</a></li>
            <li><a href="">Services</a></li>
            <li><a href="">Work</a></li>
            <li><a href="">About</a></li>
        </ul>
        <a href="tel:89509488859" class="phone">
            <img src="/assets/img/mobile.svg" alt="">
            <span>+7 (950) 948-88-59</span>
        </a>
        <button v-on:click="onMenuClick"><img src="/assets/img/menu.svg" alt=""></button>
    </nav>
</template>

<script>
    export default {
        name: "Nav",
        data() {
            return {
                isOpen: false,
            };
        },
        methods: {
            onMenuClick() {
                this.isOpen = !this.isOpen;
            }
        }
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
        background-color: var(--white);

        @include mobile {
            position: sticky;
            top: 0;
            z-index: 999;
            padding-top: 20px;
            padding-bottom: 20px;
        }

        ul {
            display: flex;

            @include mobile {
                position: absolute;
                top: 100%;
                width: 100vw;
                left: 0;
                background-color: var(--white);
                opacity: 0;
                transition: .3s;
                visibility: hidden;
                transform: translateY(-100%);
                padding-bottom: 20px;
                flex-wrap: wrap;

                &.open {
                    opacity: 1;
                    visibility: visible;
                    transform: translateY(0%);
                }
            }

            li {
                padding: 0 27px;
            }
        }

        a {
            text-decoration: none;
            display: flex;
            align-items: center;

            @include mobile {
                &.phone {
                    display: none;
                }
            }

            @include tablet-portrait {
                letter-spacing: 1px;
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
