<template>
    <div class="testimonials">
        <div class="image">
            <img src="/assets/img/ellipse.png" alt="">
            <img src="/assets/img/quotes.svg" alt="">
        </div>
        <div class="content">
            <div class="container">
                <img src="/assets/img/arrow.svg" alt="">
                <blockquote>Lectus arcu bibendum at varius. Adipiscing
                    <br>diam donec adipiscing tristique.
                </blockquote>
                <img src="/assets/img/arrow-rose.svg" alt="">
            </div>
        </div>
        <div><span>Kerry Johnes</span> - Some Company</div>
    </div>
</template>

<script>
    export default {
        name: "Testimonials"
    }
</script>

<style lang="scss" scoped>
    @import "../assets/scss/mixin";

    .testimonials {
        background-image: url("/assets/img/faces.png");
        background-repeat: no-repeat;
        background-color: var(--service-color);
        margin-top: 306px;
        padding: 0 16px 136px;
        background-size: 100%;

        .image {
            display: flex;
            justify-content: flex-start;
            align-items: center;
            flex-direction: column;

            img:first-child {
                margin-top: -126px;

                @include tablet-landscape {
                    width: 36%;
                }
            }

            img:last-child {
                margin-top: -32px;
            }
        }

        .content {

            .container {
                display: flex;
                justify-content: space-between;
                align-items: center;
                padding: 116px 0 30px;

                img {
                    border-radius: 50%;
                    padding: 0 12px;
                    width: 36px;
                    height: 36px;
                    border: 1px solid var(--rose);

                    &:first-child {
                        background-color: var(--rose);
                    }
                }
            }

            blockquote {
                font-style: italic;
                font-size: 36px;
                line-height: 64px;
                text-align: center;
                color: var(--black);

                @include tablet-landscape {
                    font-size: 31px;
                }
            }
        }

        div {
            text-align: center;
            font-size: 18px;
            line-height: 29px;

            span {
                font-weight: 800;
                font-size: 18px;
                line-height: 29px;
                color: var(--rose);
            }
        }

    }

</style>
