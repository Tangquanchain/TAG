<template>
  <div>
    <Alert />
    <div class="wrap">
      <Aside />
      <Navbar />
      <router-view></router-view>
      <Footer/>
    </div>
  </div>
</template>



<script>
import Navbar from "./Navbar";
import Aside from "./Aside";
import Footer from "./Footer";
import Alert from "./AlertMessage";
import $ from "jquery";

export default {
  components: {
    Alert,
    Navbar,
    Aside,
    Footer
  },
};
</script>

<style lang="scss">
@import url("https://fonts.googleapis.com/css?family=Open+Sans&display=swap");
@import url("https://fonts.googleapis.com/css?family=Anton&display=swap");

.wrap {
  transition: transform 0.3s;
  position: relative;
}

.wrap.active {
  transform: translateX(450px) ;
}
</style>