<template>
    <div class="newsletter">
        <div class="container">
            <h3>Subscribe to our newsletter</h3>
            <h5>Cras pulvinar mattis nunc sed blandit.</h5>
            <div>
                <input type="text" placeholder="ENTER EMAIL">
                <button>SUBSCRIBE
                    <img src="/assets/img/arrow-rose.svg" alt="">
                </button>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Newsletter"
    }
</script>

<style lang="scss" scoped>
    @import "../assets/scss/mixin";

    .newsletter {
        padding: 130px 0;

        @include mobile {
            padding: 100px 0;
        }

        .container {
            display: flex;
            flex-direction: column;
            align-items: center;

            h5 {
                text-align: center;
                color: var(--grey);
                margin: 45px 0;

                @include mobile {
                    margin: 30px 0;
                }
            }

            h3 {
                @include mobile {
                    font-size: 44px;
                }
            }

            div {
                display: grid;
                grid-template-columns: 2fr 1fr;
                max-width: 558px;
                width: 100%;

                @include mobile {
                    grid-template-columns: 1fr;
                }

                input {
                    border-style: solid;
                    border-color: var(--footer-bg-color);
                    border-width: 1px 0 1px 1px;
                    font-weight: 700;
                    line-height: 37px;
                    letter-spacing: 4px;
                    color: var(--input-color);
                    padding-left: 18px;
                    background-color: transparent;
                    border-radius: 0;
                    margin: 0;
                    box-shadow: none;

                    @include mobile {
                        border-width: 1px 1px 0;
                    }
                }

                button {
                    background: transparent;
                    font-weight: 700;
                    font-size: 12px;
                    display: flex;
                    justify-content: center;
                    align-items: center;
                    color: var(--rose);
                    letter-spacing: .6px;
                    width: 100%;
                    border: 1px solid var(--rose);
                    padding: 15px 10px;
                    margin: 0;

                    img {
                        width: 16px;
                        height: 16px;
                        margin-left: 10px;
                    }
                }
            }
        }
    }
</style>
