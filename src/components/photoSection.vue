<script>
import { store } from '../store';
import singlePhoto from '../mini-components/singlePhoto.vue';

export default {
    name: "photoSection",
    components: { singlePhoto },

    data() {
        return {
            store,
        }
    },
}
</script>

<template>
    <section class="container my-4 py-4">
        <div class="row g-4">

            <singlePhoto v-for="(photo, index) in store.photos" :key="index" :social="photo"></singlePhoto>

        </div>
    </section>
</template>

<style lang="scss" scoped></style>