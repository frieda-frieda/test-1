<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <ul>
      <li>
        <router-link to="/home"> 返回主页</router-link>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'UserDesign',
  data () {
    return {
      msg: '欢迎访问'
    }
  },
  mounted () {
    const pageId = this.$route.params.id
    if (pageId === '1') {
      this.msg = '用户画像'
    } else if (pageId === '2') {
      this.msg = '页面埋点'
    } else if (pageId === '3') {
      this.msg = '数据分析'
    } else if (pageId === '4') {
      this.msg = '自动化营销'
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
