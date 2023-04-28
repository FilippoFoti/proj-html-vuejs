<script>
import SectionOne from './SectionOne.vue';
import SectionTwo from './SectionTwo.vue';
import SectionThree from './SectionThree.vue';
import SectionFour from './SectionFour.vue';
import SectionFive from './SectionFive.vue';

export default {
    name: "Main",
    components: {
    SectionOne,
    SectionTwo,
    SectionThree,
    SectionFour,
    SectionFive
},
    props: {
        arrayOne: Array,
        arrayTwo: Array,
        arrayThree: Array
    }
}
</script>

<template>
    <SectionOne :arrayOne="arrayOne"/>
    <SectionTwo />
    <SectionThree :arrayTwo="arrayTwo"/>
    <SectionFour />
    <SectionFive :arrayThree="arrayThree"/>
</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;
@use "../style/partials/variables" as *;
</style>