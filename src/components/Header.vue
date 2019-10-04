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
    @import "../assets/scss/mixin";

    header {
        background-image: url("/assets/img/bg-header.png");
        background-repeat: no-repeat;
        background-size: cover;


        .content {
            padding: 120px 0;

            @include mobile {
                padding: 100px 0;
            }

            h1 {

                @include mobile {
                    font-size: 50px;
                }
            }
        }
    }
</style>
