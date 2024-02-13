<script >
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import axios from 'axios'


export default{
  components:{
          AppHeader,
          AppMain
  },
          data (){
       return{
        ApiUrl:'https://db.ygoprodeck.com/api/v7/cardinfo.php'

       }
}
}

</script>

<template>
 <AppHeader></AppHeader>
 <AppMain></AppMain>
 
</template>

<style lang="scss" scoped>
</style>
