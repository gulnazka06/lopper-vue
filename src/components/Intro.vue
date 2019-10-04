<template>
    <div class="intro">
        <div class="container">
            <h4>WHAT WE DO</h4>
            <p>Apparently we had reached a great height in the
                <br>atmosphere, for the sky was a dead black, and the stars
                <br>had ceased to twinkle.</p>
            <div class="prizes">
                <div class="prize">
                    <div>15+</div>
                    <span>Nobel prizes</span>
                </div>
                <div class="prize">
                    <div style="color: var(--purple)">33</div>
                    <span>Nobel prizes</span>
                </div>
                <div class="prize">
                    <div style="color: var(--green)">12</div>
                    <span>Nobel prizes</span>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Intro"
    }
</script>

<style lang="scss" scoped>
    @import "../assets/scss/mixin";

    .intro {

        .container {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin-bottom: -76px;

            @include mobile {
                margin-bottom: -44px;
            }

            h4 {
                margin: 108px 0 15px;
            }

            p {
                font-size: 27px;
                line-height: 40px;
                color: var(--black);
                text-align: center;
                padding-bottom: 90px;

                @include mobile {
                    font-size: 20px;
                    line-height: 32px;
                }
            }
        }

        .prizes {
            display: flex;
            width: 100%;
            justify-content: space-between;

            .prize {
                display: flex;
                flex-direction: column;
                align-items: center;
                z-index: 99;

                div {
                    font-weight: 700;
                    font-size: 99px;
                    line-height: 118px;
                    color: var(--rose);

                    @include mobile {
                        font-size: 46px;
                        line-height: 46px;
                    }
                }

                span {
                    font-weight: 700;
                    font-size: 12px;
                    line-height: 26px;
                    letter-spacing: 6px;
                    color: var(--service-color);

                    @include mobile {
                        letter-spacing: 1px;
                    }
                }
            }
        }
    }

</style>
