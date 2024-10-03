<template>
  <div class="menu">
      <a v-for="(m,i) in menu" :key="i">{{m}}{{i}}</a>
  </div>

  <div>
    <h4 :style="스타일1">{{products[0]}}</h4>
    <p>{{price1}} 만원</p>
  </div>
  <div>
    <h4 :style="스타일2">{{products[1]}}</h4>
    <p>{{price2}} 만원</p>
  </div>
  <div>
    <h4 :style="스타일3">{{products[2]}}</h4>
    <p>{{price3}} 만원</p>
  </div>
</template>

<script>
export default {
  name: 'App',
  data(){
    return{
      menu : ['Home','Shop','About'],
      price1 : 60,
      price2 : 70,
      price3 : 80,
      스타일1 : 'color:blue',
      스타일2 : 'color:red',
      스타일3 : 'color:pink',
      products : ['역삼동원룸', '천호동원룸', '마포구원룸'],
    }
  },
  components: {

  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* margin-top: 60px; */
}

.menu {
  background: darkslateblue;
  padding: 15px;
  border-radius: 5px;
}
.menu a {
  color: white;
  padding: 10px;
}
</style>
