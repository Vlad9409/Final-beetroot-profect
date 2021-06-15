<template>
  <Header />
  <Section />
  <SectionTwo />
  <Lock />
  <Statistic />
  <Cinema />
  <Shatter />
  <Whoweare />
  <Mapsect />
  <Oneclick />
  <Deliver />
  <Question />
  <Footer />
</template>

<script>
import Header from "./components/Header.vue";
import Section from "./components/Section.vue";
import SectionTwo from "./components/SectionTwo.vue";
import Lock from "./components/Lock.vue";
import Statistic from "./components/Statistic.vue";
import Cinema from "./components/Cinema.vue";
import Shatter from "./components/Shatter.vue";
import Whoweare from "./components/Whoweare.vue";
import Mapsect from "./components/Mapsect.vue";
import Oneclick from "./components/Oneclick.vue";
import Deliver from "./components/Deliver.vue";
import Question from "./components/Question.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    Section,
    SectionTwo,
    Lock,
    Statistic,
    Cinema,
    Shatter,
    Whoweare,
    Mapsect,
    Oneclick,
    Deliver,
    Question,
    Footer,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
