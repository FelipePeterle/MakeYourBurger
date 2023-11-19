<template>
    <div id="nav">
        <router-link to="/" id="logo-url">
            <img :src="logo" :alt="alt" id="logo">
        </router-link>
        <router-link to="/">Home</router-link>
        <router-link to="/pedidos">Pedidos</router-link>
    </div>
</template>
<script>
export default{
    name:"Navbar",
    props:["logo", "alt"]
}
</script>

<style lang="scss" scoped>
$nav-background-color: #222;
$nav-border-color: #111;
$nav-padding: 15px 50px;
$link-color: #FCBA03;
$link-hover-color: #FFF;
$logo-margin: auto;
$logo-margin-left: 0;
$logo-size: 40px;
$link-margin: 12px;
$transition-time: 0.5s;

#nav {
  background-color: $nav-background-color;
  border-bottom: 4px solid $nav-border-color;
  padding: $nav-padding;
  display: flex;
  justify-content: flex-end;
  align-items: center;

  #logo-url {
    margin: $logo-margin;
    margin-left: $logo-margin-left;
  }

  #logo {
    width: $logo-size;
    height: $logo-size;
  }

  a {
    color: $link-color;
    text-decoration: none;
    margin: $link-margin;
    transition: $transition-time;
    
    &:hover {
      color: $link-hover-color;
    }
  }
}
</style>
