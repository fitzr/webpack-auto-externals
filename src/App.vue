<template>
  <div class='container'>
    <p>{{ greeting }} World!</p>
    <el-button type="primary" icon="el-icon-search">Search</el-button>
    <bar></bar>
  </div>
</template>

<script>
import { head } from 'lodash'
import $ from 'jquery'
import moment from 'moment'
import Bar from './Bar.vue'

export default {
  data: () => ({
    greeting: 'Hello'
  }),
  components: {
    Bar
  },
  created () {
    // use vendor libs

    const v = head([1, 2, 3])
    console.log(v)

    const id = $('#app').attr('id')
    console.log(id)

    console.log(moment().format('YYYY-MM-DD'))
  }
}
</script>

<style scoped>
.container {
  font-size: 2em;
  text-align: center;
}

</style>
