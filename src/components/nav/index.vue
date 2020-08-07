<template>
  <div id="nav">
        <router-link to="/">常用网站</router-link> 
        <router-link to="/about">其他</router-link>
        <router-link to="/about">其他</router-link>
        <router-link to="/about">其他</router-link>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="less" scoped>
#nav {
  a {
    font-weight: bold;
    color: #2c3e50;
    text-decoration: none;

    &.router-link-exact-active {
      color: rgba(173, 236, 91, 0.7);
    }
  }
}
</style>