<script>
import HeaderTop from './HeaderTop.vue';
import HeaderBottom from './HeaderBottom.vue';

export default {
    name: "AppHeader",
    components: {
        HeaderTop,
        HeaderBottom,
    },
    props: {
        menu: Array
    }
}
</script>

<template>
    <HeaderTop />
    <HeaderBottom :menu="menu" />
</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;
@use "../style/partials/variables" as *;
</style>