<script>
import singleSocial from '../mini-components/singleSocial.vue';
import { store } from '../store';
// AOS-------------
import AOS from 'aos';
import 'aos/dist/aos.css';
// ----------------

export default {
    name: "socialSection",
    components: { singleSocial, AOS },

    // AOS --------------------
    created() {
        AOS.init();
    },
    // AOS --------------------

    data() {
        return {
            store,
        }
    },
}
</script>

<template>
    <section class="container my-5 py-5">
        <h3 class="text-center">Follow me:</h3>
        <singleSocial data-aos="fade-up" data-aos-duration="1500" data-aos-delay="50" data-aos-once="true"
            v-for="(social, index) in store.social" :key="index" :social="social"></singleSocial>
    </section>
</template>

<style lang="scss" scoped></style>