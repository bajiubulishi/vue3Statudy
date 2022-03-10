<template>
  <div>222</div>
  <h1>name: {{obj.name}}</h1>
  <h1>name: {{obj.age}}</h1>
  <h1>name: {{obj.company}}</h1>
  <el-button type="primary" @click="btn">dianji</el-button>
  <h1></h1>
  <h1></h1>
</template>
<script>
  // import { defineComponent } from '@vue/composition-api';
  // export default defineComponent({

  // })
  import {toRef, reactive} from 'vue';
  export default({
    setup() {
      let obj1 = toRef ({name: 'liuyin', age: 18, company: '荆州'})
      let name = 'tianhui',age = 20,company = '白马湖',obj = reactive({name, age, company}),
      btn = () => {
        console.log(obj)
        obj = obj1
      }
      return {obj,btn}
    }
  })

</script>