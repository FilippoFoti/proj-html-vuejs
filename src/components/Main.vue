<script>
import SectionOne from './SectionOne.vue';
import SectionThree from './SectionThree.vue';
import SectionTwo from './SectionTwo.vue';

export default {
    name: "Main",
    components: {
    SectionOne,
    SectionTwo,
    SectionThree
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
</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;
@use "../style/partials/variables" as *;
</style>