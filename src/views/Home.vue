<template>
  <div class="home">
    <div>{{msg}}</div>
    <!-- <HelloWorld msg="Welcome to Your Vue.js App"/> -->
    <!-- <el-table :data="dataList" border>
      <el-table-column label="111"></el-table-column>
      <el-table-column label="111"></el-table-column>
      <el-table-column label="111"></el-table-column>
      <el-table-column label="111"></el-table-column>
    </el-table> -->
    <el-button @click="btn(1)">22</el-button>
    <Day02 />
  </div>
</template>

<script>
// @ is an alias to /src
// import HelloWorld from '@/components/HelloWorld.vue'
import Day02 from './002.vue';

export default {
  // name: 'Home',
  components: {
    // HelloWorld,
    Day02
  },
  setup() {
    const dataList = [];
    const msg = 'ererer'
    const btn = (val) => {
      console.log(val)
    }
    return {msg, dataList, btn}
  }
}
</script>
