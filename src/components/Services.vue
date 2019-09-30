<template>
<div class="service">
    <div class="container">
        <img src="../assets/img/map.png" alt="">
        <h4>WE ARE AMAZING</h4>
        <h3>Our Services</h3>
        <p>Quam adipiscing vitae proin sagittis nisl rhoncus mattis
            <br>rhoncus urna. Quam elementum pulvinar etiam non. Eu
            <br>consequat.</p>
        <div class="list">
            <ServiceItem></ServiceItem>
            <ServiceItem></ServiceItem>
            <ServiceItem></ServiceItem>
            <ServiceItem></ServiceItem>
            <ServiceItem></ServiceItem>
            <ServiceItem></ServiceItem>
        </div>
    </div>
</div>
</template>

<script>
    import ServiceItem from "@/components/ServiceItem";
    export default {
        name: "Services",
        components: {ServiceItem}
    }
</script>

<style lang="scss" scoped>
    .service {
        background-image: url("../assets/img/service-bg.png");
        position: relative;
        padding-bottom: 98px;

        .container {
            display: flex;
            flex-direction: column;
            align-items: center;

            img {
                position: absolute;
                top: 122px;
            }
            h4 {
                margin: 262px 0 12px;
            }

            h3 {
                color: var(--service-color);
            }

            p {
                font-weight: 800;
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
            }
        }
    }
</style>
