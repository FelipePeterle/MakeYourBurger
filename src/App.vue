<template>
  <div>
    <Navbar :logo="logo_src" :alt="app_name" />
    <div>
      <router-view></router-view>
    </div>
    <Footer />
  </div>
</template>
<script>
import Navbar from './components/Navbar'
import Footer from './components/Footer'

export default {
  data: function() {
    return {
      logo_src: "/img/logo.png",
      app_name: "Make Your Burger"
    }
  },
  components: {
    Navbar,
    Footer
  }
}
</script>

<style lang="scss">
$font-family-default: Helvetica;
$main-text-color: #222;
$h1-font-size: 42px;
$container-margin: 50px;
$container-min-height: 250px;
$h1-margin-bottom: 30px;

* {
  font-family: $font-family-default;
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

.main-container {
  margin: $container-margin;
  min-height: $container-min-height;
}

h1 {
  text-align: center;
  font-size: $h1-font-size;
  margin-bottom: $h1-margin-bottom;
  color: $main-text-color;
}
</style>
