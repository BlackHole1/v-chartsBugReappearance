<template>
  <div id="app">
    <ve-line :data="chartData" :title="chartTitle"></ve-line>
  </div>
</template>

<script>
import 'echarts/lib/component/title'
export default {
  name: 'App',
  created () {
    this.chartData = {
      columns: ['日期', '余额', '比率'],
      rows: [
        { '日期': '1月1日', '余额': 123, '比率': 0.3 },
        { '日期': '1月2日', '余额': 1223, '比率': 0.6 },
        { '日期': '1月3日', '余额': 2123, '比率': 0.9 },
        { '日期': '1月4日', '余额': 4123, '比率': 0.12 },
        { '日期': '1月5日', '余额': 3123, '比率': 0.15 },
        { '日期': '1月6日', '余额': 7123, '比率': 0.20 }
      ]
    }
    this.chartTitle = {
      text: '标题'
    }
  }
}
</script>
