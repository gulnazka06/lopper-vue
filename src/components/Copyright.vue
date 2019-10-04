<template>
    <div class="copyright">
        <div class="container">
            <span>© 2019 Lopper by mariuszdaniel. All right reserved.</span>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Copyright"
    }
</script>

<style lang="scss" scoped>
    @import "../assets/scss/mixin";

    .copyright {
        background-color: var(--footer-bg-color);
        padding: 64px 0 124px;

        @include mobile {
            padding: 0 0 100px;
        }

        .container {

            display: flex;
            justify-content: center;
            align-items: center;

            @include mobile {
                justify-content: flex-start;
            }

            span {
                color: var(--service-color);
                font-size: 12px;
                line-height: 19px;
            }
        }
    }
</style>
