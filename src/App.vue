<script>
import mainSection from './components/mainSection.vue';
import socialSection from './components/socialSection.vue';
import photoSection from './components/photoSection.vue';



export default {
    name: "App",

    components: {
        mainSection,
        socialSection,
        photoSection,
    },
}
</script>

<template>
    <mainSection></mainSection>
    <socialSection></socialSection>
    <photoSection></photoSection>
</template>

<style lang="scss"></style>
