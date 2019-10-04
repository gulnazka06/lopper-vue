<template>
    <div class="footer-menu">
        <h4>{{ title }}</h4>
        <slot></slot>
    </div>
</template>

<script>
    export default {
        name: "FooterMenu",
        props: ['title']
    }
</script>

<style lang="scss" scoped>
    @import "../assets/scss/mixin";

    .footer-menu {
        display: flex;
        flex-direction: column;
        align-items: flex-start;

        @include tablet-portrait {
            margin-bottom: 48px;
        }

        @include mobile {
            margin-bottom: 36px;
        }

        h4 {
            color: var(--service-color);
            border-bottom: 1px solid var(--rose);
        }
    }

</style>
