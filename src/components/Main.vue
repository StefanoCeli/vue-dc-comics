<template>
  <main>
      <div class="wrap">
          <Card
          v-for="( comic, index ) in comics" :key="index"
          :card="comic"
           />
      </div>
      <LoadBtn />
  </main>
</template>

<script>
import Card from './Card.vue'
import comics from '../assets/data/dc-comics'
import LoadBtn from './LoadBtn.vue'

export default {
    name:'Main',
    components:{
        Card,
        LoadBtn
    },
    data(){
        return {
            comics
            }
    }
}
</script>

<style lang="scss" scoped>

main{
    padding: 50px 0;
    background-color: #1c1c1c;
    .wrap{
        flex-wrap: wrap;
    }   
}


</style>