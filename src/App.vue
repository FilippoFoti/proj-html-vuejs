<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";

export default {
  components: {
    Header,
    Main
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
      ],
      arrayOne: [
        {
          icon: "fa-solid fa-user-group",
          title: "Human Capital",
          text: "Humanizing business: Harness the power of technology to improve the way people work."
        },
        {
          icon: "fa-solid fa-chart-pie",
          title: "Core Business",
          text: "It takes innovative approaches to transform, modernize, and run existing platforms."
        },
        {
          icon: "fa-solid fa-coins",
          title: "Performance",
          text: "Archieving maximum impact and value from investments in finance and supply chain."
        }
      ]
    }
  }
}
</script>

<template>
  <Header :menu="menu" />
  <Main :arrayOne="arrayOne"/>
</template>

<style lang="scss">
@use "./style/general.scss"
</style>