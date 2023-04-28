<script>
import HeaderNavItem from './HeaderNavItem.vue';
import SectionNavItem from './SectionNavItem.vue';


export default {
    name: "Nav",
    components: {
        HeaderNavItem,
        SectionNavItem,
    },
    props: {
        menu: Array,
        arrayTwo: Array
    }
}
</script>

<template>
    <ul>
        <li v-for="(elem, index) in menu" :key="index" :class="elem.current ? 'active' : ''">
            <HeaderNavItem :title="elem.title" />
        </li>
        <li class="black" v-for="(elem, index) in arrayTwo" :key="index" :class="elem.current ? 'active' : ''">
            <SectionNavItem :title="elem.title" />
        </li>
    </ul>
</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;
@use "../style/partials/variables" as *;

ul {
    display: flex;
    align-items: center;
    justify-content: center;
    list-style-type: none;
    gap: 20px;

    li {
        color: white;

        &.active {
            color: rgba(0, 165, 165, 1);
        }

        &:hover {
            color: rgba(0, 165, 165, 1);
        }
    }

    .black {
        color: #e4eae6;

        &.active {
            background-color: rgba(15, 33, 40, 1);
            padding: 5px 10px;
            border-radius: 3px;
            color: #e4eae6;
        }

        &:hover {
            color: rgba(0, 165, 165, 1);
        }
    }
}
</style>