<script>
import AppHeader from "./components/AppHeader.vue";
// import AppMain from "./components/AppMain.vue";

export default {
  components: {
    AppHeader,
    // AppMain
  },
  data() {
    return {
      menu: [
        {
          title: "HOME",
          url: "#",
          current: false,
        },
        {
          title: "ABOUT",
          url: "#",
          current: false,
        },
        {
          title: "PROJECTS",
          url: "#",
          current: false,
        },
        {
          title: "PROCESS",
          url: "#",
          current: true,
        },
        {
          title: "TESTIMONIALS",
          url: "#",
          current: false,
        },
      ]
    }
  }
}
</script>

<template>
  <AppHeader :menu="menu" />
  <!-- <AppMain /> -->
</template>

<style lang="scss">
@use "./style/general.scss"
</style>