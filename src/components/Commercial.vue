<template>
  <section>
      <div class="wrap">
        
        <div v-for="(commercial,index) in commercials" :key="index">
            <a href="#">
                <img :src="commercial.image" alt="">
                {{commercial.text}}
            </a>
        </div>
        
         
      </div>
  </section>
</template>

<script>
export default {
    name:'Commercial',
    data(){
        return{
            commercials:[
                {
                    image:require('../assets/img/buy-comics-digital-comics.png'),
                    text:'DIGITAL COMICS'
                },
                {
                    image:require('../assets/img/buy-comics-merchandise.png'),
                    text:'DC MERCHANDISE'
                },
                {
                    image:require('../assets/img/buy-comics-subscriptions.png'),
                    text:'SUBSCRIPTIONS'
                },
                {
                    image:require('../assets/img/buy-comics-shop-locator.png'),
                    text:'COMIC SHOP LOCATOR'
                },
                {
                    image:require('../assets/img/buy-dc-power-visa.svg'),
                    text:'DC POWER VISA'
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';
    section{
        padding: 50px 1rem;
        background-color: $brand-blue;
        .wrap{
            justify-content: space-around;
            div{
                padding-right: 1rem;
                &:hover{
                    background-color: rgba(#fff, .3);
                }
                &:last-child img{
                    width: 60px;
                }
                a{
                color: #fff;
                display: flex;
                align-items: center;
                  img{
                      height: 60px;
                      margin-right: 1rem;
                  }
                }
            }
        }
    }
</style>