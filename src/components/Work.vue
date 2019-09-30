<template>
<div class="work">
    <div class="container">
        <h4>WHAT WE DO</h4>
        <h3>What we do</h3>
        <p>Upper prior hundred links approach reedy, was to the than
            <br>and the ever somehow surprised known for every by of there
            <br>until road, </p>
    </div>
    <WorkList></WorkList>
    <WorkList></WorkList>
    <WorkList></WorkList>
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
    .work {
        .container{
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 108px 0;

            h3 {
                color: var(--black);
            }

            p {
                font-weight: 800;
                font-size: 18px;
                line-height: 29px;
                text-align: center;
                color: var(--black);
            }
        }
    }
</style>
