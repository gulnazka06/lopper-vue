<template>
    <ul class="footer-nav" :class="direction">
        <li v-for="item of list">
            <a href="">
                <img v-if="item.image" :src="item.image" alt="">
                {{ item.name }}
            </a>
        </li>
    </ul>
</template>

<script>
    export default {
        name: "FooterNav",
        props: ['list', 'direction']
    }
</script>

<style lang="scss" scoped>
    @import "../assets/scss/mixin";

ul {
    display: flex;
    flex-direction: column;
    margin-top: 34px;

    @include mobile {
        margin-top: 22px;
    }

    li {

        a {
            text-decoration: none;
            font-weight: bold;
            font-size: 12px;
            line-height: 28px;
            letter-spacing: 1px;
            color: var(--service-color);

            img {
                margin-right: 18px;
            }
        }
    }

    &.horizontal {
        flex-direction: row;

        img {
            margin-right: 42px;

            @include tablet-portrait {
                margin-bottom: 26px;
            }
        }

        @include tablet-portrait {
            display: grid;
            grid-template-columns: .5fr .5fr .5fr;
        }
    }
}
</style>
