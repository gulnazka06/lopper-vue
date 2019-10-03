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

    .copyright {
        background-color: var(--footer-bg-color);
        padding: 64px 0 124px;

        .container {

            display: flex;
            justify-content: center;
            align-items: center;

            span {
                color: var(--service-color);
                font-size: 12px;
                line-height: 19px;
            }
        }
    }
</style>
