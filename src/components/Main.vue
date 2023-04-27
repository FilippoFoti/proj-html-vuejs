<script>
import SectionOne from './SectionOne.vue';
import SectionTwo from './SectionTwo.vue';
import SectionThree from './SectionThree.vue';
import SectionFour from './SectionFour.vue';

export default {
    name: "Main",
    components: {
    SectionOne,
    SectionTwo,
    SectionThree,
    SectionFour
},
    props: {
        arrayOne: Array,
        arrayTwo: Array
    }
}
</script>

<template>
    <SectionOne :arrayOne="arrayOne"/>
    <SectionTwo />
    <SectionThree :arrayTwo="arrayTwo"/>
    <SectionFour />
</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;
@use "../style/partials/variables" as *;
</style>