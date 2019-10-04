<template>
<div class="chopping" :class="type">
    <img :src="imgURL" alt="">
    <h5>{{ title }}</h5>
    <p>{{ description }}</p>
</div>
</template>

<script>
    export default {
        name: "ServiceItem",
        // Скоращенная запись:
        // props: ['title', 'description', 'imgURL', 'type']
        // Полная запись:
        props: {
            title: {},
            description: {
                default: 'ad'
            },
            imgURL: {},
            type: {},
        }
    }
</script>

<style lang="scss" scoped>
    .chopping {

        img {
            border-radius: 50%;
            background-color:rgba(var(--green-rgb-color), .1);
            border: 1px solid rgba(var(--green-rgb-color), .25);
            padding: 25px 22px 26px 24px;
            width: 72px;
            height: 72px;
        }

        h5 {
            font-size: 18px;
            line-height: 27px;
            color: var(--green);
            margin: 18px 0 26px;
        }

        p {
            font-size: 16px;
            line-height: 26px;
            color: var(--service-color);
        }

        &.rose {

            img {
                background-color:rgba(var(--rose-rgb-color), .1);
                border: 1px solid rgba(var(--rose-rgb-color), .25);
            }

            h5 {
                color: var(--rose);
            }
        }

        &.orange {

            img {
                background-color:rgba(var(--orange-rgb-color), .1);
                border: 1px solid rgba(var(--orange-rgb-color), .25);
            }

            h5 {
                color: var(--orange-color);
            }
        }
    }
</style>
