<template>
  <div>
          <button>LOAD MORE</button>
      </div>
</template>

<script>
export default {
    name:'LoadBtn'
}
</script>

<style lang="scss" scoped>
@import '../assets/style/variables.scss';

    div{
        text-align: center;
        button{  
             padding: 0.5rem 4rem;
             border: none;
             margin-top: 50px;
             font-size: 14px;
             font-weight: 600;
             font-family: 'Roboto', sans-serif;
             background-color: $brand-blue;
             color: #fff;
             cursor: pointer;
        }
    }
</style>