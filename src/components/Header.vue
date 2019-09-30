<template>
    <header>
        <div class="container">
            <div class="content">
                <h1>Our Services</h1>
                <h2>WE BUILD GREAT BUSINESS </h2>
            </div>
        </div>
    </header>
</template>

<script>
    export default {
        name: "Header",
        components: {}
    }
</script>

<style lang="scss" scoped>
    header {
        background-image: url("../assets/img/bg-header.png");
        background-repeat: no-repeat;

        .content {
            padding: 120px 0;

            h1 {
                font-weight: 500;
                font-size: 54px;
                line-height: 80px;
                color: var(--rose);
            }

            h2 {
                font-weight: 800;
                font-size: 18px;
                line-height: 37px;
                letter-spacing: 4px;
                color: var(--header-color);
            }
        }
    }
</style>
