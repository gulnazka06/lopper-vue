<template>
<div class="work">
    <div class="container">
        <h4>WHAT WE DO</h4>
        <h3>What we do</h3>
        <p>Upper prior hundred links approach reedy, was to the than
            <br>and the ever somehow surprised known for every by of there
            <br>until road, </p>
    </div>
    <WorkList
            order="01"
            title="Upper prior hundred links approach reedy"
            description="Upper prior hundred links approach reedy, was to the than and the ever somehow surprised known for every by of there until road, "
            imgURL="/assets/img/work-photo.png"
    ></WorkList>
    <WorkList
            order="02"
            title="Upper prior hundred links approach reedy"
            description="Upper prior hundred links approach reedy, was to the than and the ever somehow surprised known for every by of there until road, "
            type="green"
            imgURL="/assets/img/macbookpro.png"
    ></WorkList>
    <WorkList
            order="03"
            title="Upper prior hundred links approach reedy"
            description="Upper prior hundred links approach reedy, was to the than and the ever somehow surprised known for every by of there until road, "
            type="purple"
            imgURL="/assets/img/mac.png"
    ></WorkList>
</div>
</template>

<script>
    import WorkList from "@/components/WorkList";
    export default {
        name: "Work",
        components: {WorkList}
    }
</script>

<style lang="scss" scoped>
    @import "../assets/scss/mixin";

    .work {

        .container{
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 108px 0;

            @include mobile {
                padding: 100px 0;
            }


            h3 {
                color: var(--black);
            }

            p {
                font-weight: 700;
                font-size: 18px;
                line-height: 29px;
                text-align: center;
                color: var(--black);
            }
        }
    }
</style>
