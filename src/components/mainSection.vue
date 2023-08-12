<script>
export default {
    name: "mainSection",
}
</script>

<template>
    <section class="wrapper">

        <!-- lato SX -->
        <div class="side sx">
            img->photo{ debug }
        </div>
        <!-- / lato SX -->

        <!-- lato DX -->
        <div class="side dx px-5">
            <p>
                Lorem ipsum dolor, sit amet consectetur adipisicing elit. Voluptates sint dolorum voluptate similique ipsum
                quisquam quas corrupti voluptas animi unde eligendi rerum, illum et impedit aliquid quos autem itaque.
                Dicta.
                Excepturi praesentium placeat voluptate asperiores? Fugiat, minima architecto deserunt commodi dicta nobis
                doloribus rem mollitia facilis, nisi impedit quos animi earum laboriosam? Ex rerum laborum minima, sed quae
                quis dolore!
            </p>
        </div>
        <!-- / lato DX -->

    </section>
</template>

<style lang="scss" scoped>
.wrapper {
    display: flex;
    width: 100%;
    //debug
    min-height: 600px;

    .side {
        width: 50%;

        &.sx {
            //debug
            background-color: aqua;
            height: 600px;
        }
    }
}
</style>