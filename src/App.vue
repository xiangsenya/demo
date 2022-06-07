<template>
  <div id="app">
    <Head/>
    <Banner/>
    <Icon/>
    <Active/>
    <Shop/>
    <Area/>
  </div>
</template>

<script>
import Head from "@/components/Head";
import Banner from "@/components/Banner";
import Icon from "@/components/Icon";
import Active from "@/components/Active";
import Shop from "@/components/Shop";
import Area from "@/components/Area";

export default {
  name: 'App',
  components: {
    Head,
    Banner,
    Icon,
    Active,
    Shop,
    Area
  }
}
</script>

<style>
#app {
  width: 400px;
  margin: 0 auto;
}
</style>
