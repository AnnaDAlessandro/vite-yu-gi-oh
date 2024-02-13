<script >
import { store } from '../../store';
export default{
    name:"SingleCard",
    props:[ 
        'propsElement'
],
    data (){
       return {
         store
       }
    }
}

</script>

<template>
<div class="col-3">
    <div class="card" style="width: 18rem;">
  <img src="..." class="card-img-top" alt="...">
  <div class="card-body">
    <h4></h4>
    <p class="card-text"></p>
  </div>
</div>
</div>
</template>

<style lang="scss" scoped>
</style>
