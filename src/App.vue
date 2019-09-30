<template>
  <div id="app">
    <Nav></Nav>
    <Header></Header>
    <intro></intro>
    <Services></Services>
  </div>
</template>

<script>
import Header from "@/components/Header";
import Nav from "@/components/Nav";
import Intro from "@/components/Intro";
import Services from "@/components/Services";
export default {
  name: 'app',
  components: {
    Services,
    Intro,
    Nav,
    Header
  }
}
</script>

<style lang="scss">
  @import "./assets/scss/main";
</style>
