<script >
  import CardsList from './cards/CardsList.vue'
  import { store } from '../store';
export default{
  components:{
    CardsList
  },
  
  name:"AppMain",
    data (){
       return {
        store
       }
    }
}

</script>

<template>
    <main class="p-3">
        <div class="container">
          <div class="mb-3">
           <select class="form-select w-25"
            name=""
             id=""
             v-model="store.selectValue"
             @change="$emit('search')">
            <option :value="element.archetype_name" v-for="(element,index) in store.arrayArchetype"
            :key="index">{{element.archetype_name}}</option>
          </select>  
          </div>
          <div class="bg-light p-2">
            <CardsList></CardsList>
            
          </div>
        </div>
       
       

    </main>
 
</template>

<style lang="scss" scoped>
    main{
        background-color: #d48f38;
    }

</style>
