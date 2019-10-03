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
ul {
    display: flex;
    flex-direction: column;
    margin-top: 34px;

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
        }
    }
}
</style>
