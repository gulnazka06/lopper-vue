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
    .section {
        display: grid;
        grid-template-columns: 1fr 1fr;
        justify-items: center;
        align-items: center;
        grid-gap: 20px;
        position: relative;
        margin-bottom: 126px;

        .image {
            position: relative;
        }

        .content {
            padding: 0 120px;

            h5 {
                font-weight: 800;
                font-size: 18px;
                line-height: 37px;
                letter-spacing: 4px;
                color: var(--rose);
            }

            h6 {
                font-weight: 500;
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
            width: 607px;
            height: 468px;
            background-color: var(--rose);
        }

        &.green {

            .content {
                order: 2;

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
