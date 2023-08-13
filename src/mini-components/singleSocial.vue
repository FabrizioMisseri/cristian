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

        <a :href="social.link" class="btn btn-custom col-6 offset-3 py-3">
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
        animation-duration: .4s;
        animation-fill-mode: forwards;
    }
}

@keyframes scaleUp {
    0% {
        transform: scale(1);
    }

    100% {
        transform: scale(1.2);
        font-weight: 800;
    }
}
</style>