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
    .footer-menu {
        display: flex;
        flex-direction: column;
        align-items: flex-start;

        h4 {
            font-weight: 700;
            font-size: 12px;
            line-height: 26px;
            color: var(--service-color);
            border-bottom: 1px solid var(--rose);
        }
    }

</style>
