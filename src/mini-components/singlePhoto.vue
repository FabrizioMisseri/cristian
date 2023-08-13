<script>
export default {
    name: "singlePhoto",

    props: {
        photo: Object,
    },
}
</script>

<template>
    <div class="col-12 col-md-6 col-lg-4 px-4 ">

        <figure class="rounded-4 debug">

        </figure>

    </div>
</template>

<style lang="scss" scoped>
.debug {
    background-color: aqua;
    height: 300px;
}
</style>