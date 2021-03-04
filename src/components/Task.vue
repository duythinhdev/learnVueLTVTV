<template>
  <div class="Task">
    <span >{{ taskData }}</span>
  </div>
</template>

<script>
export default {
  // props:[
  //   'taskData'
  // ],
  props:{
    // name:'taskData',
    // type: Object,
    // default: {}
    taskData: Object
  },
  data(){
    return{
        content:'ABC'
    }
  },
  methods:{
    deleteTask:function (){
      console.log(this.taskData)
    }
  }
}
</script>
<style >

</style>
