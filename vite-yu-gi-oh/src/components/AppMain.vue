<script >
  import CardsList from './cards/CardsList.vue'
export default{
  components:{
    CardsList
  },
  
  name:"AppMain",
    data (){
       return {

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
             id="">
            <option value="1">Alen</option>
            <option value="2">Two</option>
            <option value="3">Three</option>
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
