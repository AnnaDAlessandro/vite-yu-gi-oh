<script >
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import axios from 'axios';
import {store} from './store';


export default{
  components:{
          AppHeader,
          AppMain
  },
          data (){
       return{
       store

       }
},
mounted(){
        this.getData()
        this.getArchetype()

},
methods:{

   getData(){
        if(store.selectValue){
                store.ApiUrl += `&archetype=${store.selectValue}`
        }
        axios.get(store.ApiUrl).then((res)=> {
                store.arrayCards=res.data.data

        })
   },
   getArchetype(){
        axios.get(store.ApiUrlArchetype).then((res)=> {
                store.arrayArchetype=res.data

        })
   }         
}
}

</script>

<template>
 <AppHeader></AppHeader>
 <AppMain @search="getData()"></AppMain>
 
</template>

<style lang="scss" scoped>
</style>
