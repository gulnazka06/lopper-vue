<template>
  <div id="app">
    <Nav></Nav>
    <Header></Header>
    <intro></intro>
    <Services></Services>
    <Work></Work>
  </div>
</template>

<script>
import Header from "@/components/Header";
import Nav from "@/components/Nav";
import Intro from "@/components/Intro";
import Services from "@/components/Services";
import Work from "@/components/Work";
import ServiceItem from "@/components/ServiceItem";
export default {
  name: 'app',
  components: {
    Work,
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
