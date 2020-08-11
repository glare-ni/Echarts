<template>
  <div class="Echarts">
    <div id="main" style="width: 1200px;height:800px;"></div>
  </div>
</template>

<script>
export default {
  name: 'Echarts',
  methods: {
    myEcharts() {
      // 基于准备好的dom，初始化echarts实例
      var myChart = this.$echarts.init(document.getElementById('main'))

      var option = null
      myChart.showLoading()
      myChart.hideLoading()

      var data = []

      var graph = {
        links: [
          {
            id: '0',
            name: null,
            source: '0',
            target: '3',
            lineStyle: { normal: {} }
          },
          {
            id: '1',
            name: null,
            source: '1',
            target: '3',
            lineStyle: { normal: {} }
          },
          {
            id: '2',
            name: null,
            source: '2',
            target: '3',
            lineStyle: { normal: {} }
          },
          {
            id: '3',
            name: null,
            source: '4',
            target: '7',
            lineStyle: { normal: {} }
          },
          {
            id: '4',
            name: null,
            source: '5',
            target: '7',
            lineStyle: { normal: {} }
          },
          {
            id: '5',
            name: null,
            source: '6',
            target: '7',
            lineStyle: { normal: {} }
          },
          {
            id: '6',
            name: null,
            source: '9',
            target: '11',
            lineStyle: { normal: {} }
          },
          {
            id: '7',
            name: null,
            source: '10',
            target: '11',
            lineStyle: { normal: {} }
          },
          {
            id: '8',
            name: null,
            source: '3',
            target: '14',
            lineStyle: { normal: {} }
          },
          {
            id: '9',
            name: null,
            source: '7',
            target: '14',
            lineStyle: { normal: {} }
          },
          {
            id: '10',
            name: null,
            source: '8',
            target: '14',
            lineStyle: { normal: {} }
          },
          {
            id: '11',
            name: null,
            source: '11',
            target: '14',
            lineStyle: { normal: {} }
          },
          {
            id: '12',
            name: null,
            source: '12',
            target: '14',
            lineStyle: { normal: {} }
          },
          {
            id: '13',
            name: null,
            source: '13',
            target: '14',
            lineStyle: { normal: {} }
          },
          {
            id: '14',
            name: null,
            source: '14',
            target: '18',
            lineStyle: { normal: {} }
          },
          {
            id: '15',
            name: null,
            source: '15',
            target: '18',
            lineStyle: { normal: {} }
          },
          {
            id: '16',
            name: null,
            source: '16',
            target: '18',
            lineStyle: { normal: {} }
          },
          {
            id: '17',
            name: null,
            source: '17',
            target: '18',
            lineStyle: { normal: {} }
          }
        ],
        nodes: [
          {
            id: '0',
            name: '化学工程',
            itemStyle: null,
            symbolSize: 10,
            x: null,
            y: null,
            value: 1957,
            category: 0,
            draggable: true,
            attributes: { modularity_class: 0 }
          },
          {
            id: '1',
            name: '石油加工',
            itemStyle: null,
            symbolSize: 10,
            x: null,
            y: null,
            value: 1958,
            category: 0,
            draggable: true,
            attributes: { modularity_class: 0 }
          },
          {
            id: '2',
            name: '工业化学',
            itemStyle: null,
            symbolSize: 10,
            x: null,
            y: null,
            value: 1986,
            category: 0,
            draggable: true,
            attributes: { modularity_class: 0 }
          },
          {
            id: '3',
            name: '化学工程',
            itemStyle: null,
            symbolSize: 20,
            x: null,
            y: null,
            value: 1957,
            category: 0,
            draggable: true,
            attributes: { modularity_class: 0 }
          },
          {
            id: '4',
            name: '无机化工',
            itemStyle: null,
            symbolSize: 10,
            x: null,
            y: null,
            value: 1952,
            category: 0,
            draggable: true,
            attributes: { modularity_class: 0 }
          },
          {
            id: '5',
            name: '煤化工',
            itemStyle: null,
            symbolSize: 10,
            x: null,
            y: null,
            value: 1952,
            category: 0,
            draggable: true,
            attributes: { modularity_class: 0 }
          },
          {
            id: '6',
            name: '有机化工',
            itemStyle: null,
            symbolSize: 10,
            x: null,
            y: null,
            value: 1955,
            category: 0,
            draggable: true,
            attributes: { modularity_class: 0 }
          },
          {
            id: '7',
            name: '化学工艺',
            itemStyle: null,
            symbolSize: 20,
            x: null,
            y: null,
            value: 1952,
            category: 0,
            draggable: true,
            attributes: { modularity_class: 0 }
          },
          {
            id: '8',
            name: '高分子化工',
            itemStyle: null,
            symbolSize: 20,
            x: null,
            y: null,
            value: 1958,
            category: 0,
            draggable: true,
            attributes: { modularity_class: 0 }
          },
          {
            id: '9',
            name: '精细化工',
            itemStyle: null,
            symbolSize: 10,
            x: null,
            y: null,
            value: 1952,
            category: 0,
            draggable: true,
            attributes: { modularity_class: 0 }
          },
          {
            id: '10',
            name: '感光材料',
            itemStyle: null,
            symbolSize: 10,
            x: null,
            y: null,
            value: 1972,
            category: 0,
            draggable: true,
            attributes: { modularity_class: 0 }
          },
          {
            id: '11',
            name: '精细化工',
            itemStyle: null,
            symbolSize: 20,
            x: null,
            y: null,
            value: 1952,
            category: 0,
            draggable: true,
            attributes: { modularity_class: 0 }
          },
          {
            id: '12',
            name: '工业分析',
            itemStyle: null,
            symbolSize: 20,
            x: null,
            y: null,
            value: 1987,
            category: 0,
            draggable: true,
            attributes: { modularity_class: 0 }
          },
          {
            id: '13',
            name: '工业催化',
            itemStyle: null,
            symbolSize: 20,
            x: null,
            y: null,
            value: 1981,
            category: 0,
            draggable: true,
            attributes: { modularity_class: 0 }
          },
          {
            id: '14',
            name: '化学工程与工艺',
            itemStyle: null,
            symbolSize: 30,
            x: null,
            y: null,
            value: 1952,
            category: 0,
            draggable: true,
            attributes: { modularity_class: 0 }
          },
          {
            id: '15',
            name: '轻化工程',
            itemStyle: null,
            symbolSize: 30,
            x: null,
            y: null,
            value: 1999,
            category: 0,
            draggable: true,
            attributes: { modularity_class: 1 }
          },
          {
            id: '16',
            name: '油气储运工程',
            itemStyle: null,
            symbolSize: 30,
            x: null,
            y: null,
            value: 2002,
            category: 0,
            draggable: true,
            attributes: { modularity_class: 2 }
          },
          {
            id: '17',
            name: '资源循环科学与工程',
            itemStyle: null,
            symbolSize: 30,
            x: null,
            y: null,
            value: 2010,
            category: 0,
            draggable: true,
            attributes: { modularity_class: 3 }
          },
          {
            id: '18',
            name: '化工学院',
            itemStyle: null,
            symbolSize: 40,
            x: null,
            y: null,
            value: 1952,
            category: 0,
            draggable: true,
            attributes: { modularity_class: 4 }
          }
        ]
      }

      var categories = []
      for (var i = 0; i < 10; i++) {
        categories[i] = {
          name: '类目' + i
        }
      }

      graph.nodes.forEach(function (node) {
        node.itemStyle = null
        node.category = node.attributes.modularity_class
        node.x = node.y = null
        node.draggable = true
        node.label = {
          normal: {
            show: node.symbolSize > 10
          }
        }
      })

      var edges = []

      option = {
        title: {
          top: 'bottom',
          left: 'right'
        },
        tooltip: {},
        // legend: [{
        //   data: categories.map(function (a) {
        //     return a.name;
        //   })
        // }],
        animation: false,
        series: [
          {
            type: 'graph',
            layout: 'force',
            data: data,
            categories: categories,
            roam: true,
            label: {
              position: 'right'
            },
            force: {
              repulsion: 500,
              edgeLength: 1
            },
            edges: edges
          }
        ]
      }
      var j = 0
      var interval = setInterval(function () {
        if (data.length < graph.nodes.length) {
          // 这里是限制循环，否则会无穷循环下去
          data.push(graph.nodes[data.length])
          myChart.setOption({
            series: [
              {
                roam: true,
                data: data,
                edges: edges
              }
            ]
          })
        }
        while (
          j < graph.links.length &&
          graph.links[j].target === data.length - 1
        ) {
          edges.push({
            source: graph.links[j].source,
            target: graph.links[j].target
          })
          j++
        }
        myChart.setOption({
          series: [
            {
              roam: true,
              data: data,
              edges: edges
            }
          ]
        })
        if (data.length === graph.nodes.length) {
          clearInterval(interval)
        }
      }, 500)
      if (option && typeof option === 'object') {
        myChart.setOption(option, true)
      }
    }
  },
  mounted() {
    this.myEcharts()
  }
}
</script>

<style>
</style>
