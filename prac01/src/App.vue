<template>
  <div>
    <!-- <h4 class="red" :style="changeColor">다다 원룸</h4> -->
    <!-- HTML속성도 데이터 바인딩 가능! :속성="데이터이름"-->
    <h4>{{products[0]}}</h4>
    <p>100 만원</p>
  </div>
  <div>
    <h4>{{products[1]}}</h4>
    <p>70 만원</p>
    <!-- <p>{{ price2 }} 만원</p> --> <!-- 실시간 자동 렌더링 하기 위해 데이터 바인딩 사용 -->
  </div>
  <div>
    <h4>{{products[2]}}</h4>
    <p>100 만원</p>
  </div>
</template>

<script>

export default {
  name: 'App',
  data() { // 데이터 보관함
    return { // object 자료로 저장할 것
      // price1: 100,
      // price2: 60,
      changeColor: "color : blue",
      products: ["역삼동원룸", "천호동원룸", "마포구원룸"]
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
  margin-top: 60px;
}
</style>
