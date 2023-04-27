<script>
import Card from "./Card.vue";

export default {
    name: "SectionOne",
    components: {
        Card
    },
    props: {
        arrayOne: Array
    }
}
</script>

<template>
    <main>
        <div class="container">
            <Card :arrayOne="arrayOne"/>
        </div>
        <div class="pattern"></div>
    </main>
</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;
@use "../style/partials/variables" as *;

main {
    background-color: rgba(238, 244, 237, 1);
    position: relative;
    z-index: 1;

    .container {
        width: 60%;
        margin: 0 auto;
    }
    
    .pattern {
        width: 170px;
        height: 75px;
        background: radial-gradient(circle, #7ED5D5 25%, transparent 26%);
        background-size: 1.2em 1.2em;
        background-color: transparent;
        opacity: 0.6;
        position: absolute;
        left: 50%;
        bottom: -36px;
        transform: translate(-50%)
    }
}
</style>