<template>
  <div>
    <div id="app">
      <side-bar></side-bar>
      <img src="./assets/logo.png">
      <router-view />
    </div>
  </div>
</template>

<script>
import SideBar from '@/components/parts/SideBar';

export default {
  name: 'App',
  components: {
    SideBar,
  },
};
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
