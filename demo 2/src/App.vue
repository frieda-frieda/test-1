<template>
  <div id="app">
    <img src="./assets/logo.png">
    <router-view/>
  </div>
</template>

<script src="//a.dmhub.cn/cbe/collect?tid=1734229266&at=0&h=web"></script>
<script>
  clab_tracker.ready(function(){
    this.push({"pageType":"web"});
    this.track("open_page", {});
  });
</script>
<script>
export default {
  name: 'App'
}
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
