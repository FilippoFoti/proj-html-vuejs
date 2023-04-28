<script>
export default {
    name: "ContentCardTwo",
    props: {
        elem: Object
    },
    methods: {
        getImagePath(image) {
            return new URL(`../assets/img/${image.img}`, import.meta.url).href;
        },
    }
}
</script>

<template>
    <div class="card">
        <img :src="getImagePath(elem)" alt="">
        <p>{{ elem.text }}</p>
        <p>{{ elem.lorem }}</p>
        <i :class="elem.icon"></i>
    </div>
</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;
@use "../style/partials/variables" as *;

.card {
    color: black;
    text-align: left;
    position: relative;

    img {
        width: 110px;
    }
    p {
        font-size: 0.8rem;
        padding-top: 10px;
    }

    i {
        color: rgba(204, 204, 204, 1);
        font-size: 1.5rem;
        position: absolute;
        bottom: -10px;
        right: -10px;
    }
}
</style>