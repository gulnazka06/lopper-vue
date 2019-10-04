<template>
    <div class="section" :class="type">
        <div class="content">
            <h5>{{ order }}</h5>
            <h6>{{ title }}</h6>
            <p>{{ description }}</p>
        </div>
        <div class="image">
            <img :src="imgURL" alt="">
            <div class="colored-shape"></div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "WorkList",
        props: [ 'order', 'title', 'description', 'type', 'imgURL']
    }
</script>

<style lang="scss" scoped>
    @import "../assets/scss/mixin";

    .section {
        display: grid;
        grid-template-columns: 1fr 1fr;
        justify-items: center;
        align-items: center;
        grid-gap: 20px;
        position: relative;
        margin-bottom: 126px;
        width: 100%;

        @include mobile {
            grid-template-columns: 1fr;
            margin-bottom: 80px;
        }

        .image {
            position: relative;

            img {
                width: 100%;
            }
        }

        .content {
            padding: 0 16px;
            width: 100%;

            h5 {
                font-weight: 700;
                font-size: 18px;
                line-height: 37px;
                letter-spacing: 4px;
                color: var(--rose);
            }

            h6 {
                font-size: 27px;
                line-height: 40px;
                color: var(--black);
                margin: 18px 0;
            }

            p {
                font-size: 18px;
                line-height: 29px;
                color: var(--subscribe-color);
            }
        }

        .colored-shape {
            position: absolute;
            bottom: -108px;
            right: 0;
            z-index: -1;
            border-radius: 0;
            width: 85%;
            height: 110px;
            background-color: var(--rose);

            @include mobile {
                bottom: -40px;
            }
        }

        &.green {

            .content {
                order: 2;

                @include mobile {
                    order: unset;
                }

                h5 {
                    color: var(--green);
                }
            }

            .colored-shape {
                right: unset;
                left: 0;
                background-color: var(--green);
            }
        }

        &.purple {

            h5 {
                color: var(--purple);
            }

            .colored-shape {
                background-color: var(--purple);
            }
        }
    }
</style>
