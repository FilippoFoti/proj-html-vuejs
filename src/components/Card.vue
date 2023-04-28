<script>
import ContentCardOne from './ContentCardOne.vue';
import ContentCardTwo from './ContentCardTwo.vue';

export default {
    name: "Card",
    components: {
    ContentCardOne,
    ContentCardTwo
},
    props: {
        arrayOne: Array,
        arrayThree: Array
    }
}
</script>

<template>
    <div class="row">
        <div class="col" v-for="(elem, index) in arrayOne" :key="index">
            <ContentCardOne :elem="elem"/>
        </div>
        <div class="col" v-for="(elem, index) in arrayThree" :key="index">
            <ContentCardTwo :elem="elem"/>
        </div>
    </div>
</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;
@use "../style/partials/variables" as *;

.row {
    display: flex;
    flex-wrap: wrap;
    gap: 20px;

    .col {
        width: calc(100% / 3 - 13.4px);
        border: 1px solid white;
        border-radius: 5px;
        background-color: white;
        padding: 30px;
    }
}

</style>