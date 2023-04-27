<script>
import HeaderNavItem from './HeaderNavItem.vue';

export default {
    name: "Nav",
    components: {
        HeaderNavItem
    },
    props: {
        menu: Array
    }
}
</script>

<template>
    <ul>
        <li v-for="(elem, index) in menu" :key="index" :class="elem.current ? 'active' : ''">
            <HeaderNavItem :title="elem.title" />
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