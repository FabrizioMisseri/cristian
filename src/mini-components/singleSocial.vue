<script>
export default {
    name: "singleSocial",

    props: {
        social: Object,
    },
}
</script>

<template>
    <section class="row my-4">

        <a :href="social.link" class="btn btn-primary col-8 offset-2">
            {{ social.name }}
        </a>

    </section>
</template>

<style lang="scss" scoped></style>