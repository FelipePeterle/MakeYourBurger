<template>
<div class="message-container">
    <p>{{ msg }}</p>
</div>

</template>

<script>
export default{
    name:"Message",
    props:{
        msg: String
    }
}

</script>

<style lang="scss" scoped>
$color-info: #004085;
$background-info: #CCE5FF;
$border-color-info: #B8DAFF;
$container-radius: 5px;
$container-spacing: 10px;
$container-max-width: 400px;
$container-margin: 30px auto;

.message-container {
  color: $color-info;
  background-color: $background-info;
  border: 2px solid $border-color-info;
  border-radius: $container-radius;
  padding: $container-spacing;
  max-width: $container-max-width;
  margin: $container-margin;
}
</style>
