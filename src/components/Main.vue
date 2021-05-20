<template>
  <main>
      <div class="wrap"><h1> {{ istruzioni }} </h1></div>
  </main>
</template>

<script>
export default {
    name:'Main',
    data(){
        return{
            istruzioni:"-->CONTENT GOES HERE<--"
        }
    }
}
</script>

<style lang="scss" scoped>
main{
    padding: 50px 0;
    background-color: #1c1c1c;
    h1{
        color: #fff;
        font-size: 22px;
    }
}


</style>