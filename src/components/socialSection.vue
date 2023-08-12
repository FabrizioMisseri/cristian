<script>
import singleSocial from '../mini-components/singleSocial.vue';
import { store } from '../store';

export default {
    name: "socialSection",
    components: { singleSocial },

    data() {
        return {
            store,
        }
    },
}
</script>

<template>
    <section class="container my-4 py-4">
        <singleSocial v-for="(social, index) in store.social" :key="index" :social="social"></singleSocial>
    </section>
</template>

<style lang="scss" scoped></style>