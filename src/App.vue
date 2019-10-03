<template>
  <div id="app">
    <Nav></Nav>
    <Header></Header>
    <intro></intro>
    <Services></Services>
    <Work></Work>
    <Testimonials></Testimonials>
    <Newsletter></Newsletter>
    <Footer></Footer>
    <Copyright></Copyright>
  </div>
</template>

<script>
import Header from "@/components/Header";
import Nav from "@/components/Nav";
import Intro from "@/components/Intro";
import Services from "@/components/Services";
import Work from "@/components/Work";
import ServiceItem from "@/components/ServiceItem";
import Testimonials from "@/components/Testimonials";
import Newsletter from "@/components/Newsletter";
import Footer from "@/components/Footer";
import Copyright from "@/components/Copyright";
export default {
  name: 'app',
  components: {
    Copyright,
    Footer,
    Newsletter,
    Testimonials,
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
