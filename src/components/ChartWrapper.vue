<template>
  <div class="hello">
    <BarChart :data = "barChartData" xKey="name" yKey="amount" />
  </div>
</template>

<script>
import BarChart from '@/components/BarChart.vue';
export default {
  name: 'ChartWrapper',
  components:{
    BarChart
  },
  props: {
    msg: String
  },
  data: () => ({
    barChartData: [
      {
        name: "Roses",
        amount: 25
      },
      {
        name: "Tulips",
        amount: 40
      },
      {
        name: "Daisies",
        amount: 15
      },
      {
        name: "Narcissuses",
        amount: 9
      }
    ]
  })
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
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
