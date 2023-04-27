<script>
import AppHeaderTop from './AppHeaderTop.vue';
import AppHeaderBottom from './AppHeaderBottom.vue';

export default {
    name: "AppHeader",
    components: {
        AppHeaderTop,
        AppHeaderBottom,
    },
    props: {
        menu: Array
    }
}
</script>

<template>
    <AppHeaderTop />
    <AppHeaderBottom :menu="menu" />
</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;
@use "../style/partials/variables" as *;
</style>