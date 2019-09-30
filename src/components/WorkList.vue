<template>
    <div class="section">
        <div class="content">
            <h5>01</h5>
            <h6>Upper prior hundred links approach reedy</h6>
            <p>Upper prior hundred links approach reedy, was to the
                <br>than and the ever somehow surprised known for
                <br>every by of there until road, </p>
        </div>
        <img src="../assets/img/work-photo.png" alt="">
        <img class="colored-shape" src="../assets/img/work-bg.png" alt="">
    </div>
</template>

<script>
    export default {
        name: "WorkList"
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

        .content {

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
        }
    }

</style>
