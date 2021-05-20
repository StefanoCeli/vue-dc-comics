<template>
  <header>
      <nav class="wrap">  
        <img src="../assets/img/dc-logo.png" alt="">
        <ul>
            <li 
            v-for="(link,index) in links" :key="index"
            ><a :class="{active: link.current}" href="#">{{link.text}}</a></li>
        </ul>   
      </nav>
  </header>
</template>

<script>
export default {
name:'Header',
    data(){
      return{
        links:[
          {
            text:'CHARACTERS',
            current:false
          },
          {
            text:'COMICS',
            current:true
          },
          {
            text:'MOVIES',
            current:false
          },
          {
            text:'TV',
            current:false
          },
          {
            text:'GAMES',
            current:false
          },
          {
            text:'COLLECTIBLES',
            current:false
          },
          {
            text:'VIDEOS',
            current:false
          },
          {
            text:'FANS',
            current:false
          },
          {
            text:'NEWS',
            current:false
          },
          {
            text:'SHOP',
            current:false
          }
        ]
      }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';
.wrap{
    
    img{
        height: 80px;
    }
    ul{
        display: flex;
        li{
            a{
                display: inline-block;
                margin-left: 2rem;
                padding: 35px 0;
                color: #4B4D50;
                font-size: 12px;
                font-weight: 600;
                &:hover,
                &.active{
                    border-bottom: 4px solid $brand-blue;
                    color: $brand-blue;
                } 
            }
        }
    }
}
</style>