<template>
  <div id="app">
    <MenuBar />
    <Billboard />
    <NewArrivals />
    <Item />
    <Footer />
  </div>
</template>

<script>
import MenuBar from "~/components/MenuBar";
import Carousel from "~/components/Billboard";
import Item from "~/components/Item";
import Billboard from "~/components/Billboard";
import Footer from "~/components/Footer";
import NewArrivals from "~/components/NewArrivals";
export default {
  components: {Billboard, MenuBar, Carousel, Item, Footer, NewArrivals},
  methods: {
  }
}

</script>

<style>
#app {
  font-family: Helvetica, sans-serif;
  text-align: center;
}
</style>
