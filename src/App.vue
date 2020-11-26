<template>
  <div id="app">
    <router-view />
    <el-backtop :visibility-height="200" target="#app"></el-backtop>
  </div>
</template>

<style lang="scss">
html,
body {
  height: 100%;
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  height: 100%;
  overflow-y: hidden;
  overflow: scroll;
}
body {
  margin: 0;
  padding: 0;
  background: #001278 url(http://www.ctma.com.cn/ctma_news/2018nianhui/bg.gif)
    repeat;
  background-size: cover;
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
