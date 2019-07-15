<template>
  <div id="app">
    <div id="nav">
      <router-link to="/">todoList1</router-link> |
      <router-link to="/about">todoList2</router-link>
    </div>
    <router-view />
  </div>
</template>
<style lang="scss" scoped>
#nav {
  padding: 30px;
  position: fixed;
  top: 0%;
  left: 0;
  width: 100%;
  a {
    font-weight: bold;
    color: #2c3e50;
    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
