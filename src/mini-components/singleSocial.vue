<script>
export default {
    name: "singleSocial",

    props: {
        social: Object,
    },
}
</script>

<template>
    <section class="row my-5">

        <a :href="social.link" class="btn btn-custom col-10 col-md-8 offset-1 offset-md-2 py-3 rounded-4 fs-4">
            {{ social.name }}
        </a>

    </section>
</template>

<style lang="scss" scoped>
.btn-custom {
    color: white;
    background-color: aqua;

    &:hover {
        animation-name: scaleUp;
        animation-duration: .25s;
        animation-fill-mode: forwards;
    }
}

@keyframes scaleUp {
    0% {
        transform: scale(1);
    }

    100% {
        transform: scale(1.2);
        font-weight: 700;
    }
}
</style>