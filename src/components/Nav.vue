<template>
    <nav class="container">
        <img src="../assets/img/Logo.svg" alt="">
        <ul>
            <li><a href="">Home</a></li>
            <li><a href="">Services</a></li>
            <li><a href="">Work</a></li>
            <li><a href="">About</a></li>
        </ul>
        <a href="">
            <img src="../assets/img/mobile.svg" alt="">
            <span>(01) 666 - 693 - 456</span>
        </a>
        <button><img src="../assets/img/menu.svg" alt=""></button>
    </nav>
</template>

<script>
    export default {
        name: "Nav"
    }
</script>

<style lang="scss" scoped>
    nav {
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 60px 0 36px;

        ul {
            display: flex;

            li {
                padding: 0 27px;
            }
        }

        a {
            text-decoration: none;
            display: flex;
            align-items: center;

            img {
                margin-right: 18px;
            }
        }

        button {
            border: none;
        }
    }

</style>
