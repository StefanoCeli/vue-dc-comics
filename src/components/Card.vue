<template>
  <div>
      <a href="#" class="image"><img :src="card.thumb" :alt="card.type"></a>
      <h4>{{ card.series.toUpperCase() }}</h4>
  </div>
</template>

<script>
export default {
    name:'Card',
    props: {
        card:Object
    }
}
</script>

<style lang="scss" scoped>
    div{
        height: 250px;
        flex-basis: calc(100% / 6 - 19px);
        transition: transform .5s;
        &:hover{
            transform: scale(1.1);
        }
        .image{
            display: inline-block;
            height: 200px;
            overflow: hidden;  
        }
        h4{
            color: #fff;
            font-size: 14px;
            margin-top: 10px;
            cursor: pointer;
            
        }
    }
</style>