<template>
  <div id="app">
    <div id="nav">
      <router-link to="/todo">Todo</router-link>

    </div>

    <!-- 路由插座 展示路由渲染的组件内容 -->
    <div class="router-view">
      <!-- router-view一般是用来当跳转到另一个页面时，显示该页面的组件的 -->
      <router-view/>
    </div>

  </div>
</template>

<script>
  export default {
    name: "App",

  
  }
</script>

<style lang="less">
  // 全局的样式要在APP.vue里面写，因为这里没有scoped
  *{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
  li{
    list-style: none;
  }

  #app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    // text-align: center;
    // color: #2c3e50;
  }

  #nav {
    padding: 30px;

    a {
      font-weight: bold;
      color: #2c3e50;

      &.router-link-exact-active {
        color: #42b983;
      }
    }
  }
</style>
