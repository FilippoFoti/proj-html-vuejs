<script>
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";

export default {
  components: {
    Header,
    Main,
    Footer
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
      ],
      arrayTwo: [
        {
          title: "ALL",
          current: true,
        },
        {
          title: "INSTITUTIONAL",
          current: false,
        },
        {
          title: "SOCIAL",
          current: false,
        },
        {
          title: "EVENTS",
          current: false,
        },
        {
          title: "INNOVATION",
          current: false,
        },
        {
          title: "ENVIRONMENT",
          current: false,
        },
        {
          title: "TECHNOLOGY",
          current: false,
        }
      ],
      arrayThree: [
        {
          img: "logo-1.png",
          text: "Praesent volutpat justo sit amet elementum malesuada. Praesent sagittis augue justo, in accumsan orci phoncus at pellentsque.",
          lorem: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
          icon: "fa-solid fa-quote-right"
        },
        {
          img: "logo-2.png",
          text: "Praesent volutpat justo sit amet elementum malesuada. Praesent sagittis augue justo, in accumsan orci phoncus at pellentsque.",
          lorem: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
          icon: "fa-solid fa-quote-right"
        },
        {
          img: "logo-3.png",
          text: "Praesent volutpat justo sit amet elementum malesuada. Praesent sagittis augue justo, in accumsan orci phoncus at pellentsque.",
          lorem: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
          icon: "fa-solid fa-quote-right"
        }
      ]
    }
  }
}
</script>

<template>
  <Header :menu="menu" />
  <Main :arrayOne="arrayOne" :arrayTwo="arrayTwo" :arrayThree="arrayThree" />
  <Footer />
</template>

<style lang="scss">
@use "./style/general.scss"
</style>