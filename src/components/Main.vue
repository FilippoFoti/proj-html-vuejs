<script>
import SectionOne from './SectionOne.vue';
import SectionTwo from './SectionTwo.vue';

export default {
    name: "Main",
    components: {
    SectionOne,
    SectionTwo
},
    props: {
        arrayOne: Array
    }
}
</script>

<template>
    <SectionOne :arrayOne="arrayOne"/>
    <SectionTwo />
</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;
@use "../style/partials/variables" as *;
</style>