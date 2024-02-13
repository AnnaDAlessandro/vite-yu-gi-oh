<script >
import SingleCard from '../../components/cards/SingleCard.vue' 
import { store } from '../../store';
export default{
    name:"CardsList",
    components:{
        SingleCard
    },
    data (){
       return {
        store

       }
    }
}

</script>

<template>
<div class="row">
    <SingleCard
    v-for="(element,index) in store.arrayCards"
    :key="index"
    :propsElement ="element" ></SingleCard>
</div>
</template>

<style lang="scss" scoped>
</style>
