<template>
  <div>
    <app-header></app-header>
    <app-slider></app-slider>
    <app-stream></app-stream>
    <app-content></app-content>
    <app-subscribe></app-subscribe>
    <app-support></app-support>
    <app-footer></app-footer>
  </div>
</template>

<script>
import Header from "../components/Header";
import Slider from "../components/Slider";
import Stream from "../components/Stream";
import Content from "../components/Content";
import Support from "../components/Support";
import Subscribe from "../components/Newsletter";
import Footer from "../components/Footer";
export default {
  components: {
    "app-header": Header,
    "app-slider": Slider,
    "app-stream": Stream,
    "app-content": Content,
    "app-support": Support,
    "app-subscribe":Subscribe,
    "app-footer":Footer,
  },
};
</script>

<style>
</style>
