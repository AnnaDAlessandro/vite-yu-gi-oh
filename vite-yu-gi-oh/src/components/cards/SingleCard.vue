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
<div class="col-3 mb-4">
    <div class="card" style="width: 18rem;">
  <img :src="propsElement.card_images[0].image_url" class="card-img-top" alt="...">
  <div class="card-body">
    <h4>{{ propsElement.name }}</h4>
    <p class="card-text">{{ propsElement.archetype }}</p>
  </div>
</div>
</div>
</template>

<style lang="scss" scoped>
</style>
