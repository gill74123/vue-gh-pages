<!-- 有點像 layout 的元件都放在這邊 -->
<template>
  <div id="nav">
    <router-link to="/">Home</router-link> |
    <router-link to="/about">About</router-link> |
    <a href="#" to="/123">123</a>
  </div>
  <router-view/> <!-- 路由顯示的區塊 -->
  {{ name }}
  <button type="button" class="btn btn-primary">Primary</button>
</template>

<style lang="scss">
@import "bootstrap";
</style>

<script>
export default {
  data () {
    return {
      name: process.env.VUE_APP_NAME
    }
  }
}
</script>
