<template>
  <div id="app">
    {{ tongTien | dauchamphantach }}
    <button @click="tongTien +=20000">
    <Task  :task-data="tongTien" />
    </button>
  </div>
</template>

<script>
import Task from "@/components/Task";
export default {
  components: {Task},
  data(){
    return {
      tongTien: 1000000
    }
  },
  filters: {
    dauchamphantach: function(soTien){
      return soTien.toFixed(2).replace(/\d(?=(\d{3})+\.)/g, '$&,');
    }
  }
}
</script>
<style >
</style>
