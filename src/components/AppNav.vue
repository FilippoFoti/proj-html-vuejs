<script>
import AppItemNav from './AppItemNav.vue';

export default {
    name: "AppNav",
    components: {
        AppItemNav
    },
    props: {
        menu: Array
    }
}
</script>

<template>
    <ul>
        <li v-for="(elem, index) in menu" :key="index" :class="elem.current ? 'active' : ''">
            <AppItemNav :title="elem.title" />
        </li>
    </ul>
</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;
@use "../style/partials/variables" as *;

ul {
    list-style-type: none;

    li {
        color: white;

        &.active {
            color: rgba(0, 165, 165, 1);
        }
    }
}
</style>