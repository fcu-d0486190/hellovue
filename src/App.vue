<template>
  <div id="app">
   <img src="./assets/logo.png" alt="">
   <h1>{{title}}</h1>
   <test></test>
   <ve-line :data="chartData"></ve-line>
   <ve-bar :data="chartData"></ve-bar>
  </div>
</template>

<style lang="scss">
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>

<script>
import test from './components/test'
import VeLine from 'v-charts/lib/line'
import VeBar from 'v-charts/lib/bar'

export default {
  name: 'app',
  data () {
    return {
      title: 'h1heiei',
      chartData: { columns: ['日期', '销售额'],
        rows: [
          { '日期': '1月1日', '销售额': 123 },
          { '日期': '1月2日', '销售额': 1223 },
          { '日期': '1月3日', '销售额': 2123 },
          { '日期': '1月4日', '销售额': 4123 },
          { '日期': '1月5日', '销售额': 3123 },
          { '日期': '1月6日', '销售额': 7123 }
        ]
      }
    }
  },
  components: {
    test,
    VeLine,
    VeBar
  }
}
</script>
