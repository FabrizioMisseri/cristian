<script>
import { store } from '../store';
import singlePhoto from '../mini-components/singlePhoto.vue';
// AOS-------------
import AOS from 'aos';
import 'aos/dist/aos.css';
// ----------------


export default {
    name: "photoSection",
    components: { singlePhoto, AOS },

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
        <div class="row g-4">

            <singlePhoto data-aos="fade-up" data-aos-duration="1500" data-aos-delay="50" data-aos-once="true"
                v-for="(photo, index) in store.photos" :key="index" :social="photo">
            </singlePhoto>

        </div>
    </section>
</template>

<style lang="scss" scoped></style>