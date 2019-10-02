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
    .newsletter {
        padding: 130px 0;

        .container {
            display: flex;
            flex-direction: column;
            align-items: center;

            h5 {
                font-weight: 500;
                font-size: 18px;
                line-height: 27px;
                text-align: center;
                color: var(--grey);
                margin: 45px 0;
            }

            div {
                display: flex;
                align-items: center;
                border-bottom: 3px solid var(--header-color);
                max-width: 558px;
                width: 100%;

                input {
                    font-weight: 700;
                    font-size: 18px;
                    line-height: 37px;
                    letter-spacing: 4px;
                    color: var(--input-color);
                    border: none;
                    width: 100%;
                    max-width: 332px;
                    padding-left: 18px;
                }

                button {
                    background-image: var(--button-bg-color);
                    font-weight: 700;
                    font-size: 12px;
                    line-height: 26px;
                    display: flex;
                    align-items: center;
                    letter-spacing: 6px;
                    color: var(--rose);
                    max-width: 226px;
                    width: 100%;
                    border: none;
                    padding-left: 27px;

                    img {
                        border-radius: 50%;
                        padding: 0 12px;
                        width: 36px;
                        height: 36px;
                        border: 1px solid var(--rose);
                        margin-left: 20px;
                    }
                }
            }
        }
    }
</style>
