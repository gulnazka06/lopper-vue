<template>
<div class="service">
    <div class="container">
        <img src="/assets/img/map.png" alt="">
        <h4>WE ARE AMAZING</h4>
        <h3>Our Services</h3>
        <p>Quam adipiscing vitae proin sagittis nisl rhoncus mattis
            <br>rhoncus urna. Quam elementum pulvinar etiam non. Eu
            <br>consequat.</p>
        <div class="list">
            <ServiceItem
                    title="Chopping heads"
                    description="Tincidunt lobortis feugiat vivamus at augue eget. Risus feugiat in ante metus dictum. Amet aliquam id diam maecenas."
                    imgURL="/assets/img/chopping-icon.svg"
            ></ServiceItem>
            <ServiceItem
                    title="Atom dev"
                    description="Eget nulla facilisi etiam dignissim diam quis enim lobortis scelerisque. Eu feugiat pretium nibh ipsum consequat nisl vel pretium. "
                    imgURL="/assets/img/atom.svg"
                    type="rose"
            ></ServiceItem>
            <ServiceItem
                    title="Do you even try?"
                    description="Eu augue ut lectus arcu bibendum at. Pellentesque nec nam aliquam sem et tortor consequat."
                    imgURL="/assets/img/castle.svg"
                    type="orange"
            ></ServiceItem>
            <ServiceItem
                    title="Justice for Metallica "
                    description="Id venenatis a condimentum vitae. Magna fermentum iaculis eu non diam phasellus vestibulum lorem. Tortor dignissim convallis aenean et."
                    imgURL="/assets/img/justice.svg"
                    type="orange"
            ></ServiceItem>
            <ServiceItem
                    title="Better than the Dude"
                    description="Sollicitudin ac orci phasellus egestas tellus rutrum tellus pellentesque. Malesuada fames ac turpis egestas sed."
                    imgURL="/assets/img/dude.svg"
            ></ServiceItem>
            <ServiceItem
                    title="Hmmmm"
                    description="Integer quis auctor elit sed vulputate mi. Semper auctor neque vitae tempus. Vulputate odio ut enim blandit volutpat maecenas volutpat."
                    imgURL="/assets/img/hm.svg"
                    type="rose"
            ></ServiceItem>
        </div>
    </div>
</div>
</template>

<script>
    import ServiceItem from "@/components/ServiceItem";
    export default {
        name: "Services",
        components: {
            ServiceItem: ServiceItem
        }
    }
</script>

<style lang="scss" scoped>
    @import "../assets/scss/mixin";

    .service {
        background-image: url("/assets/img/service-bg.png");
        position: relative;
        padding-bottom: 98px;

        .container {
            display: flex;
            flex-direction: column;
            align-items: center;

            img {
                position: absolute;
                top: 122px;
                left: 50%;
                transform: translateX(-50%);
                width: 100%;

                @include mobile {
                    top: 60px;
                }
            }

            h4 {
                margin: 262px 0 12px;

                @include mobile {
                    margin: 100px 0 12px;
                }
            }

            h3 {
                color: var(--service-color);
            }

            p {
                font-weight: 700;
                font-size: 18px;
                line-height: 29px;
                text-align: center;
                color: var(--service-color);
                margin: 23px 0 51px;
            }

            .list {
                display: grid;
                grid-template-columns: 1fr 1fr 1fr;
                grid-gap: 70px;

                @include mobile {
                    grid-template-columns: 1fr;
                    grid-gap: 40px;
                }
            }
        }
    }
</style>
