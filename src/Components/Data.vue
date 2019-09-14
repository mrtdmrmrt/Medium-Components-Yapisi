<template>
  <div class="container">
  	<div class="row">
  		<DataSource @dataSource="dataTarget"/>
  	</div>
  	<hr>
  	<div class="row">
  		<DataTarget :dataList = "data"/>
  	</div>
  </div>
</template>

<script>
import DataSource from "./DataSource"
import DataTarget from "./DataTarget"
  export default {
   components : {
   	DataSource,
   	DataTarget
   },
   data(){
    return {
      data : {}
    }
   },
   methods : {
      dataTarget($event){
        this.data = $event
      }
   }
  }
</script>
