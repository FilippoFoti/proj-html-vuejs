<script>
export default {
    name: "ItemNav",
    props: {
        title: "",
        // path: "",
    },
}
</script>

<template>
    <a href=""> {{ title }}</a>
</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;
@use "../style/partials/variables" as *;

a {
    text-decoration: none;
    color: inherit;
}
</style>