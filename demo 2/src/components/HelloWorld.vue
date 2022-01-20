<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <h2>热门功能</h2>
    <ul>
      <li @click="testone">
        <router-link to="/home/1">客户画像</router-link>
      </li>
      <li @click="testone">
        <router-link to="/home/2">页面埋点</router-link>
      </li>
      <li @click="testone">
        <router-link to="/home/3">数据分析</router-link>
      </li>
      <li @click="testone">
        <router-link to="/home/4">定点营销</router-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data () {
    return {
      msg: '欢迎访问'
    }
  },
  methods: {
    testone () {
      // 在事件需要触发的地方进行 track
      console.log('触发埋点事件')
      clab_tracker.track('c_smart_custom_event')
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h1, h2 {
  font-weight: normal;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
