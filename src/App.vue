<template>
  <Header />
  <Section />
  <SectionTwo />
</template>

<script>
import Header from "./components/Header.vue";
import Section from "./components/Section.vue";

export default {
  name: "App",
  components: {
    Header,
    Section,
    SectionTwo,
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
