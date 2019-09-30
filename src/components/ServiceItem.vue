<template>
<div class="chopping">
    <img src="../assets/img/chopping-icon.svg" alt="">
    <h5>Chopping heads</h5>
    <p>Tincidunt lobortis feugiat vivamus at
        <br>augue eget. Risus feugiat in ante metus
        <br>dictum. Amet aliquam id diam maecenas.</p>
</div>
</template>

<script>
    export default {
        name: "ServiceItem"
    }
</script>

<style lang="scss" scoped>
    .chopping {

        img {
            border-radius: 50%;
            background-color: var(--chopping-bg-color);
            border: 1px solid var(--chopping-border-color);
            padding: 25px 22px 26px 24px;
        }

        h5 {
            font-weight: 500;
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
    }
</style>
