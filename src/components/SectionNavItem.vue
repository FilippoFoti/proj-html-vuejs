<script>

export default {
    name: "SectionNavItem",
    props: {
        title: ""
    }
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