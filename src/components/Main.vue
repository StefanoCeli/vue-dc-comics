<template>
  <main>
      <div class="wrap">
          <h1>CURRENT SERIES</h1>
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
@import '../assets/style/variables.scss';

main{
    padding: 50px 0;
    background-color: #1c1c1c;
    .wrap{
        flex-wrap: wrap;
        position: relative;
        h1{
            color: #fff;
            position: absolute;
            top: -9%;
            left: -1%;
            transform: translateY(-50%);
            font-size: 23px;
            padding: 0.5rem 1.25rem;
            background-color: $brand-blue;
        }
    }   
}


</style>