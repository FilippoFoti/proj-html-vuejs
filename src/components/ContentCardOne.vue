<script>
export default {
    name: "ContentCardOne",
    props: {
        // icon: "",
        // title: "",
        // text: "",
        elem: Object
    },
}
</script>

<template>
    <div class="card">
        <i :class=" elem.icon "></i>
        <h2>{{ elem.title }}</h2>
        <p>{{ elem.text }}</p>
    </div>
</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;
@use "../style/partials/variables" as *;

.card {
    color: black;

    i {
        color: rgba(5, 130, 131, 1);
        background-color: rgba(218, 236, 237, 1);
        border-radius: 50%;
        padding: 10px;
    }

    h2 {
        margin: 20px 0;
        font-size: 1.3rem;
    }

    p {
        font-size: 0.85rem;
    }
}
</style>