<script>
import SingleSocial from '../mini-components/singleSocial.vue';
import singleSocial from '../mini-components/singleSocial.vue';

export default {
    name: "socialSection",
    components: { SingleSocial }
}
</script>

<template>
    <section class="container my-5 py-5">
        <SingleSocial v-for="n in 3"></SingleSocial>
    </section>
</template>

<style lang="scss" scoped></style>