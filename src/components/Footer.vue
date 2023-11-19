<template>
    <div id="footer">
      <p>Make Your Burger &copy; 2021</p>
    </div>
  </template>
  
  <script>
  export default {
    name: "Footer"
  }
  </script>
  
<style lang="scss" scoped>
$background-color: #222;
$border-top-color: #111;
$font-color: #fcba03;

#footer {
  height: 200px;
  background-color: $background-color;
  border-top: 4px solid $border-top-color;
  color: $font-color;
  display: flex;
  align-items: center;
  justify-content: center;
  bottom: 0;
  width: 100%;
}
</style>
